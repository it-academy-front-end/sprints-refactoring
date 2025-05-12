## Introducció  

Com a part d’un equip àgil, **traduïxes necessitats del client** en tasques tècniques concretes. Utilitzes eines com les *user stories* i els *criteris d’acceptació* per delimitar l’abast de cada funcionalitat, i desenvolupes codi orientat a superar els escenaris de prova definits. Aquest enfocament et permet alliberar funcionalitats iterativament, assegurant que el producte final s’ajusti a les expectatives.  

La durada estimada d'aquest mòdul és de **3 hores**.  

## Objectius d'Aprenentatge

1. **Entendre els principis bàsics de l’entorn àgil**  
- Conèixer els **4 valors del Manifest Àgil** i com s’apliquen al desenvolupament front-end (ex: col·laboració amb dissenyadors).  
- Participar en **cercles d’stand-up diaris** per comunicar progrés i bloquejos.  

2. **Traduir dissenys a tasques amb històries d’usuari**  
- Redactar **històries d’usuari** senzilles per a components UI (ex: *"Com a usuari, vull un botó d’‘Afegir a la cistella’ visible per comprar ràpid"*).  
- Descompondre històries en **tasques tècniques front-end** (ex: maquetar HTML/CSS, implementar funcionalitat amb JavaScript).  

3. **Gestionar tasques amb Kanban i prioritats**  
- Organitzar tasques en un **tauler Kanban** (ex: Trello) amb columnes: *To Do / In Progress / Done*.  
- Aplicar **MoSCoW** per decidir quines funcionalitats són *Must-Have* (ex: navegació responsive) vs. *Could-Have* (ex: animacions).  

4. **Escriure tests bàsics per a components UI**  
- Definir **criteris d’acceptació** visuals i funcionals (ex: *"El botó ha de canviar de color en hover"*).  
- Crear **escenaris de prova** senzills amb Gherkin (ex: *Donat que l’usuari està a la pàgina de producte, quan clica ‘Afegir a la cistella’, llavors el comptador de la cistella s’incrementa*).  

5. **Col·laborar amb eines de desenvolupament**  
- Practicar **pair programming** per a resoldre errors de maquetació o lògica.  

## Metodologia  
El mòdul consta de tres apartats diferenciats: teòric, pràctic i qüestionari d'autoconeixement.  

- Per a la teoria, hauràs d'**elaborar** uns apunts i lliurar la **URL** al final d'aquesta unitat.  
- Per a la part pràctica, treballaràs al Visual Studio Code. Els exercicis els pujaràs a la plataforma.
- El qüestionari el resoldràs a la plataforma.  

## Fonaments teòrics (1,5 h)  
Per construir la teva base teòrica, hauràs d'investigar **una sèrie de temes** i elaborar un glossari de termes que has de conèixer.  

### Temes d'investigació  

1. **Cicle de vida del desenvolupament de software (SDLC)**  
   Fases típiques dins d’un projecte de software i com s’integra amb metodologies àgils.
 
2. **Fonaments d’Agile i manifest àgil**  
   - Valors i principis, i per què Agile és útil en entorns de canvi constant.
   - Col·laboració, adaptació, lliuraments incrementals.  
   - Diferències entre mètodes tradicionals (Waterfall) i Agile.

3. **Extreme Programming (XP)**  
   Pràctiques clau com *pair programming*, *test-driven development*, *refactoring*, *continuous integration*, *planning game* i *collective code ownership*.

4. **Històries d’usuari**  
   Estructura i redacció d’històries útils (Rol + Acció + Valor).

5. **Criteris d’acceptació**  
   Què són, com es defineixen i per què són importants per validar el compliment dels requisits.

6. **Escenaris de prova**  
   Com descriure situacions concretes d’ús per provar funcionalitats, utilitzant llenguatge comprensible per tots els rols.

7. **Sintaxi Gherkin i format Donat/Quan/Llavors**  
   Com utilitzar aquest format per comunicar requeriments i proves de manera clara i estructurada.

8. **Descomposició de funcionalitats en tasques tècniques**  
   Com transformar una història d’usuari i els seus criteris en tasques concretes per al desenvolupament.

9. **Taulers Kanban**  
   - Ús de taulers per a la gestió del flux de treball i el seguiment de tasques dins d’un projecte àgil.
   - Priorització amb MoSCoW (Must-Have, Should-Have, Could-Have).  
   - Backlog management (kanban)

10. **Pair programming**  
   Pràctica del desenvolupament en parella: rols de *driver* i *navigator*, beneficis i estratègies per aplicar-la correctament.


#### Glossari:

Manifest Àgil, Extreme Programming (XP), Pair Programming, Test Driven Development (TDD), Refactoring, Continuous Integration (CI), MoSCoW, Continuous Deployment (CD), Històries d'usuari, Criteris d’acceptació, Escenaris de prova (Gherkin), Kanban, Trello, Jira, Taiga, MVP (Mínim Producte Viable), Sprint, Scrum, Feedback Continu, Funcionalitat, Desenvolupador, Kanban Board, Gestió de Tasques, Mètriques de Qualitat del Codi, Revisió de Codi (Code Review), Entorn de Staging, Documentació Mínima, Requisits Funcional, Requisits No Funcionals, Cicle de Vida del Desenvolupament de Software (SDLC), Iteració, Equip de desenvolupament, Client/Product Owner, Feedback continu, Millora contínua.


