## Introducció  

En aquest mòdul, construiràs una base sòlida en JavaScript modern següint principis de codi net en la pràctica del desenvolupament web. 

Explorarem:

- JavaScript Modern (ES6+): Sintaxi com funcions fletxa, desestructuració, mètodes inmutables d'array, mòduls (import/export), i gestió d'operacions asíncrones mitjançant promises i async/await.
- DOM Manipulation Eficient: Tècniques com seleccionar elements amb querySelector i optimitzar esdeveniments amb event delegation per evitar càrrega excessiva.
- Codi Net i Mantenible: Principis com SOLID (Single Responsibility, Open/Closed), DRY i KISS, amb èmfasi en separar lògica de negoci, DOM i estat. 
- Patrons Útils: Introducció a factory functions per crear elements dinàmicament i state containers per centralitzar dades.

Bonus Track
- Javascript Avançat: currying, Set, Map, Iterators i Generators, Operadors avançats: nullcoalescens operators,...

Aquesta unitat te una durada de 12 hores

### Objectius d'Aprenentatge

- Entendre i aplicar sintaxi com ara funcions fletxes, desestructuració i declaració de variables amb `const`/`let`.
- Utilitzar mètodes inmutables d'arrays.
- Utilitzar operadors avançats.
- Organitzar codi mitjançant mòduls (`import`/`export`) per a projectes estructurats.
- Gestionar operacions asíncrones amb callbacks i promises. Utilitzar la sintaxi `async`/`await`, i manejar errors de forma segura amb `try`/`catch`.
- Seleccionar i manipular elements del DOM de manera òptima amb `querySelector()`, evitant pràctiques ineficients com l’ús massiu d’`innerHTML`.
- Treballar amb esdeveniments de forma òptima, com implementant _event delegation_ mitjançant event.target per optimitzar el rendiment en aplicacions amb múltiples esdeveniments.
- Aplicar els principis SOLID
- Evitar els _code smells_ i aplicar patrons de codi net com DRY, KISS, YAGNI, etc.
- Separar clarament capes d’abstracció (lògica de negoci, DOM i estat).
- Aplicar patrons de disseny a la construcció de codi com _Factory_, _Moduler_ o _Observer_
- Gestionar l’estat de l’aplicació de manera centralitzada i ordenada amb state containers.

### Metodologia  
El mòdul consta de tres apartats diferenciats: teòric, pràctic i qüestionari d'autoconeixement.  

- Per a la teoria, hauràs d'**elaborar** uns apunts i lliurar la **URL** al final d'aquesta unitat.  
- Per a la part pràctica, treballaràs al Visual Studio Code. Els exercicis els pujaràs a la plataforma.
- El qüestionari el resoldràs a la plataforma.  

## Fonaments teòrics (1,5 h)  
Per construir la teva base teòrica, hauràs d'investigar **una sèrie de temes** i elaborar un glossari de termes que has de conèixer.  

### Temes d'investigació  
- ¿Com milloren les funcions fletxa, la desestructuració i const/let l’estructura i llegibilitat del codi respecte a les funcions tradicionals i var?
- Investiga: Diferències d’abast, hoisting, i casos pràctics on la desestructuració simplifica l’accés a dades complexes.
- ¿Quins avantatges aporten els mètodes inmutables d’arrays (map, filter, reduce) i operadors com el spread davant de mètodes destructius com push o splice?
- ¿Per què són clau els mòduls (import/export) per a projectes escalables?
- Analitza: Problemes de l’ús de variables globals amb <script> tradicionals i com els mòduls ajuden a evitar conflictes de noms i acoblament excessiu.
- ¿Com gestionar operacions asíncrones (API calls, temporitzadors) de forma llegible i segura amb async/await i try/catch?
- ¿Quins problemes resol l’event delegation amb event.target en interficies amb centenars d’elements interactius?
- Treu un llistat dels _code smells_ més importants i com es poden resoldre amb patrons de codi net.
- ¿Com dissenyar una aplicació que apliqui SOLID, separació de capes i patrons com Factory o Observer per a mantenibilitat?

