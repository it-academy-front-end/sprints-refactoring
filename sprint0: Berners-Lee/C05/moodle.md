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
Una aplicació web permet registrar usuaris mitjançant un formulari (email i contrasenya). El flux inclou validacions, errors i interaccions entre components.  
Crear un **diagrama de flux** que representi el procés complet de registre d'usuari, incloent camins alternatius i punts de decisió.  

### **Objectius d'aprenentatge**  
1. Representar processos complexes amb diagrames de flux  
2. Utilitzar eines visuals o code-first per a documentació tècnica  
3. Identificar punts de fallada i camins alternatius  

### **Passos a seguir**  

1. **Tria una eina de diagramació**  
- **Code-first**: Mermaid.js (sintaxi Markdown)  
- **Visual**: Draw.io, Excalidraw o Lucidchart  

2. **Crea el diagrama de flux**  
   -  **Elements obligatoris**:  
      - **Nodes**:  
      - Inici/Fi  
      - Operacions (ex: "Usuari omple formulari")  
      - Decisions (ex: "Dades vàlides?")  
      - Connexions amb fletxes  
      - **Camins**:  
      - Flux principal (registre exitós)  
      - 2 camins alternatius (ex: email invàlid, error de connexió)  

3. **Afegir complexitat (Bonus)**  
- Inclou **3 nivells de validació**: format email, força contrasenya, disponibilitat email  
- Afegeix un **sistema de reintents** després d'errors  

4. **Documentació**  
- Integra el diagrama als apunts
- Explica en 2-3 línies les decisions de disseny més rellevants  

### **Autoevaluació**  
- [ ] El diagrama mostra mínim **8 nodes** i **3 decisions**  
- [ ] Inclou icones o colors per diferenciar tipus de nodes (opcional)  
- [ ] S'ha validat el renderitzat en l'eula triada  
- [ ] La documentació explica com milloraria el flux amb més temps  

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

## Lliuraments  

- Els apunts digitals propis del contingut treballat.  
- Els diagrames incorporats als apunts.

## Autoevaluació dels coneixements (0,5 h)  

Respon **aquestes preguntes** als teus apunts per fixar coneixements i identificar dubtes:  

1. Saps dissenyar un sitemap d'un projecte web?
2. Saps usar diagrams com user-flows o diagrames de seqüencia per dissenyar la lògica de l'aplicació ?
