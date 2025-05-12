## Introducció  

Començaràs a treballar amb les eines per desenvolupar aplicacions webs. 
Al final de l'unitat hauràs de estar capacitat per configurar i manejar Visual Studio Code i les eines de l'ecosistema Node.js  (nvm, package managers, 
vite, package.json) i Vite.

La durada estimada d'aquest mòdul és de **3 hores**.  

### Objectius d'aprenentatge  

1. Conèixer els diferents components de la interfície d'usuari i personalitzar-la segons les teves preferències.
2. Escriure codi i utilitzar les funcions d'edició integrades, com IntelliSense i Code Actions, i aprendre sobre l'execució i depuració de codi.
3. Instal·lar una extensió de llenguatge i afegir suport per a un llenguatge de programació diferent.
4. Conèixer les millors pràctiques de la intel·ligència artificial (IA) en l'entorn de desenvolupament.
5. Instal·lar Node.js i els gestors de paquets de Node.
6. Conèixer i utilitzar les ordres bàsiques de npm per gestionar paquets de Node.js.
7. Conèixer i configurar el fitxer package.json per iniciar projectes de JavaScript.
8. Crear projectes amb Vite.
9. Configurar dependències en Vite.
10. Configurar l'entorn de producció en Vite.


### Metodologia  
El mòdul consta de tres apartats diferenciats: teòric, pràctic i qüestionari d'autoconeixement.  

- Per a la teoria, hauràs d'**elaborar** uns apunts i lliurar la **URL** al final d'aquesta unitat.  

- Per a la part pràctica, treballaràs al Visual Studio Code. Els exercicis els pujaràs a la plataforma.
- El qüestionari el resoldràs a la plataforma.  

## Fonaments teòrics (1,5 h)  
Per construir la teva base teòrica, hauràs d'investigar **una sèrie de temes** i elaborar un glossari de termes que has de conèixer.  

### Temes d'investigació  

- Quines són les característiques principals que defineixen Node.js com a entorn d'execució?
- Com funciona l'arquitectura event-driven i non-blocking I/O en Node.js?
- Quina diferència hi ha entre `package.json` i `package-lock.json`?
- Gestionar de dependències d'un projecte mitjançant npm
- Quins tipus de variables d'entorn suporta Vite i com es configuren?
- Què és el Hot Module Replacement (HMR) i quins avantatges ofereix en el desenvolupament?
- Quines eines integrades de VS Code són essencials per a la depuració de codi (breakpoints, watch expressions)?
- Com es personalitza l'entorn de desenvolupament amb extensions com ESLint, Prettier o GitLens?
- De quina manera pot assistir GitHub Copilot en l'escriptura o refactorització de codi?
- Que és Vite i quins tipus d'aplicacions pot generar
- Com es gestionen els diferents entorns (desenvolupament, producció) mitjançant variables d'entorn?
- Com s'integra el control de versions (Git) dins de l'entorn de VS Code?
- Quins avantatges ofereixen les eines modernes com Vite o HMR respecte a enfocaments tradicionals?
- Com influeix l'ús d'IA (ex: Copilot) en el procés de desenvolupament de software actual?  

### Recursos  

