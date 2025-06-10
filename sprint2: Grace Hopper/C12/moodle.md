### Configuració i Treball amb TypeScript en el Desenvolupament Web  

## Introducció  
En aquesta unitat, dominaràs la integració de TypeScript en projectes web, des de la configuració inicial fins a l'aplicació de tipat avançat per millorar la robustesa i mantenibilitat del codi.  

Explorarem:  
- **Fonaments de TypeScript**: Sintaxi bàsica, tipus primitius, unions, aliases i interfícies.  
- **Configuració**: Compilació amb `tsconfig.json`, integració amb eines com Webpack/Babel.  
- **Estructures avançades**: Classes, genèrics, decoradors, i tipus condicionals.  
- **Integració amb frameworks**: Ús amb React/Angular/Vue.  
- **Pràctiques òptimes**: Validació de dades, gestió d'errors, i asincronia tipada.  

**Durada**: 12 hores  

### Objectius d'Aprenentatge  
- Configurar un entorn TypeScript amb `tsconfig.json`.  
- Utilitzar tipus estàtics per a variables, funcions i objectes.  
- Implementar interfícies i tipus per a validar estructures de dades.  
- Gestionar mòduls (import/export) amb tipat.  
- Compilar codi TypeScript i depurar errors de tipus.  
- Aplicar genèrics per a components reutilitzables.  
- Integrar TypeScript en frameworks frontend.  
- Implementar asincronia tipada amb `async/await`.  
- Utilitzar decoradors per a metadades avançades.  

### Metodologia  
- **Teoria**: Elaboraràs apunts digitals amb glossari de termes.  
- **Pràctica**: Exercicis al VS Code amb lliurament via GitHub.  
- **Autoavaluació**: Qüestionari a la plataforma.  


## Fonaments teòrics (1,5 h)  
### Temes d'investigació  
1. **Per què TypeScript millora la qualitat del codi respecte JavaScript pur?**  
   Analitza: Reducció d'errors en runtime, autocompletat intel·ligent i documentació viva mitjançant tipat.  
2. **Quines decisions clau implica configurar `tsconfig.json`?**  
   Investiga: Opcions com `strictNullChecks`, `noImplicitAny`, i el seu impacte en la seguretat.  
3. **Com defineixen les interfícies contractes de dades?**  
   Compara: Interfícies vs tipus, extensibilitat i ús en validació d'APIs.  
4. **Quins problemes resolen els genèrics en funcions i components?**  
   Exemples: Containers tipats (Array<T>), funcions reutilitzables.  
5. **Com gestiona TypeScript la integració amb llibreries JavaScript sense tipat?**  
   Recerca: Declaracions `.d.ts` i `@types` de DefinitelyTyped.  

### Recursos  
- [TypeScript Official Handbook](https://www.typescriptlang.org/docs/)  
- [TypeScript Deep Dive](https://basarat.gitbook.io/typescript/)  
- [TypeScript Config Cheat Sheet](https://www.typescriptlang.org/tsconfig)  
- [DefinitelyTyped Repo](https://github.com/DefinitelyTyped/DefinitelyTyped)  

---

## Exercici pràctic 1: Configuració i Tipat Bàsic (12h)  
### Context  
Configura un entorn TypeScript i resol exercicis de tipat per internalitzar sintaxi i compilació.  

### Objectius  
- Crear un projecte TypeScript des de zero.  
- Implementar tipus, interfícies i unions.  
- Gestionar errors de compilació.  
- Utilitzar ESM (mòduls) amb tipat.  

### Pas a pas  
1. **Inicialització**:  
   ```bash
   npm init -y
   npm install typescript @types/node --save-dev
   npx tsc --init  # Genera tsconfig.json
   ```
   Configura `tsconfig.json`:  
   ```json
   {
     "compilerOptions": {
       "target": "ES2020",
       "module": "ESNext",
       "strict": true,
       "outDir": "./dist"
     }
   }
   ```

2. **Exercicis**:  
   Crea `exercises/`:  
   - `basics.ts`: Defineix tipus per a:  
     ```ts
     type User = { name: string; age: number };
     const users: User[] = [/* ... */];
     ```
   - `functions.ts`: Implementa funcions tipades:  
     ```ts
     function sum(a: number, b: number): number { 
       return a + b; 
     }
     ```

3. **Tests**:  
   Executa tests amb `tsc` i `ts-node`:  
   ```bash
   npx tsc  # Compila a JS
   npx ts-node exercises/functions.test.ts
   ```

4. **Lliurament**:  
   - Commits amb [conventional commits](https://www.conventionalcommits.org/).  
   - URL del repositori GitHub amb exercicis resolts.  

### Autoavaluació  
1. Què fa l'opció `strict` a `tsconfig.json`?  
2. Com defineixes un tipus per a un objecte amb propietats opcionals?  
3. Quina diferència hi ha entre `interface` i `type`?  
4. Com tiparies una funció que retorna una Promise?  

---

## Exercici pràctic 2: BOTIGA ONLINE TIPADA (16-20h)  
### Context  
Implementa una botiga online amb TypeScript, fent èmfasi en:  
- **Tipat de dades**: Productes, carretó, usuaris.  
- **Gestió d'estat**: Centralitzat i tipat.  
- **Integració amb DOM**: Manipulació segura.  

### Objectius  
- Crear estructures de dades amb interfícies.  
- Gestionar esdeveniments amb tipat.  
- Utilitzar genèrics per a funcions reutilitzables.  
- Implementar un "state container" tipat.  

### Pas a pas  
#### Branques:  
| Versió          | Branca                     |
|-----------------|----------------------------|
| Configuració    | `feat/ts-config`          |
| Core Tipat      | `feat/core-typing`        |
| State Container | `feat/state-container`    |
| DOM Tipat       | `feat/dom-integration`    |

1. **Configuració inicial** (`feat/ts-config`):  
   - Crea `index.ts` amb importacions ESM.  
   - Configura Webpack o Vite per a TypeScript.  

2. **Core Tipat** (`feat/core-typing`):  
   Defineix interfícies:  
   ```ts
   interface Product {
     id: string;
     name: string;
     price: number;
   }
   interface CartItem extends Product {
     quantity: number;
   }
   ```

3. **State Container** (`feat/state-container`):  
   ```ts
   class StateContainer<T> {
     private state: T;
     constructor(initialState: T) {
       this.state = initialState;
     }
     // Implementa getters/setters tipats
   }
   ```

4. **DOM Tipat** (`feat/dom-integration`):  
   ```ts
   function createButton(text: string): HTMLButtonElement {
     const btn = document.createElement('button');
     btn.textContent = text;
     return btn;
   }
   ```

### Autoavaluació  
1. Com assegures que l'estat del carretó sempre sigui vàlid?  
2. Quins avantatges té un `StateContainer` tipat sobre un objecte JS pur?  
3. Com redueix TypeScript els errors en manipulació de DOM?  

---

## Lliuraments  
- **Apunts digitals**: Glossari amb termes TypeScript (URL).  
- **Repositoris GitHub**: Amb exercicis resolts.  
- **Qüestionari**: Respostes a la plataforma.  

> **Nota**: Tots els lliuraments es faran via la plataforma de l'Acadèmia.