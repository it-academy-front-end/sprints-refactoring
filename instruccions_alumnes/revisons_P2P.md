# Guia per al Code Review i el Feedback entre Estudiants

## Introducció

Aquesta guia té com a objectiu proporcionar un procés estructurat i efectiu per fer Code Review i donar Feedback entre companys/es de classe (parelles).

**Per què és important?**
- Aprenentatge actiu: Descobreixes noves solucions i bones pràctiques.
- Qualitat del codi: Detectes errors abans i millores la mantenibilitat.
- Habilitat professional: El Code Review és essencial en entorns laborals. 

## Com Realitzar un Code Review?

### 1. Preparació

1. **Descarrega i Prova:** Descarrega el projecte de la companya i prova'l al teu entorn local.
   
2. **Creació d’Issue:** Crea una **issue** al repositori de la propietària del projecte amb el títol:  
- `Code Review Sprint [Número] - [Nom-revisa]`. Això facilita l'organització i el seguiment del Feedback.

### 2. Mètodes de Revisió

1. **Revisió Asíncrona (GitHub Issues)**
- Segueix els **criteris tècnics de revisió** detallats més avall.
- Documenta els teus resultats a la issue utilitzant el **format de documentació d’un Code Review** detallat més avall.
 
2. **Revisió en Parelles (Síncrona/Presencial)**
- La revisió es fa de manera síncrona, presencialment i per parelles.
- L’**autora** explica: l’objectiu de la solució, les decisions tècniques preses, els punts clau a considerar.
- La **revisora**: llegeix el codi amb deteniment, identifica possibles millores, planteja dubtes i propostes de canvi, i documenta els seus resultats a la issue utilitzant el **format de documentació d’un Code Review** detallat més avall.

## Criteris Tècnics a Observar en un Code Review
1. **Compliment de l’Enunciat**
- Verificar que la solució compleix tots els requisits especificats.
- Assegurar que les funcionalitats obligatòries estan implementades correctament.
- Comprovar que els casos especials i possibles errors es gestionen adequadament.
- Revisar que el codi està escrit en anglès: noms de classes, mètodes, variables i comentaris.

2. **Qualitat del Codi**
    **Format i Convencions**
    - Mantenir una indentació coherent segons els estàndards del llenguatge.
    - Utilitzar correctament espais i salts de línia en estructures de control.
    - Escriure comentaris breus i clars només quan siguin necessaris.
    - Mantenir una organització consistent a tots els fitxers del projecte.

    **Nomenclatura**
    - Fer servir noms descriptius per a classes, mètodes i variables.
    - Evitar abreviatures poc clares o noms genèrics.
    - Seguir les convencions de nomenclatura establertes en el projecte.
    - Utilitzar noms que indiquin la funció o responsabilitat de cada element.

    **Mètodes Curts amb Única Responsabilitat**
    - Verificar que els mètodes i classes siguin concisos i no facin massa coses.
    - Aplicar el principi de responsabilitat única per millorar llegibilitat i manteniment.
    - Considerar dividir mètodes complexos en altres més específics quan calgui.

    **Control de la Complexitat**
    - Reduir condicionals i bucles imbricats innecessaris.
    - Utilitzar estratègies com `early returns` o `fail fast` per simplificar la lògica.
    - Evitar l'ús excessiu de variables temporals o `flags` que compliquin el flux.

    **Estructures de Dades**
    - Escollir les col·leccions adequades per a cada tipus de dada.
    - Evitar iteracions o modificacions ineficients de llistes i conjunts.
    - Considerar construccions del llenguatge que puguin simplificar la lògica.

3. **Robustesa i Gestió d'Errors**
- Garantir que les excepcions es gestionen correctament.
- Evitar captures massa genèriques, prioritzant la gestió específica d'errors.
- Minimitzar l’ús de valors nuls, utilitzant alternatives que millorin el control.
- Assegurar que no hi ha errors que quedin sense tractament o notificació.

4. **Estructura del Projecte**
- Verificar que les classes estan organitzades coherentment en paquets.
- Comprovar que els fitxers tenen noms apropiats que reflecteixin el seu propòsit.
- Assegurar que les dependències estan ben gestionades i sense imports innecessaris.

    **Fitxer `.gitignore`**
    - Incloure fitxers que no han d’estar al repositori (ex: de compilació).
    - Revisar que no s’exposen secrets ni dades sensibles.

    **Fitxer `README.md`** confirmar que inclou:
    - Descripció i propòsit del projecte.
    - Tecnologies utilitzades.
    - Instruccions clares per a la configuració i execució.
    - Captures de pantalla o demos quan sigui rellevant.

## Com Donar Feedback Efectiu?
Un bon Code Review no només assenyala errors, sinó que inspira millores i celebra els encerts.  
Preparades per convertir-vos en expertes en Code Review? A practicar! 💻🔍

1. **Bones Pràctiques d’un Code Review**
- Mantingues una actitud constructiva: es revisa el codi, no la persona.
- Anota dubtes i suggeriments de forma clara i respectuosa.
- L’objectiu és que la revisió sigui efectiva i promogui una millora contínua.

2. **Estructura el teu Feedback en 3 parts:**
- **Fortaleses**: "El sistema de rutes està molt ben organitzat."
- **Àrees de millora**: "El component Button podria reutilitzar-se en altres vistes."
- **Suggeriments concrets**: "Utilitza `Array.map()` per simplificar aquest loop."

### Format de documentació d’un Code Review
Pots fer servir aquesta estructura per documentar el Code Review realitzat:

    ```html
    ## Code Review Sprint 3 - Manuela Grajales Duque

    ### 🔧 **Funcionalitat**  
    - ✅ Tot el CRUD funciona segons l’esperat.  
    - ❌ El botó "Desar" no mostra Feedback a l’usuari quan falla l’API.  

    ### 🧹 **Clean Code**  
    - 👍 Els noms de variables són molt clars (`userList`, `handleSubmit`).  
    - 👀 Oportunitat: Elimina el codi comentat a `utils/helpers.js`.  

    ### 📚 **README**  
    - ✨ Molt complet, però falta afegir com executar els tests.  

    ### 🤝 **Feedback General**  
    Excel·lent feina! El codi és net i funcional. Suggereixo afegir un spinner durant les crides a l’API per millorar la UX.   
    ```