- [Tutorial: Get started with Visual Studio Code](https://code.visualstudio.com/docs/getstarted/getting-started)
- [Best practices for using Github Copilot](https://docs.github.com/en/copilot/using-github-copilot/best-practices-for-using-github-copilot)
- [ Searching for information > Using AI ](https://developer.mozilla.org/en-US/docs/Learn_web_development/Getting_started/Environment_setup/Browsing_the_web#using_ai)
- [Visual Studio Code keyboard shortcuts for Window](https://code.visualstudio.com/shortcuts/keyboard-shortcuts-windows.pdf)
- [Visual Studio Code keyboard shortcuts for macOS](https://code.visualstudio.com/shortcuts/keyboard-shortcuts-macos.pdf)
- [Visual Studio Code keyboard shortcuts for Linux](https://code.visualstudio.com/shortcuts/keyboard-shortcuts-linux.pdf)
- [Introduction to Node.js](https://nodejs.org/en/learn/getting-started/introduction-to-nodejs)
- [An introduction to the npm package manager](https://nodejs.org/en/learn/getting-started/an-introduction-to-the-npm-package-manager)
- [How To Use Node.js Modules with npm and package.json](https://www.digitalocean.com/community/tutorials/how-to-use-node-js-modules-with-npm-and-package-json)
- [Node Version Manager](https://github.com/nvm-sh/nvm)
- [Package Managers Comparison: Yarn, NPM, PNPM](https://www.cookielab.io/blog/package-managers-comparison-yarn-npm-pnpm)
- [Corepack-Handling package managers problems](https://www.totaltypescript.com/how-to-use-corepack)
- [Vite](https://es.vite.dev/guide/)

## Exercici pràctic: Creació i publicació d’un package npm (1 h)  

### Context
En aquest taller aprendràs a crear un package npm que mostri la data i l’hora actual. També aprendràs a publicar aquest package a npm i a utilitzar-lo en un projecte nou. Aquest exercici et permetrà entendre el procés de creació, publicació i ús de packages npm, una habilitat essencial per a desenvolupadors front-end i back-end.

### Objectius d’aprenentatge
- Entendre com inicialitzar un projecte npm.
- Aprendre a crear un script senzill en Node.js.
- Publicar un package a npm.
- Utilitzar un package npm publicat en un projecte nou.

### Passos a seguir
1. **Inicialitzar el projecte npm**
   - Crea un nou directori a la teva carpeta de projectes.
   - Dins de la nova carpeta, inicialitza un nou projecte npm
   - Completa la informació requerida, com el nom del package (busca un nom que reflexi l'utilitat), la versió (comença amb "0.0.1"), l'autor (teu usuari de npm) i la descripció.

2. **Crear l’script per mostrar la data i l’hora actual**
   - Crea un fitxer `index.js`.
   - Escriu una funció que imprimeixi la data i l’hora actual a la consola.

3. **Configurar `package.json`**
   - Afegeix un camp `main` al `package.json` que apunti al fitxer `index.js`.
   - Defineix un script personalitzat per executar el fitxer amb `node`.

4. **Publicar el package a npm**
   - Assegura’t que tens un compte a npm i que has iniciat sessió amb `npm login`.
   - Publica el package amb la comanda `npm publish`.

5. **Utilitzar el package en un projecte nou**
   - Crea un nou projecte "vanilla" "javascript" amb  **`vite`**
   - Instal·la el package que has creat abans dins d'aquest nou projecte.
   - Importa el package al fitxer `main.js` del projecte.
   - Comprova el resultat a la consola del navigador.

## Lliuraments  
- Els apunts digitals propis del contingut treballat.  
- Proporciona el nom del package publicat a npm.


## Autoevaluació dels coneixements (0,5 h)  

Respon **aquestes preguntes** als teus apunts per fixar coneixements i identificar dubtes:  

1. Defineix els següents conceptes i les seves funcionalitats principals:
    - Node.js
    - npm (Node Package Manager)
    - package.json
(Inclou almenys 2 característiques clau per cada element)
2. Explica quines ordres de npm són necessàries per:
    - Instal·lar dependències regulars
    - Instal·lar dependències de desenvolupament
    - Actualitzar totes les dependències
(Menciona com es reflecteixen aquestes accions al fitxer package-lock.json)
3. Què són les variables d'entorn i com es configuren en un projecte amb Vite?
    - Descriu el seu propòsit
    - Indica la convenció de noms que s'ha de seguir
    - Mostra l'estructura bàsica del fitxer .env
4. Com es configura i treballa amb un workspace a Visual Studio Code?
    - Detalla els passos per crear-lo
    - Menciona 2 avantatges d'utilitzar aquesta funcionalitat
    - Explica com gestionar múltiples carpetes dins d'un mateix workspace
5. Quines estratègies utilitzaries per integrar la IA (ex: GitHub Copilot) en el teu procés d'aprenentatge?
    - Descriu 3 casos pràctics d'ús (ex: generació de codi, resolució d'errors)
    - Com equilibraries la dependència de l'IA amb l'aprenentatge autònom?