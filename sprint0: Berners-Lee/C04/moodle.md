## Introducció  

En aquest mòdul, aprendràs a utilitzar Git i GitHub per gestionar el desenvolupament de software de manera eficient i col·laborativa. El teu objectiu serà:

- Garantir la traçabilitat del codi, registrant canvis i decisions de manera clara.
- Treballar en equip amb GitHub, compartint i revisant codi de forma ordenada.
- Integrar canvis sense errors, resolent conflictes i aplicant fluxos de treball estructurats.
- Seguir bones pràctiques com commits significatius, branques temàtiques i documentació coherent.

Utilitzaràs Git per controlar versions localment i GitHub per sincronitzar el treball en entorns remots. Al final, dominaràs eines essencials per contribuir a projectes reals amb seguretat i rigor.

La durada estimada d'aquest mòdul és de **4 hores**.  

Comencem.

### Objectius d'aprenentatge  

1. **Diferenciar Git de GitHub**: Entendre les diferències fonamentals entre Git (sistema de control de versions) i GitHub (plataforma de col·laboració).
2. **Instal·lar i configurar Git**: Configurar nom d'usuari, correu electrònic i editor per defecte a l'entorn local.
3. **Crear i gestionar repositoris locals**:Inicialitzar un repositori local amb `git init` i entendre l'estructura bàsica.
4. **Identificar els estats dels canvis a Git**: Distingir entre canvis modificats (working directory), preparats (staging area) i versionats (commits).
5. **Utilitzar ordres bàsiques d'inspecció**: Emprar `git status` per verificar l'estat actual i `git log` per revisar l'historial de commits.
6. **Fer commits efectius**: Crear commits amb missatges descriptius seguint l'estàndard Conventional Commits (ex: feat:, fix:).
7. **Vincular repositoris locals i remots**: Configurar una connexió entre un repositori local i un remot a GitHub amb git remote add.
8. **Clonar repositoris remots**: Duplicar un repositori remot en local amb `git clone`.
9. **Sincronitzar canvis locals amb el remot**: Pujar canvis al repositori remot amb git push.
10. **Sincronitzar canvis remots en local**: Actualitzar el repositori local amb canvis del remot mitjançant `git pull` o `git fetch`.
11. **Treballar amb branques**: Crear branques (git branch), canviar entre elles (`git checkout`/`git switch`), i eliminar-les.
12. **Realitzar fusions bàsiques (merge)**: Integrar canvis d'una branca a una altra amb `git merge` sense conflictes.
13. **Gestionar conflictes de fusió**: Identificar conflictes en fusions i resoldre'ls manualment amb eines com `git diff` o editors de codi.
14. **Bifurcar (fork) repositoris a GitHub**: Crear una còpia personal d'un repositori extern a GitHub per contribuir-hi.
15. **Crear i gestionar pull requests**: Proposar canvis a repositoris externs mitjançant sol·licituds d'incorporació (pull requests) a GitHub.
16. **Revisar i aprovar pull requests**: Analitzar canvis, deixar comentaris i integrar sol·licituds d'incorporació en projectes col·laboratius.


### Metodologia  
El mòdul consta de tres apartats diferenciats: teòric, pràctic i qüestionari d'autoconeixement.  

- Per a la teoria, hauràs d'**elaborar** uns apunts i lliurar la **URL** al final d'aquesta unitat.  

- Per a la part pràctica, treballaràs al Visual Studio Code. Els exercicis els pujaràs a la plataforma.
- El qüestionari el resoldràs a la plataforma.  

## Fonaments teòrics (1,5 h)  
Per construir la teva base teòrica, hauràs d'investigar **una sèrie de temes** i elaborar un glossari de termes que has de conèixer.  

### Temes d'investigació  

- Necessitat del control de versions: historial de canvis, col·laboració, resolució de conflictes.  
- Conceptes bàsics: *commit*, *repository*, *branch*, *merge*, *clone*.  
- Estratègies de ramificació (*branching strategies*): main/dev/feature branches, *tags* per versions.  
- Protocols per a treball en equip: pull requests, code reviews, *forking workflow*.  
- `git init`, `git add`, `git commit`, `git push`, `git pull`, `git checkout`, `git merge`, `git status`, `git log`.  
- Crear i gestionar repositoris remots, sincronització local-remot, *issues*, *projects*, *milestones*.  
- *GitHub Actions*: automatització de tasques (CI/CD), execució de tests, desplegament.  
- *Git Hooks*: scripts per automatitzar accions abans/després d’esdeveniments (p.e., pre-commit).   

