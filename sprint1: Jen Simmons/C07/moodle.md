## Introducció  

En aquesta unitat explorarem com el disseny i el codi s’integren per crear experiències digitals efectives. Això et servirà per treballar de la mà dels dissenyadors o millorar la coherència dels teus projectes.

En el món del desenvolupament web, no tot es redueix a escriure línies de codi. Saber interpretar un disseny, reutilitzar components eficientment i mantenir l’estètica consistent és clau per construir productes escalables i fàcils de mantenir. 

La durada estimada d'aquest mòdul és de **12 hores**.  

### Objectius d'Aprenentatge

1. **Prototipatge funcional**: Entendre i dissenyar wireframes i mockups per centrar-nos en el que realment importa: els fluxos d’usuari.
2. **Atomic Design**: Organitzar components (des de botons fins a pàgines senceres) com si fossin “Lego”, millorant la reutilització.
3. **Eines híbrides**: Ús de Figma per a dissenyar *i* exportar codi útil, i Storybook per documentar components com un professional.
4. **Integració codi-disseny**: Variables CSS (design tokens) i sistemes com Material UI per no reinventar la roda.


### Metodologia  
El mòdul consta de tres apartats diferenciats: teòric, pràctic i qüestionari d'autoconeixement.  

- Per a la teoria, hauràs d'**elaborar** uns apunts i lliurar la **URL** al final d'aquesta unitat.  
- Per a la part pràctica, treballaràs al Visual Studio Code. Els exercicis els pujaràs a la plataforma.
- El qüestionari el resoldràs a la plataforma.  

## Fonaments teòrics (1,5 h)  
Per construir la teva base teòrica, hauràs d'investigar **una sèrie de temes** i elaborar un glossari de termes que has de conèixer.  

### Temes d'investigació  

- Diferència entre *wireframe* i *mockup*.  
- Què és l'àtomic design i com ens pot ajudar a la reutilització de components per a escalabilitat.
- Qual són els elements bàsics d'una carta gràfica.  
- Investiga com s'utilitzen els frames, auto-Layout, els components i les variants en figma.
- Cóm fer un prototip interactiu amb figma
- Cóm funcionen els storybooks per documentar components.
- Concepte de *Design Tokens* (variables CSS, tipografia, espaiat).  
- Ús de sistemes de disseny existents (Material UI, Atlassian, Finastra).  


