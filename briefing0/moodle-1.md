## Introducció 

En aquesta unitat, aprendràs a interactuar amb el terminal com un professional: navegar directoris, manipular fitxers, crear scripts i gestionar permisos. Tot això et prepararà per treballar en entorns reals de desenvolupament.

> **Important**  
> Per aquesta unitat es recomana treballar amb l'entorn linux. Si el teu sistema operatiu es Windows es recomana instal·lar [WSL](https://learn.microsoft.com/es-es/windows/wsl/install) o com a mínim treballar al terminal de [bash](https://git-scm.com/downloads).  

La durada estimada d'aquest mòdul és de **3 hores**.  

### Objectius d'Aprenentatge
1. Utilitzar ordres bàsiques del terminal per gestionar fitxers i directoris.
2. Gestionar permisos d'accés.

### Metodologia  
Aquesta unitat consta de tres apartats diferenciats: teoria, pràctica i qüestionari d'autoconeixement.  

- Per a la teoria i la pràctica, hauràs d'**elaborar** uns apunts amb els processos i les teves conclusions i lliurar la **URL** al final d'aquesta unitat.  
- El qüestionari el resoldràs a la plataforma **Moodle**. 

## Fonaments teòrics (1,5 h) 
Per construir la teva base teòrica, hauràs d'investigar **una sèrie de temes y termes** que has de conèixer. Et donem alguns recursos que poden ser interessants i un glossari que us ajudaran a enfocar i orientar la vostra recerca. 

### Temes a investigar

- Introducció al terminal Linux: concepte de shell, terminal vs. interfície gràfica (GUI).
- Estructura del sistema de fitxers Linux: directoris arrel (/), rutes absolutes i relatives.
- Ordres bàsiques de navegació i gestió: `ls, cd, pwd, mkdir, touch, cp, mv, rm, cat, grep`
- Permisos de fitxers i directoris: chmod, chown, notació octal (755, 644).
- Manipulació de text: redirecció (>, >>, pipes |), editors de terminal com nano o vim (bàsics).
- Gestió de processos: ordres ps, kill, top, execució en segon pla (&, Ctrl+Z).
- Variables d’entorn: PATH, ordres echo, export, fitxers de configuració (.bashrc, .profile).

### Recursos