### Recursos
- [The Modern JavaScript Tutorial](https://javascript.info/)
- [JavaScript Clean Code Guidelines](https://github.com/ryanmcdermott/clean-code-javascript)    
- [Cohesion and Coupling in Javascript](https://medium.com/@m-mdy-m/cohesion-and-coupling-in-javascript-0318f56d7ff2)
- [Code Smells](https://refactoring.guru/es/refactoring/smells)
- [Design Patterns in JavaScript: A Comprehensive Guide](https://dev.to/topefasasi/js-design-patterns-a-comprehensive-guide-h3m)

## Exercici pràctic 1: Funcionalitats modernes de JavaScript (12h)

### Contexte
Aquest projecte està dissenyat per introduir-te a les característiques modernes de JavaScript, des de ES6 fins a les versions més recents. A través d'exercicis pràctics, exploraràs conceptes com el block scoping, funcions fletxa, literals de plantilla, destructuració, noves APIs, i molt més. L'objectiu és que adquireixis una comprensió sòlida de com utilitzar aquestes funcionalitats per escriure codi més eficient, llegible i mantenible.

### Objectius d'aprenentatge
- Comprendre i aplicar el block scoping amb `let` i `const`.
- Utilitzar funcions fletxa per simplificar el codi i mantenir el context de `this`.
- Explorar literals de plantilla per interpolar cadenes i crear cadenes multi-línia.
- Aprendre a desestructurar objectes i arrays per accedir a dades de manera eficient.
- Familiaritzar-se amb les noves APIs com `Array.from`, `Object.assign`, i `String.includes`.
- Entendre i aplicar conceptes avançats com classes, promeses, async/await, iteradors, generadors, i més.

### Passos a seguir
1. **Preparació del repositori**: 
- Clona el repositori
```bash
$ git clone https://github.com/IT-Academy-BCN/it-sprint1-basics-js.git  
$ cd it-sprint1-basics-js
```
- Desconnecta el teu repositori del repositori de IT Academy. Utilitza la següent ordre de git:  
```sh  
$ git remote rm origin  
``` 
- Connecta el teu repositori amb el teu compte de GitHub:  
```sh  
$ git remote add origin <URL-del-teu-repositori>  
```  

2. **Instal·la les dependències**:
```bash
$ npm install
```
3. **Executa els tests**
- Utilitza Jest per executar els tests i veure quins passen i quins necessiten ser completats.
```bash
$ npm test
```
4. **Completa els exercicis**: 
- Cada fitxer dins del directori **`exercises`** conté tests que necessiten ser completats. Llegeix les instruccions dins de cada test i implementa el codi necessari per fer que passin.
- Pots llançar els tests en _mode watch_
```bash
$ npm run test:watch
```
- i seleccionar els fitxers d'un en un seguint les instruccions del terminal.

- Fes **un commit per cada test** que resolguis. Segueix les conventions de conventionalcommits.org

5. **Revisa les solucions**: 
- Un cop completats els exercicis, revisa les solucions per assegurar-te que has entès els conceptes.

### Lliurament de les respostes
- Completa els exercicis dins dels fitxers corresponents al directori exercises.
- Assegura't que tots els tests passen abans de fer el lliurament.
- Comparteix l'url del projecte complet als teus apunts.

### Autoavaluació
1. Quina diferència hi ha entre var, let i const? Quan hauries d'utilitzar cadascun?
2. Com funcionen les funcions fletxa i com gestionen el context de this?
3. Quins avantatges ofereixen els literals de plantilla en comparació amb la concatenació de cadenes?
4. Què és la desestructuració i com pots utilitzar-la per simplificar el teu codi?
5. Quines són algunes de les noves APIs introduïdes en ES6 i versions posteriors? Pots donar exemples pràctics d'ús?
6. Què són les promeses i com es relacionen amb async/await?
7. Pots explicar la diferència entre iteradors i generadors? Quan utilitzaries cadascun?

## Lliuraments  

- Els apunts digitals propis del contingut treballat.  
- L'exercicis als apunts.

## Exercici pràctic 2: SHOPPING CART (16-20h)

### Contexte
En aquest exercici construirem un carretó de la compra on explorarem dues formes diferents de gestionar esdeveniments:

1. Afegint un event listener individual a cada botó.
2. Utilitzant un únic event listener al contenidor pare (delegació d'esdeveniments).

A més, separarem la lògica de negoci (càlcul de preus, gestió dels articles) de la renderització (manipulació del DOM). Com a extra, utilitzarem _factory functions_ per crear elements dinàmics i gestionarem l'estat amb un _state container_ centralitzat.

 L'aplicació mostrarà una llista de productes amb un botó per afegir al carretó. El carretó mostrarà els productes afegits, la quantitat, el preu unitari i el preu total. També permetrà eliminar productes del carretó.

### Objectius d'aprenentatge
- Comparar el rendiment d'afegir listeners individuals vs. un únic listener al contenidor pare
- Separar la lògica de negoci de la renderització del DOM per mantenir un codi més net i mantenible.
- Utilitzar `factory functions` per crear elements dinàmics
- Implementar un _state container_ per gestionar l'estat de l'aplicació
- Practicar ES6+ (arrow functions, destructuring, template literals, etc.)

### Requisits
1. Crear una llista de productes amb botons per afegir al carretó
2. Implementar un carretó que mostri els productes afegits i el total
3. Comparar dues estratègies de gestió d'esdeveniments
4. Separar la lògica de càlcul de la renderització
5. (Extra) Utilitzar factory functions per crear elements
6. (Extra) Implementar un state container

### Pas a pas
#### Instruccions generals
1. Crea el teu propi repositori a GitHub amb el nom **it-sprint1-shopping-cart** (conèixes el [client per a GitHub](https://cli.github.com/))
2. Clona'l al teu entorn local. 
3. Crea la branca corresponent a l'exercici (veure taula següent).
4. Treballa la versió de l'exercici a la branca creada, **fes commit** cada vegada que **afegeixes** alguna funcionalitat o **arreglis** alguna cosa. 
5. Quan finalitzis la versió de l'exercici **puja-la** al repositori de github i obre un _**pull request**_ per fer un merge amb la branca **main**.

|Versió exercici|Nom branca|
|---|---|
|1|**feat/event-listeners-individuals**|
|2|**feat/event-delegation**|
|3|**feat/concerns-separation**|
|4|**feat/factory-functions**|
|5|**feat/state-container**|

#### Versió 1: Carretó amb _event listeners_ individuals per als botons d'afegir i eliminar

1. Crea un array de productes (objectes amb id, nom, preu). 

>TIP: Encara que l'idioma de l'aplicació sigui el català l'estructures del codi (noms de variables i funcions es millor que les facis en anglés)

2. Renderitza la llista de productes en el DOM. Cada producte ha de tenir:

    - Nom
    - Preu
    - Botó "Afegir al carretó"

3. Renderitza el carretó (inicialment buit). El carretó ha de mostrar:

    - Llista d'articles afegits (id, nom, quantitat, preu unitari, preu total per article).
    - Preu total del carretó.
    - Per cada article, un botó per eliminar-lo.

4. Afegeix _event listeners_ individuals a cada botó "Afegir" i "Eliminar":

    - Al fer clic a "Afegir", s'afegeix el producte al carretó (o s'incrementa la quantitat si ja existeix).
    - Al fer clic a "Eliminar" d'un article del carretó, es redueix la quantitat o s'elimina si la quantitat és 1.

5. Actualitza la vista del carretó cada vegada que es fa un canvi.

#### Versió 2: Delegació d'esdeveniments

1. Elimina els _event listeners_ individuals.
2. Afegeix un event listener al contenidor de la llista de productes (per capturar els clics en els botons "Afegir").
3. Afegeix un event listener al contenidor del carretó (per capturar els clics en els botons "Eliminar").
4. Utilitza la delegació d'esdeveniments per identificar quin botó s'ha clicat i actuar en conseqüència.

#### Versió 3: Separació de responsabilitats

1. Crea un mòdul per a la lògica de negoci (businessLogic.js) que contingui:

    - L'estat del carretó (un array d'objectes { id, nom, preu, quantitat }).
    - Funcions per afegir un producte, eliminar un producte, calcular el preu total, etc.

2. Crea un mòdul per a la renderització (render.js) que contingui funcions per:

    - Renderitzar la llista de productes.
    - Renderitzar el carretó.
    - Actualitzar el carretó quan l'estat canviï.

3. Utilitza un patró d'observador o simplement crida a les funcions de renderització des de les funcions que modifiquen l'estat.

#### Versió 4: Factory functions (extra)

1. Crea una factory function per crear un element de producte en la llista.
2. Crea una factory function per crear un element d'article en el carretó.

#### Versió 5: State container (extra)

1. Utilitza un objecte com a _state container_ que contingui l'estat del carretó i funcions per modificar-lo.
2. Fes que aquest objecte notifiqui als observadors (per exemple, la funció de renderització) quan l'estat canviï.

#### Més _Bonus tracks_

1. Afegeix la possibilitat de modificar quantitats directament al carretó
2. Implementa persistència de dades amb localStorage
3. Afegeix funcionalitat per buidar tot el carretó
4. Implementa un sistema de descomptes o promocions
5. Millora l'estil amb CSS

### Autoavaluació

1. Quins avantatges té la delegació d'esdeveniments sobre l'afegiment individual d'event listeners? I quins desavantatges?
2. Com hem separat la lògica de negoci de la renderització? Per què és important?
3. Què són les factory functions i com hem contribuït a la nostra implementació?
4. Com funciona el nostre state container? Quins beneficis aporta?


## Lliurament

- Crea un repositori a GitHub amb el projecte.
- Assegura't que cada part està ben documentada amb commits descriptius.
- Inclou un README.md que expliqui com executar el projecte i les decisions preses.
- Respon les preguntes d'autoavaluació


