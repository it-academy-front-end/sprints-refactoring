## Resolució de problemes amb eines i estratègies de desenvolupador  

## Introducció  
En aquest mòdul, aprendràs estratègies i eines essencials per diagnosticar i resoldre problemes de codi de manera eficient. Desenvoluparàs habilitats per pensar com un programador, utilitzar eines de depuració avançades i interpretar errors per millorar la qualitat del teu codi.  

## Objectius d'Aprenentatge  
- Aplicar el pensament lògic sistemàtic per descompondre problemes complexos.  
- Utilitzar Chrome DevTools/Firefox Developer Tools per inspeccionar codi, depurar i analitzar rendiment.  
- Identificar i resoldre errors comuns (sintaxi, referències null, tipus incorrectes) mitjançant missatges de consola.  
- Implementar estratègies d'aïllament d'errors com breakpoints, console.log i la paraula clau debugger.  
- Executar tasques de desenvolupament bàsiques amb terminal i npm scripts.  
- Analitzar bottlenecks de rendiment amb Performance, Network i Lighthouse.  

## Metodologia  
El mòdul combina:  
1. **Teoria**: Investigació i elaboració d'apunts sobre tècniques de depuració.  
2. **Pràctica**: Exercicis amb errors intencionats per resoldre amb eines de desenvolupador.  
3. **Autoavaluació**: Qüestionari per validar la comprensió dels conceptes.  

## Fonaments teòrics (1,5 h)  

### Temes d'investigació  
1. **Pensament computacional**:  
   - Com poden, la descomposició de problemes i l'abstracció simplificar la resolució d'errors?  
   - Busca exemples de transformació de problemes reals a passos algorísmics.  

2. **Depuració amb DevTools**:  
   - Funcionalitats clau del panel "Sources": breakpoints condicionals, call stack, i watch expressions.  
   - Com inspeccionar estats de variables i flux d'execució en temps real.  

3. **Interpretació d'errors**:  
   - Mapatge d'errors comuns (TypeError, ReferenceError) a les seves causes subjacents.  
   - Estratègies per identificar l'origen d'un "Cannot read property X of null".  

4. **Estratègies d'aïllament**:  
   - Quan utilitzar console.log vs. breakpoints? Pros i contres de cada enfocament.  
   - Tècniques per reproduir errors intermitents (entorns controlats, registres).  

5. **Terminal bàsica**:  
   - Comandes essencials de Git/NPM per gestionar dependències i executar tests.  
   - Automatització de tasques amb npm scripts (ex: `npm run debug`).  

6. **Anàlisi de rendiment**:  
   - Identificació de codi lent amb el flame graph de Performance.  
   - Optimització de càrrega de recursos amb el panel Network.  

### Recursos  
- [Chrome DevTools Documentation](https://developers.google.com/web/tools/chrome-devtools)  
- [What went wrong? Troubleshooting JavaScript](https://developer.mozilla.org/en-US/docs/Learn_web_development/Core/Scripting/What_went_wrong#types_of_error)
- [Debugging JavaScript in Firefox](https://firefox-source-docs.mozilla.org/devtools-user/debugger/)  
- [Common JavaScript Errors](https://rollbar.com/blog/top-10-javascript-errors/)  
- [npm Scripts Guide](https://docs.npmjs.com/cli/v8/using-npm/scripts)  
- [Lighthouse Performance Metrics](https://web.dev/learn/#lighthouse)  

## Exercici pràctic: Correcció d'errors en un joc d'endevinar nombres

### Context

En aquest exercici treballarem amb un joc d'endevinar nombres que no funciona correctament. El joc hauria de generar un nombre aleatori entre 1 i 100 i permetre a l'usuari endevinar-lo en 10 intents o menys, però conté diversos errors que impedeixen el seu funcionament adequat. 

Aquest exercici et permetrà practicar:
- Identificació de diferents tipus d'errors en codi JavaScript
- Ús d'eines de depuració del navegador
- Tècniques de correcció d'errors
- Comprensió de manipulació bàsica del DOM

### Objectius d'aprenentatge

1. Identificar i classificar diferents tipus d'errors (sintaxi, lògics, d'execució)
2. Utilitzar la consola del navegador per depurar errors
3. Aplicar mètodes sistemàtics per trobar i solucionar problemes en codi existent
4. Comprendre el funcionament bàsic de les interaccions DOM amb JavaScript
5. Desenvolupar estratègies per prevenir errors comuns

### Passos a seguir
1. **Prepara el repositori**: 
- Clona el repositori
```bash
$ git clone https://github.com/IT-Academy-BCN/it-sprint1-number-guessing-game.git  
$ cd it-sprint1-number-guessing-game
```
- Desconnecta el teu repositori del repositori de IT Academy. Utilitza la següent ordre de git:  
```sh  
$ git remote rm origin  
``` 
- Connecta el teu repositori amb el teu compte de GitHub:  
```sh  
$ git remote add origin <URL-del-teu-repositori>  
```  
2. **Executa el codi** i observa el comportament inesperat
3. **Identifica 5 errors** diferents al codi:
   - 2 errors de sintaxi
   - 2 errors lògics
   - 1 error de tipus
4. **Utilitza la consola** del navegador per obtenir missatges d'error
5. **Corregeix els errors** un per un, verificant després de cada correcció
6. **Assegura't** que el joc funcioni amb totes les funcionalitats:
   - Generació correcta de nombres aleatoris
   - Comptatge d'intents
   - Retroalimentació d'intents (massa alt/baix)
   - Finalització del joc (victòria/derrota)
   - Reinici del joc

### Eines que es poden fer servir

- Consola de desenvolupament del navegador (F12)
- Eines de depuració (breakpoints, debugger)
- `console.log()` per traçar l'execució
- Validadors de sintaxi JavaScript
- Documentació MDN Web Docs


## Lliuraments  
- URL dels apunts digitals amb glossari de termes.  
- Enllaç al repositori de l'exercici pràctic.  

### Questionari d'autoavaluació

1. Quin tipus d'error és més fàcil de detectar i per què?
   a) Errors de sintaxi
   b) Errors lògics
   c) Errors de tipus
2. Quina eina et va ser més útil per trobar errors i per què?
3. Explica la diferència entre els errors que es detecten en temps de compilació i els que es detecten en temps d'execució.
4. Com podries prevenir errors similars en el futur?
5. Quin error va ser el més difícil de trobar i per què?