### Recursos  
  - [Cicle de vida del software](https://www.viewnext.com/el-ciclo-sdlc-en-7-fases/)
  - [Que és Agile](https://www.coursera.org/mx/articles/what-is-agile-a-beginners-guide)
  - [Que és Extreme Programming (XP)](https://asana.com/es/resources/extreme-programming-xp)
  - [Especificació de requisits](https://www.browserstack.com/guide/software-requirement-specifications-in-agile)
  - [Introducció a les històries d'usuaris](https://www.scrummanager.com/files/scrum_manager_historias_usuario.pdf)
  - [Definició de criteris d'acceptació i escenaris de prova amb gherkin](https://www.scrummanager.com/blog/2023/03/criterios-de-aceptacion-definicion-y-ejemplos/)
  - [Definició de tasques a partir d'històries d'usuari, criteris d'acceptació i escenaris de prova](https://www.pluralsight.com/resources/blog/guides/break-down-agile-user-stories-into-tasks-and-estimate-level-of-effort?utm_source=chatgpt.com)
  - [Priorització amb MoSCoW](https://www.uifrommars.com/priorizacion-metodo-moscow/)
  - [Bones practiques](https://github.com/it-academy-front-end/sprints-refactoring/blob/main/instruccions_alumnes/bones_practiques.md)

## Exercici pràctic 1: Registre d'usuaris (1 h)  

### Context
Treballaràs amb la següent història d'usuari:

*"*"Com a usuari de la botiga online, vull poder registrar-me amb el meu correu electrònic i contrasenya per crear un compte."*  

### Objectius d'aprenentatge
Planificar el desenvolupament d'una funcionalitat front-end seguint metodologia àgil: des de la història d'usuari fins al tauler Kanban prioritzat.  


### Passos a seguir
1. **Definir Criteris d'Acceptació**  
   - Llista 3-5 condicions **mesurables** que la funcionalitat ha de complir.  
   *Exemple*:  
   - [ ] Es validen en temps real que l'email tingui un format vàlid i que las contrasenyes siguin coincidents.  

2. **Escenaris de Prova amb Gherkin**  
   - Escriu 2 escenaris en sintaxi `Donat/Quan/Llavors` per validar els criteris.  
   *Exemple*:  
   ```gherkin  
   Escenari: Registre exitós  
      Donat que estic a la pàgina de registre  
      Quan omplo "email@exemple.com" al camp email  
      I escric "P@ssw0rd" als camps de contrasenya i confirmació  
      I clico "Registrar-me"  
      Llavors veig el missatge "Compte creat. Verifica el teu correu electrònic."  
      I sóc redirigit a /verifica-correu   
   ```  

3. **Desglossament de Tasques**  
   - Divideix la història en **tasques tècniques front-end** específiques:  
     *Exemple*:  
     - - Maquetar formulari de registre amb HTML/CSS (camps, botó, missatges d'error).  

4. **Organització en Tauler Kanban**  
   - Crea un tauler a **Trello** amb aquestes columnes:  
     - *Backlog* | *To Do* | *Doing* | *Test* | *Done*  
   - Afegeix les tasques com a targetes i prioritza amb **MoSCoW**:  
     - 🟢 **Must-Have**: Formulari bàsic funcional + validació inicial en enviar. 
     - 🟡 **Should-Have**: Validació en temps real (errors es mostren mentre l'usuari escriu).  
     - 🔵 **Could-Have**: Indicador de força de la contrasenya (barra de progrés).  
     - 🔴 **Won't-Have**: Registre amb xarxes socials (Facebook/Google).  

5. **Documentació**  
   - Crea una pàgina a **Notion** que inclogui:  
     1. Història d'usuari original.  
     2. Criteris d'acceptació i escenaris Gherkin.  
     3. Enllaç al tauler Kanban.  
     4. Captura de pantalla del codi més complex (ex: funció de filtrat).  
6. **Bonus track**: Repeteix l'exercici per la següent història d'usuari:

*"Com a usuari registrat, vull poder canviar la meva contrasenya perquè pugui mantenir el meu compte segur."*

### Autoevaluació
- [ ] Els Criteris d'Acceptació han de ser verificables (ex: "redirecció automàtica", no "registre ràpid").  
- [ ] Els enunciats Gherkin:  Mínim 2 escenaris amb estructura clara.  
- [ ] Al Tauler Kanban las tasques estan prioritzades amb etiquetes MoSCoW i distribuïdes en columnes.  
- [ ] Has documentat el procés de presa de decisions (ex: per què el slider és *Should-Have*).   

## Lliuraments  

- Els apunts digitals propis del contingut treballat.  
- L'exercici als apunts.

## Autoevaluació dels coneixements (0,5 h)  

Respon **aquestes preguntes** als teus apunts per fixar coneixements i identificar dubtes:  

1. Conèixes la notació de l'històries d'usuari i els criteris d'aceptació?
2. Saps desglosar una història en tasques i saps organitzar-les a un tauler Kanban ?
3. Saps com treballar en pair-programming?