- [Dealing with files](https://developer.mozilla.org/en-US/docs/Learn_web_development/Getting_started/Environment_setup/Dealing_with_files)
- [Command line crash course](https://developer.mozilla.org/en-US/docs/Learn_web_development/Getting_started/Environment_setup/Command_line)
- [cheat sheet de ordres Linux](https://cheatography.com/jonathan992/cheat-sheets/gnu-linux-command-spanish/)
- [Environment Variables: A Comprehensive Guide](https://dev.to/pizofreude/environment-variables-a-comprehensive-guide-34dg)
- [Environment Variables in Windows/macOS/Linux](https://www3.ntu.edu.sg/home/ehchua/programming/howto/Environment_Variables.html)

### Glossari

Sistema operativo, Unix, Linux, windows, Extensiones comunes (.txt, .sh, .log, .conf, .tar.gz, .zip, .json, .csv), raíz (/), variables de entorno y/o sistema operativo, terminal, shell, rutas absolutas, rutas relativas, pwd, ls, ls -l, ls -a, cd, cd ~, cd .., mkdir, touch, cp, mv, rm, rm -r, chmod, chown, grep, find, |, ps, ps aux, kill, top, htop, ping, ssh, curl, wget, #!/bin/bash, history, man, tar, sudo, PATH, echo, cat, nano, vim, clear, exit, su, df, du, alias, env, scp, rsync, ln, cron, jobs, bg, fg.

## Exercici pràctic 1: Webminal (0.5 h)

### Context
[Webminal](https://www.webminal.org/) és un joc per practicar les ordres del terminal Linux. Amb aquest joc aprendràs les ordres més comuns.

### Objectius d’aprenentatge
- Practicar amb las ordres executades des del terminal Linux.

### Passos a seguir
1. Registra't al web de [Webminal](https://www.webminal.org/)
2. Entra al terminal
3. Completa les lliçons 1 a 11.

## Exercici pràctic 2: Fitxers i Directoris (0.5 h)

### Context
Amb aquest exercici practicaràs les ordres bàsiques per navegar eficientment per l’estructura del sistema i gestionar fitxers i directoris en entorns Unix/Linux. 

### Objectius d’aprenentatge
- Navegar i gestionar directoris i l’estructura del sistema.
- Manipular fitxers amb precisió.

### Passos a seguir
- 1. **Navegació**
    - Mostra tots els fitxers (inclosos els ocults) del vostre directori arrel (/ o ~).
    - Navega al directori on vols començar a desar els projectes de la ItAcademy.
- 2. **Creació d'estructura**
    - Crea una carpeta nova anomenada **itacademy-projects** al directori arrel.
    - Accedeix a la carpeta itacademy-proyectos.
    - Dins d'aquesta carpeta crea una subcarpeta anomenada sprint-1
    - Accedeix a la carpeta sprint-1.
    - Dins de sprint-1 crea una altra subcarpeta anomenada unitat-1
    - Accedeix a la carpeta unitat-1.
    - Crea un fitxer anomenat hoal-mundo.txt.
- 3. **Gestió d'errors**
    - Elimina el fitxer mal escrit (hoal-mundo.txt).
    - Crea un nou fitxer anomenat hola-mundo.txt.
    - Verifica el contingut del directori actual
    - Retorna al directori arrel sense usar la ruta completa.
    - Verifica el contingut del directori arrel

## Exercici pràctic 3:  Ordres Avançades

### Context
En aquest taller aprendràs a utilitzar ordres avançades del terminal per gestionar permisos de fitxers, directoris en entorns Unix/Linux.

### Objectius
- Entendre i modificar permisos 

### Passos a seguir

1. **Preparació inicial**
    - Dins de sprint-1 crea una nou directori un directori nou anomenat projecte-secret.
    - Dins de projecte-secret, crea un fitxer anomenat clau.txt amb el contingut: "Això és una clau secreta!" (Recorda que el text l'has d'inserir al document mitjançant l'ús de la terminal)

2. **Verificació de permisos actuals**
    - Executa ls -l ~/projecte-secret i observa els permisos del fitxer clau.txt (ex:   -rw-r--r--).

3. **Modificació de permisos**
    - Canvia els permisos de clau.txt perquè només el propietari pugui llegir-lo i escriure’l

4. **Simulació d’accés denegat**
    - Obre una nova terminal o canvia d’usuari (opcional amb su).
    - Intenta llegir el fitxer amb. (Resultat esperat: Permission denied)

5. **Gestió de permisos per a directoris**
    - Canvia els permisos del directori projecte-secret perquè només el propietari hi pugui accedir:
    - Verifica que altres usuaris no puguin veure el contingut del directori.

### Autoevaluació
- [ ] He navegat entre directoris.  
- [ ] He creat directoris i fitxers. 
- [ ] He buscat fitxers i directoris.
- [ ] He renombrat fitxers o directoris.
- [ ] He eliminat fitxers o directoris.
- [ ] He corregit errors comuns (ex: fitxers mal escriptes). 
- [ ] He entès els permisos bàsics (r, w, x).
- [ ] He canviat permisos de fitxers/directoris.
- [ ] Puc explicar què fa cada comanda utilitzada en l’exercici.

## Lliuraments

- Els apunts propis digitals del contingut treballat, amb screenshots dels resultats obtinguts als exercicis
- Entrega a la plataforma el llistat de punts dels exercicis amb les ordres que has fet servir a cada pas.

## Autoevaluació dels Coneixements

Respon **aquestes preguntes** als teus apunts per fixar coneixements i identificar dubtes:  

- Sé diferenciar entre unix i windows?
- Per què serveix el terminal en el desenvolupament de programari?
- Quina diferència hi ha entre rutes absolutes i relatives?
- Quines limitacions té el terminal davant d'una interfície gràfica (GUI)?