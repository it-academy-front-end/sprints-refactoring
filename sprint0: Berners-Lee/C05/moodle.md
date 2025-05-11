## Introducció  

En aquesta unitat treballaràs el procés d'anàlisi i disseny. Abans de posar-te a codificar has d'**estructurar visualment** les decisions tècniques i l’experiència d’usuari. Per fer allò, pots utilitzar els **fluxos lògics** per definir com es relacionen les funcionalitats del sistema, **sitemaps** per organitzar l’arquitectura de la informació, i **user journeys/user flows** per anticipar com es mourà l’usuari dins de l’aplicació. Aquest enfocament et permetrà identificar errors de planificació en fases inicials i assegurar que el producte final sigui coherent i eficient.  

La durada estimada d'aquest mòdul és de **4 hores**.  

## Objectius d'Aprenentatge

1. **Dominar els tipus de diagrames clau i el seu propòsit**:  
   - Diferenciar **fluxos lògics**, **sitemaps**, **user journeys**, **UML** i **ERD**, entenent quan aplicar cada un (ex: fluxos lògics per relacions frontend-backend, ERD per bases de dades).  

2. **Utilitzar eines de diagramació (visuals i code-first) amb eficàcia**:  
   - Practicar amb eines com Lucidchart, Draw.io o Mermaid.js per crear diagrames clars, adaptant-los a l’escala del projecte.  

3. **Aplicar diagrames per estructurar decisions tècniques i d’usuari**:  
   - **Fluxos lògics**: Definir interaccions entre components del sistema.  
   - **Sitemaps**: Organitzar jerarquia de continguts i navegació.  
   - **User journeys/flows**: Anticipar moviments de l’usuari i detectar punts de fricció.  

4. **Validar i millorar el disseny abans del codi**:  
   - Usar diagrames com a filtres per identificar errors (funcionalitats incompatibles, fluxos trencats) i assegurar coherència entre totes les parts (ex: alinear user journeys amb l’arquitectura tècnica).  

5. **Integrar diagrames en la documentació tècnica**:  
   - Vincular diagrames amb especificacions escrites per facilitar la comunicació entre perfils tècnics i no tècnics.  

6. **Seleccionar críticament el tipus de diagrama segons la fase del projecte**:  
   - Decidir si es requereix un **sitemap** (fase d’arquitectura), un **diagrama de seqüència** (fase de desenvolupament) o un **cas d’ús UML** (fase d’anàlisi).  

7. **Col·laborar mitjançant diagrames compartits**:  
   - Utilitzar diagrames com a base per a discussions en equip i per validar decisions amb stakeholders.  

**Resultat esperat**: Al finalitzar, seràs capaç de **transformar requeriments funcionals** en diagrames estructurats que guiïn el desenvolupament d’una aplicació, millorant-ne la planificació i reduint errors en fases inicials. 🎯  


## Metodologia  
El mòdul consta de tres apartats diferenciats: teòric, pràctic i qüestionari d'autoconeixement.  

- Per a la teoria, hauràs d'**elaborar** uns apunts i lliurar la **URL** al final d'aquesta unitat.  

- Per a la part pràctica, treballaràs al Visual Studio Code. Els exercicis els pujaràs a la plataforma.
- El qüestionari el resoldràs a la plataforma.  

## Fonaments teòrics (1,5 h)  
Per construir la teva base teòrica, hauràs d'investigar **una sèrie de temes** i elaborar un glossari de termes que has de conèixer.  

### Temes d'investigació  

1. **Quins són els components bàsics d’un flux lògic i com es relacionen amb la interacció entre frontend i backend?**  
   - *Per què?* Entendre com es comuniquen les parts del sistema és fonamental abans de dissenyar funcionalitats.  

2. **En quins escenaris és més útil un sitemap que un user journey map?**  
   - *Per què?* Defineix quan prioritzar l’estructura de continguts (sitemap) sobre l’experiència d’usuari (journey map).  