### Recursos  
  - [How to design an app in five steps](https://www.figma.com/resource-library/how-to-design-an-app/)
  - [What is Wireframing?](https://www.codecademy.com/article/ios-what-is-wireframing)
  - [What's the Difference Between a Wireframe, a Prototype, and a Mockup?](https://careerfoundry.com/en/blog/ux-design/difference-between-wireframes-prototypes-mockups/)
  - [The Definitive Guide: How To Make Your First Wireframe](https://careerfoundry.com/en/blog/ux-design/how-to-create-your-first-wireframe/)
  - [How to Make Wireframes for Mobile Apps and Websites: A Beginner's Guide](https://careerfoundry.com/en/blog/ux-design/wireframing-mobile-apps-websites/)
  - [Guide to prototyping in Figma](https://help.figma.com/hc/en-us/articles/360040314193-Guide-to-prototyping-in-Figma)
  - [Why Storybook?](https://storybook.js.org/docs/get-started/why-storybook)
  - [A collection of Design Systems for Figma from all over the globe 🌎 backed by code](https://www.designsystemsforfigma.com/?languages=Angular)
  - [Lesson 3: Build your design system](https://help.figma.com/hc/en-us/articles/14548865734679-Lesson-3-Build-your-design-system)

## Exercici pràctic 1: Wireframing del joc Farsa de Frases (2 h)  

### Context

En aquest projecte, aprendràs tècniques professionals de wireframing digital mentre dissenyes la pantalla principal de "Farsa de Frases", un joc per Android que desafia els usuaris a corregir cites manipulades trobades a Internet. Per fer aixó utilitzaràs l'eina **Figma** amb plugins especialitzats per a wireframing.

![](https://content.codecademy.com/courses/Android/sample-quote-image.png)
> Pista: Marilyn Monroe mai va dir això, però Internet segueix sense convençar-se!

### Objectius d'aprenentatge
- Crear wireframes digitals interactius
- Utilitzar components reutilitzables
- Aplicar principis d'arquitectura de la informació
- Optimitzar el flux de treball amb plugins

### Passos a seguir

- Abans de començar, configura Figma per a wireframing:
  1. Crea un nou fitxer a Figma
  2. Activa **Layout Grid** amb columnes de 12px de gutter
  3. Instal·la algun plugin de wireframing (ex. ink wireframe)
  4. Configura un _frame_ amb mida de dispositiu Android (ex: 412 x 917 px)

1. Defineix els **proposits del joc**. Per això has d'imaginar com funciona i definir els seus comportaments. 
  > Recorda, que _Farsa de Frases_ és un joc de trivia d'una única pantalla, presenta als usuaris cites (la majoria falses) i els demana que identifiquin les fonts reals de la seva saviesa!. L'usuari ha de escollir entre quatre opcions i és puntua els encerts. S'ha de mostrar el progrès del joc i, al final de les preguntes, la puntuació obtinguda.

2. Crea el **primer wireframe**: Utilitzant les eines del plugin de wireframing afegeix les decoracions del dispositiu (status bar i action bar).

3. Tria un dels propòsits anteriors i il·lustra-lo al wireframe.  
  > Un bon lloc per començar és qualsevol propòsit que probablement consumeixi una gran part de la pantalla (presentar una imatge o un conjunt de botons).  
  >Torna al Pas 3 i revisa els propòsits de la **pantalla del joc**.  
  > Per exemple, "mostrar el nombre de preguntes restants": com podríem presentar aquesta informació? Com a percentatge? Com a número enter? A la cantonada inferior-dreta? Superior-esquerra? Al mig?  
4. Repeteix el pas 3 fins que el teu primer wireframe satisfaci tots els propòsits llistats sota la pantalla del joc.  

5. Crea **3 versions** alternatives:
 - Versió jeràrquica (enfoc a imatge gran)
 - Versió minimalista (enfoc a opcions de resposta)
 - Versió experimental (layout no convencional)

### Autoevaluació

1. Quins elements són ESSENCIALS en la configuració inicial de Figma per a aquest exercici?  
- [ ] Afegir transicions animades  
- [x] Activar Layout Grid de 12px gutter  
- [x] Utilitzar mida de frame Android (ex: 412x917px)  
- [ ] Incloure icones en alta definició  
- [x] Instal·lar plugin de wireframing (ex: ink wireframe)  

**Retroalimentació**:  
La configuració correcta requereix:  
- Grid per alinear components  
- Mida realista de dispositiu mòbil  
- Plugins per agilitzar el procés  
*(Elements opcionals: animacions i icones detallades són per fases posteriors)*  

2. Quin d'aquests elements DEU CONTENDR el wireframe final segons els propòsits del joc?  
- [x] Barra d'estat (status bar)  
- [x] 4 opcions de resposta interactives  
- [ ] Música ambiental amb controls  
- [x] Indicador de progrés (preguntes restants)  
- [x] Àrea destacada per a la imatge de la cita  
- [ ] Enllaços a xarxes socials  

**Retroalimentació**:  
Elements obligatoris (Objectius):  
- Components de navegació Android (status/action bar)  
- Elements funcionals del gameplay (imatge, preguntes, respostes, progrés)  
*(Elements exclosos: música i xarxes socials no són part del wireframe bàsic)*  

3. Com s'hauria de diferenciar les 3 versions alternatives?  
- [x] Jeràrquica: Composició visual amb imatge com a element dominant  
- [ ] Corporativa: Ús de colors de marca institucional  
- [x] Minimalista: Reducció d'elements als essencials (botons/text)  
- [x] Experimental: Distribució no convencional (ex: opcions en cercle)  
- [ ] Internacional: Textos en 3 idiomes simultanis  

**Retroalimentació**:  
Les versions han d'explorar:  
- Prioritats visuals diferents (jerarquia vs minimalisme)  
- Innovació en layouts (experimental)  
*(Elements no requerits: internacionalització i identitat corporativa són decisions posteriors al wireframing)*  


## Exercici pràctic 2: Prototyping with figma - Clon de [PulseApp Pricing](https://pulseapp.com/pricing) (4h)

### Context
Aquest exercici et permetrà practicar les habilitats bàsiques i intermèdies de disseny i prototipatge amb Figma, recreant una pàgina web real. En clonar la pàgina de preus de PulseApp, aprendràs a estructurar components complexes, aplicar jerarquia visual i implementar interaccions com *hover effects* o navegació entre seccions.

### Objectius d'Aprenentatge
Al finalitzar l'exercici, seràs capaç de:
1. Utilitzar eines de disseny vectorial (eines de forma, text, icons) a Figma.
2. Aplicar **Auto Layout** per crear components responsius.
3. Prototipar interaccions bàsiques (transicions, overlays, navegació).
4. Organitzar capes i components de manera eficient.
5. Col·laborar mitjançant comentaris i versions a Figma.

### Passos a Seguir

1. Anàlisi de la Pàgina Original (15 min)
- Obre [pulseapp.com/pricing](https://pulseapp.com/pricing) i identifica:
  - Estructura de la pàgina (header, seccions de preus, FAQ, footer).
  - Components repetitius (ex: targetes de preus, botons, icons).
  - Colors, tipografies i espaiat.

2. Configuració del Projecte a Figma (10 min)
- Crea un nou fitxer a Figma.
- Defineix un **frame** amb les dimensions de pantalla d'escriptori (1440x900 px).
- Configura una graella de 12 columnes per al disseny responsive.

3. Disseny de Components (1 h 30 min)
 a) Header
  - Recrea el menú de navegació amb logo, enllaços i botó "Sign Up".
  - **Auto Layout**: Fes que els elements s'adaptin a canvis de text.

 b) Secció de Preus
  - Dissena 3-4 targetes de preus amb:
    - Llistes de característiques amb icons (✔️/❌).
    - Botons amb *hover effect* (canvi de color o ombra).
    - Utilitza **variants** per als estats actiu/inactiu.

 c) Secció de Comparació de Funcions
  - Crea una taula amb fileres alternes (fons gris/blanc).
  - Afegeix icons personalitzats amb eines de vector.

 d) Footer
  - Reprodueix les columnes d'enllaços i xarxes socials.

4. Prototipatge (30 min)
- Connecta els botons del menú a les seccions corresponents.
- Afegeix transicions suaus (**Smart Animate**) en fer clic.
- Prototipa el *hover* dels botons amb **Interactive Components**.

5. Revisió i Exportació (15 min)
- Comprova l'aliniament amb **Design System Check** (plugin).
- Exporta un PDF amb els wireframes i un enllaç al prototip interactiu.


### Questionari d'Autoavaluació

1. Per qué has fet servir l'Auto Layout.
2. Com es crea un hover effect.
3. Quins components has identificat a la pàgina original.
4. Com es pot reutilitzar un disseny de botó amb variants per estalviar temps.


**✅ Fes clic a "Present" a Figma quan acabis i comparteix el teu prototip amb #FigmaChallenge!**

## Exercici pràctic 3: Mockup Profile d'usuari ITAlumni (2h)


## Lliuraments  

- Els apunts digitals propis del contingut treballat.  
- L'exercici als apunts.

## Autoevaluació dels coneixements (0,5 h)  

Respon **aquestes preguntes** als teus apunts per fixar coneixements i identificar dubtes:  

1. Conèixes la notació de l'històries d'usuari i els criteris d'aceptació?
2. Saps desglosar una història en tasques i saps organitzar-les a un tauler Kanban ?
3. Saps com treballar en pair-programming?