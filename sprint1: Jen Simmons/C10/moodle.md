## Introducció  

En aquest mòdul, adquiriràs una visió general dels processos i entorns moderns de desplegament d'aplicacions web. Aprendràs a posar en producció projectes web utilitzant eines actuals i comprendre els fluxos de treball bàsics per a l'entrega contínua.  

Explorarem:  

- **Entorns de desplegament**: Diferències entre entorns de desenvolupament, proves i producció.  
- **Plataformes de hosting**: Serveis com Vercel, Netlify, GitHub Pages i serveis tradicionals (Shared Hosting, VPS).  
- **Integració contínua/Desplegament continu (CI/CD)**: Fluxos bàsics amb GitHub Actions.  
- **Contenidors Docker**: Introducció al concepte de contenidors i el seu paper en el desplegament.  
- **Monitorització bàsica**: Eines per verificar l'estat d'aplicacions desplegades.  

Aquesta unitat té una durada de 4 hores.  

### Objectius d'Aprenentatge  

- Identificar els components clau d'un entorn de producció.  
- Distingir entre diferents tipus de serveis d'hosting i els seus casos d'ús.  
- Configurar desplegaments automàtics en plataformes com Vercel/Netlify.  
- Utilitzar comandes bàsiques de Docker per gestionar contenidors.  
- Implementar un flux CI/CD bàsic amb GitHub Actions.  
- Interpretar errors comuns en el desplegament i aplicar solucions bàsiques.  
- Realitzar verificacions post-desplegament (checks de salut).  
- Entendre els conceptes de DNS i certificats SSL bàsics.  

### Metodologia  
El mòdul consta de tres apartats: teòric, pràctic i qüestionari d'autoconeixement.  

- **Teoria**: Elaboraràs apunts digitals i lliuraràs la URL al final.  
- **Pràctica**: Desplegaràs projectes a diferents plataformes.  
- **Qüestionari**: Resoldràs a la plataforma.  

## Fonaments teòrics (1,5 h)  
Per construir la teva base, investigaràs aquests temes i elaboraràs un glossari:  

### Temes d'investigació  
- Quins són els riscos de desplegar directament a producció sense entorns de prova?  
- Compara Shared Hosting, VPS i Serverless: costos, control i escenaris idonis.  
- Per què són importants els certificats SSL i com s'obtenen gratuïtament (Let's Encrypt)?  
- Què és un "build process" en aplicacions modernes i quines eines el realitzen (Webpack, Vite)?  
- Explica el flux bàsic d'un pipeline CI/CD: testeig, construcció i desplegament.  
- Quins beneficis ofereixen els contenidors Docker respecte a entorns tradicionals?  
- Descriu els errors més comuns en desplegaments: dependencies faltants, variables d'entorn no configurades, permisos.  

### Recursos  
- [Software Deployment Models – Explained for Beginners](https://www.freecodecamp.org/news/software-deployment-models/)  
- [How to Deploy Your Websites and Apps – User-Friendly Deployment Strategies](https://www.freecodecamp.org/news/how-to-deploy-websites-and-applications/)
- [20 Sites to deploy any application (Paid/Free alternatives)](https://dev.to/joselatines/sites-to-deploy-any-application-paidfree-alternatives-3em8)
- [Vercel Documentation](https://vercel.com/docs)  
- [Docker Getting Started](https://docs.docker.com/get-started/)  
- [GitHub Actions Guide](https://docs.github.com/es/actions/guides)  

## Exercici pràctic 1: Desplegament estàtic (2h)  

### Context  
Desplegaràs una pàgina HTML/CSS/JS simple a tres plataformes diferents: GitHub Pages, Netlify i Vercel.  

### Objectius  
- Experimentar amb fluxos de desplegament automatitzat.  
- Entendre les limitacions de cada plataforma.  
- Generar URLs públiques per als projectes.  

### Pas a pas  
1. **Prepara el projecte**:  
   - Crea una carpeta amb `index.html`, `style.css` i `script.js` bàsics.  
2. **GitHub Pages**:  
   - Puja el projecte a un repositori GitHub.  
   - Activa GitHub Pages a Settings > Pages (branch `main`).  
3. **Netlify**:  
   - Arrossega la carpeta del projecte al dashboard de Netlify.  
   - Configura el nom del projecte a `xxx-netlify.app`.  
4. **Vercel**:  
   - Importa el repositori GitHub a Vercel.  
   - Accepta les configuracions per defecte.  

### Lliurament  
- URLs dels tres desplegaments funcionant.  
- Captura de pantalla de cada configuració.  

---

## Exercici pràctic 2: CI/CD amb GitHub Actions (4h)  

### Context  
Configuraràs un pipeline bàsic que:  
1. Executa tests automàtics  
2. Construeix una aplicació React/Vite  
3. Desa el resultat a una branca `gh-pages`  

### Objectius  
- Crear un fitxer de configuració YAML per a GitHub Actions.  
- Entendre el concepte de "artefactes" en CI/CD.  
- Gestionar variables d'entorn secrets.  

### Pas a pas  
1. **Prepara el projecte**:  
   - Genera una app amb `npm create vite@latest` (escull React).  
   - Afegeix un test bàsic amb Vitest/Jest.  
2. **Configura GitHub Actions**:  
   - Crea el fitxer `.github/workflows/deploy.yml`.  
   - Defineix els passos:  
     - Checkout del codi  
     - Instal·la Node.js  
     - Executa `npm test`  
     - Construeix el projecte (`npm run build`)  
     - Desa la carpeta `dist` a `gh-pages`  
3. **Configura variables**:  
   - Afegeix un secret `GH_TOKEN` amb un token d'accés personal.  

### Lliurament  
- Enllaç al repositori amb el workflow funcionant.  
- Captura del historial d'execucions a GitHub Actions.  

---

## Lliuraments finals  
- URL dels apunts digitals amb el glossari.  
- Enllaços als exercicis pràctics.  
- Respostes al qüestionari d'autoavaluació.  

## Autoavaluació  
1. Quins factors decidirien triar Vercel sobre un Shared Hosting?  
2. Explica per què són necessàries les variables d'entorn en desplegaments.  
3. Què faries si una aplicació es veu localment però no en producció?  
4. Com permet Docker evitar el problema "funciona en la meva màquina"?  
5. Quins passos inclouries en un pipeline CI/CD per a una API?  