3. **Com es diferencien els diagrames UML dels ERD en el disseny d’aplicacions?**  
   - *Per què?* Ajuda a triar l’eina correcta per modelar la lògica del sistema (UML) o les bases de dades (ERD).  

4. **Quines eines de diagramació són més eficaces (visuals vs. code-first) per a projectes web?**  
   - *Per què?* Decidir entre agilitat (ex: Draw.io) o integració amb codi (ex: Mermaid.js) optimitza el temps.  

5. **Quins elements clau s’han d’incloure en un user flow per anticipar problemes d’experiència d’usuari?**  
   - *Per què?* Identificar punts de fricció abans de codificar estalvia hores de debug.  

### Recursos  
  - [Què és l'algorítmia?](https://www.ionos.es/digitalguide/online-marketing/analisis-web/que-es-un-algoritmo/)  
  - [Tot és qüestió de lògica](https://www.youtube.com/watch?v=ajkglMnByFM)  
  - [Què és un flux de lògic?](https://www.lucidchart.com/pages/es/que-es-un-diagrama-de-flujo)  
  - [Què és un sitemap](https://miro.com/es/diagrama/que-es-sitemap/)  
  - [Com definir un user journey map](https://www.coursera.org/mx/articles/creating-user-journey-maps-a-guide)   
  - [Exemples de fluxos i journeys amb Figma](https://www.figma.com/community/file/1129569920411169134/user-flow-template-wireframe-flow)  
  - [Bones pràctiques de documentació visual](https://xd.adobe.com/ideas/process/wireframing/guide-user-flow-diagrams/)  
  - [Mermaid.js Live Editor](https://mermaid-js.github.io/mermaid-live-editor/) (per crear fluxos amb codi).  
  - [Flowmapp](https://flowmapp.com/) (eina especialitzada en sitemaps i user flows).  
  - [Lucidchart: Guia UML per a principiants](https://www.lucidchart.com/pages/uml-diagram) (exemples interactius).  
  - [MySQL Oficial: Disseny de bases de dades amb ERD](https://dev.mysql.com/doc/workbench/en/wb-erd-tutorial.html) (pràctic).  
  - [Draw.io](https://app.diagrams.net/) (plantilles predefinides per UML i ERD).  
  - [Draw.io: Tutorial en 10 minuts](https://www.youtube.com/watch?v=2O8pkybH6po) (vídeo, anglès).  
  - [Mermaid.js + VS Code](https://code.visualstudio.com/docs/languages/markdown#_mermaid-diagram-support) (integració directa).  
  - [Excalidraw](https://excalidraw.com/) (diagrames hand-drawn per esbossos ràpids).  
  - [Figma: Com dissenyar user flows](https://www.figma.com/blog/how-to-create-user-flows/) (pas a pas amb imatges).  
  - [Interaction Design Foundation: Usabilitat en UX](https://www.interaction-design.org/literature/topics/usability) (cursos profunds).  
  - [Figma Jam](https://www.figma.com/jam/) (per a prototips col·laboratius).  
  - [Dessign Toolkit de la UOC](https://design-toolkit.recursos.uoc.edu/).  


## Exercici pràctic 1: Registre d'usuaris (1 h)  

### Context
Imagina una aplicació web on l’usuari omple un formulari de registre (email i contrasenya). El frontend envia aquestes dades al backend, que valida la informació i retorna una resposta (èxit o error).  

### Objectius d'aprenantatge
Crear un **diagrama de seqüència** amb Mermaid.js que representi la interacció entre el frontend i el backend durant un procés de registre d’usuari.  

### Passos a seguir
1. **Configura Mermaid.js**:  
   - Obre l’[editor en línia de Mermaid](https://mermaid-js.github.io/mermaid-live-editor/) o configura Mermaid al teu entorn local (ex: VS Code amb extensió de Markdown).  

2. **Codi del diagrama**:  
   - Escriu la sintaxi de Mermaid per a un **diagrama de seqüència** que inclogui:  
     - **Actors**: Usuari, Frontend, Backend, Base de dades.  
     - **Passos**:  
       - L’usuari introdueix dades i fa clic a "Registrar-se".  
       - El frontend envia les dades al backend.  
       - El backend valida l’email (ex: format correcte) i la contrasenya (ex: longitud mínima).  
       - Si tot és correcte, el backend guarda les dades a la base de dades i retorna un missatge d’èxit.  
       - Si hi ha errors, el backend retorna un missatge d’error específic.  

3. **Bonus track**:  
   - Afegeix **notes** als passos crítics (ex: "Validar email amb regex").  
   - Inclou un **alt flux** per a un error de connexió amb la base de dades.  
4. **Bonus Bonus**

- **Integra el diagrama** en un document Markdown a GitHub i comparteix l’enllaç.  
- **Afegeix un tercer camí** per a un error de xarxa (ex: timeout).  

### Autoevaluació
- [] El diagrama es renderitza sense errors a l’editor de Mermaid.  
- [] Mostra **com mínim 4 participants** i **2 camins alternatius** (èxit/error).  
- [] Inclou **missatges amb descripcions tècniques** (ex: `POST /api/register`).  

## Exercici pràctic 2: Botiga online (1 h)  

### Context
La botiga "BotigaTech" ven productes electrònics (mòbils, ordinadors, accessoris) i necessita un sitemap clar per guiar el desenvolupament de la seva aplicació web.  

### Objectius d'aprenantatge
Crear un **sitemap** estructurat que representi la jerarquia de pàgines i la navegació d’una botiga online fictícia (ex: "BotigaTech").  

### Passos a seguir

1. **Configura Draw.io**:  
   - Obre [Draw.io](https://app.diagrams.net/) i tria la plantilla **"Flowchart"** o **"Blank Diagram"**.  

2. **Defineix la jerarquia principal**:  
   - Crea nodes per a les pàgines principals:  
     - **Pàgina d’inici** (`/`)  
     - **Productes** (`/productes`)  
     - **Categories** (`/categories`)  
     - **Cistella** (`/cistella`)  
     - **Compte d’usuari** (`/compte`)  
     - **Contacte** (`/contacte`)  

3. **Afegeix subpàgines**:  
   - Sota **Productes**, inclou:  
     - Detall d’un producte (`/productes/{id}`).  
   - Sota **Categories**, inclou:  
     - Mòbils (`/categories/mobils`), Ordinadors (`/categories/ordinadors`), Accessoris (`/categories/accessoris`).  

4. **Connexions i navegació**:  
   - Uneix els nodes amb fletxes per indicar el flux de navegació.  
   - Exemple: *Pàgina d’inici → Productes → Detall del producte*.  

5. **Elements visuals**:  
   - Utilitza **icones** (Draw.io té una llibreria integrada) per diferenciar tipus de pàgines:  
     - 🛒 per la cistella.  
     - 📱 per categories de mòbils.  

6. **Bonus track**:  
   - Afegeix notes als nodes per explicar decisions (ex: "La pàgina de contacte inclou formulari i mapa").

7. **Bonus Bonus**  
- **Exporta el sitemap com a XML** i penja’l a GitHub amb un fitxer `README.md` que l’expliqui.  
- **Crea una versió responsive** del sitemap que mostri com s’adaptaria la navegació a mòbil.  


### Autoevaluació
- [] El sitemap inclou **com a mínim 2 nivells de jerarquia** (ex: Categories → Subcategories).  
- [] Les connexions entre pàgines són **lògiques** (ex: No es pot accedir a "Detall producte" sense passar per "Productes").  
- [] S’han utilitzat **icones o colors** per diferenciar tipus de pàgines (ex: administratives vs. públiques).    

### Lliuraments  

- Els apunts digitals propis del contingut treballat.  

## Autoevaluació dels coneixements (0,5 h)  

Respon **aquestes preguntes** als teus apunts per fixar coneixements i identificar dubtes:  

1. Saps dissenyar un sitemap d'un projecte web?
2. Saps usar diagrams com user-flows o diagrames de seqüencia per dissenyar la lògica de l'aplicació ?