### Recursos  

  - [Version control](https://developer.mozilla.org/en-US/docs/Learn_web_development/Core/Version_control)
  - [About Git](https://docs.github.com/en/get-started/using-git/about-git)
  - [Hello World](https://docs.github.com/en/get-started/start-your-journey/hello-world)
  - [Adopt a Git branching strategy](https://learn.microsoft.com/en-us/azure/devops/repos/git/git-branching-guidance?view=azure-devops)
  - [GitHub flow](https://docs.github.com/en/get-started/using-github/github-flow)
  - [Git command list](https://docs.github.com/en/get-started/start-your-journey/hello-world)  
  - [Github Glossary](https://docs.github.com/en/get-started/learning-about-github/github-glossary#pull-request)
  - [Creating an example workflow](https://docs.github.com/en/actions/use-cases-and-examples/creating-an-example-workflow)
  - [GitHub Actions documentation](https://docs.github.com/en/actions)

## Exercici pràctic 1: Git-it-electron (1 h)  

### Context
Aquesta aplicació inclou reptes per aprendre Git i GitHub utilitzant l’entorn real de Git i GitHub, no emuladors. Aprendràs a utilitzar la línia de ordres, que és increïble (i no tan terrorífica), i GitHub. Això vol dir que, quan completis tots els reptes, tindràs repositoris reals al teu compte de GitHub i quadrats verds al teu gràfic de contribucions. 

### Objectius d’aprenentatge
- ordres bàsics de Git.
- Treballar amb branques de Git.
- Fer pull-request a GitHub.

### Passos a seguir
1. Instal·la el joc des de [sourceforge](https://sourceforge.net/projects/git-it.mirror/) o desde el mateix repositori de [github](https://github.com/jlord/git-it-electron/releases)
2. Completa els reptes del joc.

## Exercici pràctic 2: Git-flow (1 h)  
### Context
Aprendre a gestionar el treball en **branques de Git** i la metodologia **Git-Flow** facilita el treball col·laboratiu en projectes de desenvolupament d'aplicacions. Aquest exercici **reprodueix** un escenari de treball en equip, per la qual cosa **has de col·laborar amb un company/a**.  

Durant l'activitat, **haureu de buscar les ordres adequades** per resoldre cada pas de l'exercici.

Al final haurás de completar el questionari de resolució de l'exercici.

### Objectius d’aprenentatge
- Introduir l’ús de Git com a eina i de Gitflow com a metodologia per al sistema de gestió de versions d’un projecte digital.  

### Passos a seguir

Aquest exercici s’ha de fer **en parelles**. Trieu qui serà la **Persona 1** i la **Persona 2**.  

#### Nivell 1: Obligatori
1. Les dues persones obriu la **Terminal** al vostre ordinador i trieu la ruta on voleu desar el projecte.  
2. **Persona 1**: A GitHub, creeu un projecte públic anomenat `git_flow` i compartiu l’URL del projecte amb la Persona 2.  
3. **Totes dues persones**: Dins del projecte creat a GitHub, copieu l’URL per clonar el repositori.  
4. **Totes dues persones**: Clonar el repositori en local
5. **Totes dues persones**: Obrir el projecte en VScode.
6. **Una persona del duo**: Crear un fitxer `index.html` i afegiu-hi el títol:  
"Gitflow sota control"
7. **La mateixa persona**: Des de la terminal del VSCode:  
   - Afegir els canvis a la staging area  
   - Fer un commit  (recorda fer commits convencionals)
   - Pujar els canvis al repositori remot
8. **Totes dues persones**: Actualitzar el projecte local

#### Nivell 2: Obligatori

9. **Una persona**: 
   - Crear la branca `develop`
   - Pujar-la a github
10. **Totes dues persones**: 
   - Canviar a la branca `develop`creada
   - Afegir al fitxer `index.html` els següents paràgraf sota el títol:  
   - Persona 1: "Git és una eina útil que ens ajuda a controlar versions."
   - Persona 2: "Però la seva utilitat principal és en el treball col·laboratiu."
   - Pujar els canvis (i preparar-vos per conflictes 🔥):  
12. **Resoldre els conflictes** perquè tots dos paràgrafs apareguin en l’ordre correcte.🧯  

#### Nivell 3: Opcional  

13. **Una persona**: crear **4 branques** a partir de `develop`:  
    ```bash  
    feature/navbar  
    feature/main_section  # Ha de contenir l’h1 i els paràgrafs anteriors  
    feature/side  
    feature/footer  
    ```  
14. Cada persona afegirà al `index.html` un `h2` amb un títol lliure, **excepte** qui tingui la branca `main_section` (ha de mantenir l’`h1` i els paràgrafs).  
15. **Totes dues personas**: Pujar els canvis a la vostra branca.
16. **Una a una**: Fusionar la branca amb `develop` mitjançant un **Pull Request** a GitHub per demanar aprovació a la companya.  
17. **Una companya**: Acceptar els canvis al GitHub, fusionar-los a `develop` i eliminar la branca.  
18. Repetir fins que totes les branques estiguin fusionades.  
19. **BONUS**: ¿Has llegit sobre els fitxers `.gitignore`? 🧠  

## Lliuraments  

- Els apunts digitals propis del contingut treballat.  
- Entrega a la plataforma el llistat de punts de l'exercici 2 amb les ordres que has fet servir a cada pas.

## Autoevaluació dels coneixements (0,5 h)  

Respon **aquestes preguntes** als teus apunts per fixar coneixements i identificar dubtes:  

1. Saps distinguir git de github?
2. Quins ordres bàsiques fas servir per treballar amb git?
3. Saps fer _pull-requests_ i revisar-los