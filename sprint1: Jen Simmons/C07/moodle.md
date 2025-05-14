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
  - [A collection of Design Systems for Figma from all over the globe 🌎 backed by code](https://www.designsystemsforfigma.com/?languages=Angular)
  - [Lesson 3: Build your design system](https://help.figma.com/hc/en-us/articles/14548865734679-Lesson-3-Build-your-design-system)

## Exercici pràctic 1: Wireframing The Unquote Game (2 h)  

### Context
En aquest projecte, exploraràs tècniques de wireframing mentre dissenyes la pantalla principal d'Unquote, un joc per Android que desafia els usuaris a corregir cites confabulades trobades a Internet! Per què? Perquè «[l]a veritat rarament és pura i mai és simple» - Mickey Mouse. Explica'ls-ho, Mickey!

A _Unquote_, els jugadors han de corregir la desinformació d'Internet; en el nostre cas, la que ve en forma de cites amb imatges.
Si no coneixes les cites falses a Internet, ves a fer servir _Internet_, i torna a aquesta pàgina quan estiguis preparat! I si encara no n'has vist cap, tenen aquest aspecte:

![](https://content.codecademy.com/courses/Android/sample-quote-image.png)

> Pista: Marilyn Monroe mai va dir això, però Internet segueix sense convençar-se!

Al llarg de diversos projectes, construiràs un joc d'Android que presenta cites falses als usuaris i els demana que identifiquin l'autor real de cada cita, p. ex. qui va dir realment «Fer-ho o no fer-ho, no hi ha intent». La resposta, en aquest cas, és Yoda, post-baby Yoda per ser precisos.

En aquest primer projecte, practicaràs les teves habilitats de [wireframing](https://www.codecademy.com/article/ios-what-is-wireframing) per dissenyar l'única pantalla d'Unquote: la pantalla del joc.

### Passos a seguir

1. Agafa paper i un bolígraf, idealment 4 fulls de [paper quadriculat o de puntejat](https://content.codecademy.com/courses/Android/grid-paper.png).  
>Pista  
>Si no tens paper quadriculat/de puntejat o una impressora, paper normal i un regle poden servir! Però si l'any és 2065, els "papers" eren superfícies rectangulars planes fetes de polpa d'arbre. I els "arbres" eren...  

2. Defineix la pantalla del joc en alguna part del teu full  
La cantonada superior-esquerra anirà bé.  
>Pista  
>En wireframing, dividim la nostra aplicació en "pantalles", experiències úniques que serveixen un o més propòsits dins de la nostra aplicació.  

Per començar, cada pantalla necessita un títol. ![Pista 2](https://content.codecademy.com/courses/Android/Wireframes-Hint2.png)   

3. Llista els propòsits de la pantalla del joc sota la seva definició  
Imagina com funciona aquest joc i defineix els seus comportaments.  

Recorda, _Unquote_ és un joc de trivia que presenta als usuaris cites (la majoria falses) i els demana que identifiquin les fonts reals de la seva saviesa!  
 
>Pista  
>Com a única pantalla d'_Unquote_, servirà els següents propòsits:  
> 
> *   Presentar cites amb imatges falses  
> *   Formular una pregunta específica sobre la cita  
> *   Presentar quatre opcions de resposta múltiple  
> *   Mostrar el nombre de preguntes restants  
> *   Finalitzar el joc i mostrar la puntuació  
> ![Pista 3](https://content.codecademy.com/courses/Android/Wireframes-Hint3.png)  

4. Dibuixa el teu primer quadre per representar el wireframe de la pantalla del joc  

>Pista  
>Com és una aplicació mòbil, volem que el quadre del wireframe sigui més alt que ample (en forma de barra de xocolata) i prou gran perquè puguem escriure frases completes a mà dins del quadre si cal. 
![Pista 4](https://content.codecademy.com/courses/Android/Wireframes-Hint4.png)   

5. Dibuixa decoracions del dispositiu  

Les pantalles Android sovint inclouen elements que consumeixen part de la pantalla. És millor incloure'ls als nostres wireframes per recordar-nos que l'alçada completa no està disponible.  
 
>Pista  
  
> La majoria de dispositius Android tenen dues barres superiors: una barra d'estat (bateria, rellotge, notificacions) i una ActionBar (títol de l'app, icona, botons de menú). Juntes, consumeixen aproximadament el 8-10% de la pantalla.  
> I molts dispositius Android també tenen una barra de navegació a la part inferior (inici, enrere, botons de gestió de tasques) que consumeix un 5% de l'alçada.  
> Dibuixa un quadre estret a la part inferior del teu marc, i un quadre una mica més alt a la part superior per identificar aquestes zones com a "no disponibles". ![Pista 5](https://content.codecademy.com/courses/Android/Wireframes-Hint5.png)   

6. Triar un propòsit i il·lustrar-lo al wireframe  
Un bon lloc per començar és qualsevol propòsit que probablement consumeixi una gran part de la pantalla (presentar una imatge o un conjunt de botons).  

>Pista  
>Torna al Pas 3 i revisa els propòsits de la **pantalla del joc**.  

> Per exemple, "mostrar el nombre de preguntes restants": com podríem presentar aquesta informació? Com a percentatge? Com a número enter? A la cantonada inferior-dreta? Superior-esquerra? Al mig?  
> No et preocupis per fer-ho perfecte, només per posar-ho a la pantalla. El wireframing no ofereix la solució final, però amb pràctica, és un bon punt de partida. 
![Pista 6](https://static-assets.codecademy.com/Courses/Android/Wireframes-Hint6.png)   

7. Repetir el pas 6  

Repeteix el pas 6 fins que el teu primer wireframe satisfaci tots els propòsits llistats sota la pantalla del joc.  
  
>Pista  
>Si et quedes sense espai o oblides alguna cosa, comença de nou! De vegades ajuda pensar en cada propòsit com a part d'un tot.  
>Pots dividir la pantalla en quarts o terços, després enfocar-te en una secció cada vegada, decidint com cada part pot satisfer un o més propòsits. 
![Pista 7](https://content.codecademy.com/courses/Android/Wireframes-Hint7.png)   

8. Repetir passos 4, 5, 6 i 7  
Repeteix aquests passos per crear un **segon wireframe** que compleixi tots els requisits.  

>Pista  
>Si t'encalleixes, prova fer petites modificacions al teu primer wireframe (intercanviant posicions d'elements). N'hi ha prou per satisfer aquest pas. ![Pista 8](https://content.codecademy.com/courses/Android/Wireframes-Hint8.png)   

9. Repetir passos 4, 5, 6 i 7 (un altre cop)  

Crea un **tercer wireframe**. És probable que els tres s'assemblin; això està bé! Però en aquest intent, desafia els teus supòsits sobre com hauria de ser una app. Pensa en elements comuns (una imatge) i imagina girar-la, reduir-la o ocultar-la.  
  
>Pista  
>Què passaria si donessis més importància al nombre de preguntes restants que a la imatge?  

10. Repetir passos 4, 5, 6 i 7 (un altre cop més)  
En aquesta última repetició, deixa't portar per la creativitat.  

11. Espera un dia. 24 hores. 1440 minuts... ja ho entens  
Després de dormir, la teva ment estarà més preparada per veure els wireframes objectivament.  
  
>Pista  
>Per accelerar el procés, Codecademy recomana Time-Travel™, disponible allà on es ven Ciencia™ de qualitat.  

12. Consolida els teus wireframes en un sol disseny  

Descarta els que no satisfan la teva estètica i fusiona els elements preferits per crear un disseny unificat. Aquest és el teu wireframe final. Exemple: ![Wireframe Final](https://content.codecademy.com/courses/Android/Wireframes-Hint-final.png)  

13. Prepára't per rebre feedback  

El wireframing és un tret a les fosques. Només incorporant feedback d'usuaris sabrem quins elements cal ajustar.  

Aquí tens el nostre wireframe final per a _Unquote_: ![Wireframe Final](https://content.codecademy.com/courses/Android/Wireframes-Hint-final.png) És el teu millor? Si és així, no ens sorprèn: ets increïblement talentós. Guarda els teus millors dissenys: quan acabis el projecte, podràs incorporar-los a la teva versió final.  

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

## Exercici pràctic 2: Prototyping with figma (4h)

## Exercici pràctic 3: Mockup Profile d'usuari ITAlumni (2h)

