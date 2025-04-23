# Exercici: Configuració de GitHub Actions per a Tests i Desplegament

## Objectiu
Configurar un workflow bàsic amb GitHub Actions per executar tests automatitzats (Vitest) i desplegar una aplicació React a GitHub Pages.

---

## Aplicació de React (Formulari de Registre)

### Requisits de l'aplicació:
1. **Tecnologies**: React (creat amb Vite), Vitest + React Testing Library.
2. **Funcionalitats**:
   - Formulari amb camps: Nom, Email, Contrasenya.
   - Validacions en temps real:
     - Nom: mínim 3 caràcters.
     - Email: format vàlid.
     - Contrasenya: mínim 6 caràcters.
   - Missatges d'error per cada camp.
3. **Tests**:
   - Verificar que el formulari es renderitza correctament.
   - Testejar validacions dels camps.

---

## Passos de l'exercici

### 1. Crear l'aplicació React
```bash
npm create vite@latest registre-app -- --template react
cd registre-app
npm install
```

### 2. Afegir Testing (Vitest)
```bash
npm install -D vitest jsdom @testing-library/react @testing-library/jest-dom
```

### 3. Codi de l'aplicació (Actualitza els fitxers)

#### `src/App.jsx`
```jsx
import { useState } from 'react';
import './App.css';

function App() {
  const [formData, setFormData] = useState({ name: '', email: '', password: '' });
  const [errors, setErrors] = useState({});

  const validateForm = () => {
    const newErrors = {};
    if (formData.name.length < 3) newErrors.name = "Nom massa curt";
    if (!/^\S+@\S+\.\S+$/.test(formData.email)) newErrors.email = "Email invàlid";
    if (formData.password.length < 6) newErrors.password = "Contrasenya massa curta";
    setErrors(newErrors);
    return Object.keys(newErrors).length === 0;
  };

  const handleSubmit = (e) => {
    e.preventDefault();
    if (validateForm()) {
      console.log("Formulari vàlid:", formData);
    }
  };

  return (
    <div className="container">
      <h1>Registre</h1>
      <form onSubmit={handleSubmit}>
        <div>
          <label>Nom:</label>
          <input 
            type="text" 
            value={formData.name}
            onChange={(e) => setFormData({...formData, name: e.target.value})}
          />
          {errors.name && <span className="error">{errors.name}</span>}
        </div>
        {/* Afegeix camps similars per email i contrasenya */}
        <button type="submit">Enviar</button>
      </form>
    </div>
  );
}

export default App;
```

#### `src/App.test.jsx`
```jsx
import { render, screen, fireEvent } from '@testing-library/react';
import App from './App';

describe('Formulari de Registre', () => {
  test('Mostra errors de validació', () => {
    render(<App />);
    fireEvent.click(screen.getByText('Enviar'));
    expect(screen.getByText(/Nom massa curt/i)).toBeInTheDocument();
    expect(screen.getByText(/Email invàlid/i)).toBeInTheDocument();
  });
});
```

### 4. Configurar GitHub Actions

#### Crea el fitxer `.github/workflows/main.yml`

Configura un workflow de GitHub Actions que:
1. Executi els tests **en fer push a main o obrir una PR**.
2. Desplegui a GitHub Pages **només si els tests passen**.

**Instruccions**: Completa els espais buits (___1___, ___2___, etc.) al següent codi YAML.

---

## Preguntes per desenvolupar el fitxer `.github/workflows/main.yml`

### 1. Events que activen el workflow
Quin bloc defineix els events que activaran l'execució?
```yaml
on:
  push:
    branches: [ ___1___ ]
  pull_request:
    branches: [ ___2___ ]
```

### 2. Nom del workflow
Quina directiva s'utilitza per donar nom al workflow?
```yaml
___3___: Tests i Desplegament
```

### 3. Job de tests
Com es defineix un job que s'executi en Ubuntu i instal·li les dependències?
```yaml
jobs:
  test:
    runs-on: ___4___
    steps:
      - uses: actions/checkout@v4
      - uses: ___5___@v4
        with:
          node-version: 20
      - run: npm install
      - run: ___6___
```

### 4. Dependència entre jobs
Com s'indica que el job de desplegament necessita que el job de tests passi?
```yaml
deploy:
  ___7___: test
```

### 5. Desplegament a GitHub Pages
Quina acció s'utilitza per desplegar a GitHub Pages?
```yaml
- uses: ___8___/actions-gh-pages@v3
  with:
    github_token: ${{ secrets.GITHUB_TOKEN }}
    publish_dir: ___9___
```

### 6. Variable global
Quina directiva s'hauria d'afegir per evitar problemes amb l'OS en desplegar?
```yaml
env:
  ___10___: npm
```

---

## Validació final
Un cop respostes totes les preguntes, crea el fitxer complet YAML i verifica que:
- S'executen els tests en fer push.
- El desplegament només es dispara si els tests són exitosos.

---

## Respostes correctes
1. `main`  
2. `main`  
3. `name`  
4. `ubuntu-latest`  
5. `actions/setup-node`  
6. `npm test`  
7. `needs`  
8. `peaceiris`  
9. `./dist`  
10. `NODE_ENV`  

**Exemple complet**:
```yaml
name: Tests i Desplegament

on:
  push:
    branches: [main]
  pull_request:
    branches: [main]

jobs:
  test:
    runs-on: ubuntu-latest
    steps:
      - uses: actions/checkout@v4
      - uses: actions/setup-node@v4
        with:
          node-version: 20
      - run: npm install
      - run: npm test

  deploy:
    needs: test
    runs-on: ubuntu-latest
    env:
      NODE_ENV: production
    steps:
      - uses: actions/checkout@v4
      - uses: actions/setup-node@v4
        with:
          node-version: 20
      - run: npm install
      - run: npm run build
      - uses: peaceiris/actions-gh-pages@v3
        with:
          github_token: ${{ secrets.GITHUB_TOKEN }}
          publish_dir: ./dist
```


### 5. Configuració addicional
1. **package.json**:
```json
{
  "scripts": {
    "dev": "vite",
    "build": "vite build",
    "test": "vitest"
  },
  "homepage": "https://<USERNAME>.github.io/<REPO-NAME>"
}
```

2. **Habilitar GitHub Pages**:
   - A GitHub: Settings → Pages → Source: `gh-pages` branch / `root`.

---

## Validació
1. Fes un push al repositori i verifica:
   - **Actions**: S'executen els tests automàticament.
   - **GitHub Pages**: L'aplicació es mostra en l'URL proporcionada.

2. Prova el formulari en l'entorn de producció.

---

## Notes
- Assegura't que el fitxer `vite.config.js` inclou la configuració base per a testing.
- Opcional: Afegeix més tests per als camps de password i email.
