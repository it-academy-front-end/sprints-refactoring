## Introducció  

En aquesta unitat explorarem com crear pàgines web funcionals, accessibles i visualment atractives des de les bases. No es tracta només de fer que el codi "funcioni", sinó d’entendre per què certes decisions tècniques milloren l’experiència per a tothom, incloent-hi usuaris amb discapacitats visuals o motores.

Començarem estructurant el contingut amb HTML semàntic, aprendent a escollir etiquetes com <article> o <nav> perquè els lectors de pantalla entenguin la pàgina sense veure-la. Després, aprofundirem en CSS modern: des de graelles flexibles amb Grid i Flexbox fins a variables reutilitzables i unitats que s’adapten a qualsevol pantalla.

La responsivitat serà clau: veurem com ajustar dissenys per a mòbil i escriptori amb estratègies intel·ligents, i com les imatges adaptatives poden estalviar dades als usuaris. Però no només això: integrarem accessibilitat avançada des del primer dia, assegurant contrastos llegibles i navegació fluida per teclat.

La durada estimada d'aquest mòdul és de **12 hores**.  

### Objectius d'Aprenentatge

1. Estructurar contingut web utilitzant etiquetes semàntiques (<header>, <article>, etc.) per millorar l'accessibilitat i SEO.
2. Aplicar atributs bàsics d'accessibilitat (alt, aria-label) per a elements no textuals.
3. Crear layouts complexes i responsius amb CSS Grid i Flexbox.
4. Utilitzar variables CSS i funcions com clamp() per a dissenys fluidos i mantenibles.
5. Desenvolupar interfícies adaptables a diferents dispositius amb media queries.
6. Escollir estratègies de breakpoint efectives (mobile-first vs desktop-first) per a escalar dissenys.
7. Distingir entre CSS Reset i Normalize.css per a estils base coherents.
8. Utilitzar bones pràctiques per millorar rendiment eliminant codi CSS innecessari.

### Metodologia  
El mòdul consta de tres apartats diferenciats: teòric, pràctic i qüestionari d'autoconeixement.  

- Per a la teoria, hauràs d'**elaborar** uns apunts i lliurar la **URL** al final d'aquesta unitat.  
- Per a la part pràctica, treballaràs al Visual Studio Code. Els exercicis els pujaràs a la plataforma.
- El qüestionari el resoldràs a la plataforma.  

## Fonaments teòrics (1,5 h)  
Per construir la teva base teòrica, hauràs d'investigar **una sèrie de temes** i elaborar un glossari de termes que has de conèixer.  

### Temes d'investigació  
- Per què és important usar etiquetes com <header>, <nav> o <article> en lloc de <div>? Explica com ajuden als lectors de pantalla.
- Com crearies un menú horitzontal adaptable amb Flexbox que es convertira en vertical en mòbil? Inclou la propietat gap i explica per què és millor que posar marges manualment.
- Què és un CSS Reset i per què s’utilitza? Compara breument amb Normalize.css i indica quina opció triaries per a un projecte nou i per què.
- Quina diferència hi ha entre `max-width` i `min-width` en les media queries? Com faries el disseny d'un contenidor que ocupi el 90% de la pantalla en mòbil i 70% en escriptori usant rem.
- Indaga les diferències entre la maquetació Mobile-first i desktop-first
- Per què és clau l’atribut alt a les imatges? Proposa un exemple amb una imatge decorativa i una informativa, i com indicaries als lectors de pantalla que ignorin la primera.

**Bonus**
- Com pots estructurar un formulari complex utilitzant <section>, <fieldset> i aria-labelledby per a garantir que els lectors de pantalla identifiquin correctament grups de camps relacionats? Proposa un exemple amb roles ARIA i justifica l'elecció de cada etiqueta semàntica.
- Explica com CSS Grid amb `grid-template-areas` més l'ús de variables css per als espais (`--gap: clamp()`) pot millorar l'accessibilitat respecte a `floats`/`positioning` tradicional.
- Compara l'impacte d'utilitzar CSS Reset vs Normalize.css en l'accessibilitat. Com afecten als estils per defecte dels formularis i quines propietats CSS modernes (ex: accent-color) permetrien substituir hacks antics mantenint contrastos WCAG 2.1?"
- Defineix una estratègia per a imatges adaptatives amb <picture> i srcset que prioritzi l'"art direction" en mode retrat (mòbil) i inclogui atributs alt descriptius diferents per a cada context. Quin rol juguen els media queries dins de l'etiqueta <picture>?
- Com implementaries un sistema de temes clar/fosc amb variables CSS (prefers-color-scheme) que garanteixi contrastos adequats automàticament? Proposa un fragment amb calc() per ajustar luminositat i explica com :focus-visible millora la navegació per teclat."

### Recursos  
- [A Step-By-Step Process for Turning Designs Into Code](https://css-tricks.com/a-step-by-step-process-for-turning-designs-into-code/)
- [Semantic HTML5 Elements Explained](https://www.freecodecamp.org/news/semantic-html5-elements/)
- [Learn How To Make a Website](https://learnfromsteph.dev/)
- [What is Mobile First Design?](https://www.geeksforgeeks.org/mobile-first-design/)
- [CSS Grid Layout Guide](https://css-tricks.com/snippets/css/complete-guide-grid/)
- [CSS Flexbox Layout Guide](https://css-tricks.com/snippets/css/a-guide-to-flexbox/)
- [Modern CSS Solutions for Old CSS Problems](https://moderncss.dev/)
- [Container Query Units and Fluid Typography](https://moderncss.dev/container-query-units-and-fluid-typography/)
- [Accesibility on the web](https://developer.mozilla.org/en-US/docs/Learn_web_development/Core/Accessibility)
- [Resources on Accessibility - The A11Y Project](https://www.a11yproject.com/resources/)

## Exercici pràctic 1: Bad Religion (2 h)  

### Context

Reproduiràs el disseny del [póster Bad Religion d'Swissted](https://www.swissted.com/products/bad-religion-at-eagles-lodge-1990#&gid=1&pid=1). L’exercici se centra en:
- Estructura jeràrquica amb Grid
- Alineació precisa de textos amb Flexbox
- Responsivitat mínima (centrat en pantalles grans)

La url del repositori de l'exercici l'hauràs d'anexar als teus apunts. 

### Objectius d'aprenentatge
- Practicar CSS Grid per a layouts complexes.
- Dominar Flexbox per a alinear contingut dins de cel·les de la graella.
- Utilitzar unitats relatives (rem, %) per a mantenir proporcions.
- Aplicar accessibilitat bàsica amb etiquetes semàntiques.

### Passos a seguir
- Per començar, crea un repositori a GitHub amb el nom **"bad-religion-layout"**.
- Clona el repositori i crea dos fitxers: `index.html`i `style.css`. 
- Crea l'estructura bàsica de l'html (utilitza alguna dreçera de teclat de vscode)  i conecta'l amb la fulla de estils. Fes el primer commit (recorda seguir les convencions als commits).
- Continua amb la maquetació:
  1. Observa el póster i descompon-lo en blocs visuals (15 min):
  - Identifica com es distribueixen els elements (alineacions, jerarquia, espais).
  - Determina quines parts requereixen una graella fixa i quines poden ser flexibles.
  2. Configuració inicial (20 min)
  - Escull etiquetes semàntiques o genèriques segons el context per definir l'estructura de la pàgina.
  - Hauràs observat que l'estructura principal de la pàgina es un quadrat. Experimenta amb un contenidor principal, utilitzant una propietat CSS que permeti mantenir una relació d’aspecte quadrat.
  3. Experimenta amb Grid i Flexbox (60 min)
  - Per a la disposició global:
    - Prova diferents enfocaments amb CSS Grid (grid-template-rows/columns, gap).
    - Com pots alinear elements secundaris (data, localització) en oposats sense usar marges fixos?
  - Per a components interns:
    - Quina tècnica (Flexbox o subgrid) permet controlar millor l’espaiat entre línies de text?
  4. Tipografia adaptable (15 min)
  - Simula la font amb `sans-serif` i `text-transform` 
  - Ajusta mides de text amb `clamp()` per a escalat fluid. 
  5. Accessibilitat (10 min)
  - Afegeix `aria-label` al contenidor principal per descriure el póster.
  - Prova el contrast de color. Quin contrast mínim has de garantir entre el fons i el text?
  6. Exporta tu disseny a PDF i compara’l amb la imatge original usant eines com [PerfectPixel](https://www.welldonecode.com/perfectpixel/) per detectar desajustos.
  7. Valora el rendiment de la teva pàgina amb l'eina "Lighthouse" del navigador.

### Autoevaluació
- Quina diferència pràctica hi ha entre usar grid-template-areas i grid-column/grid-row per posicionar elements?
- Si el logo no s’alinea a la cantonada inferior dreta, quines propietats de Flexbox o Grid revisaries?
- Per què és important definir aspect-ratio: 1/1 en el contenidor principal?

## Exercici pràctic 2: Refactorització d'un formulari accesible (1,5 h)

### Context
Has rebut un formulari de registre existent amb múltiples problemes d'accessibilitat:  
- Etiquetes (`<label>`) absents o mal vinculades.  
- Grups de camps sense agrupar semànticament (ex: radio buttons per triar un pla de subscripció).  
- Errors de contrast de color i falta de feedback clar per a usuaris de lectors de pantalla.  

**Formulari original**:  
```html
<form>
  <div>
    <span>Nom complet</span>
    <input type="text" id="name">
  </div>
  
  <div>
    <input type="radio" name="plan"> Bàsic
    <input type="radio" name="plan"> Premium
  </div>

  <button>Envia</button>
</form>
```

### Objectius d'aprenentatge
1. Millorar l’estructura semàntica amb etiquetes HTML adequades.  
2. Aplicar atributs ARIA per a comunicar estats dinàmics.  
3. Verificar contrastos de color segons WCAG 2.1 (>4.5:1 per text).  
4. Assegurar la navegació per teclat i el focus visible.  

### Passos a seguir
Per començar, crea un repositori a GitHub amb el nom **"formulari-accesible"** i clona'l al teu entorn local.

1. **Anàlisi inicial (20 min)**  
- Identifica elements que violen principis d’accessibilitat:  
  - Camps sense etiqueta clara.  
  - Grups de opcions no agrupats semànticament.  
  - Colors amb contrast insuficient (ex: gris clar sobre blanc).  
2. **Refactorització HTML (40 min)**  
- Vincula cada camp del formulari amb la seva etiqueta mitjançant `<label for="id">`.  
- Agrupa els radio buttons amb `<fieldset>` i afegeix un `<legend>` descriptiu.  
- Prova a substituir `<div>` genèrics per etiquetes semàntiques com `<section>` si s’escau.  
3. **Millores visuals i d’interacció (30 min)**  
- Defineix estils de `:focus-visible` per a resaltar elements en navegar amb teclat.  
- Afegeix `aria-describedby` per a errors de validació (ex: "El camp email és obligatori").  
- Utilitza eines com [WebAIM Contrast Checker](https://webaim.org/resources/contrastchecker/) per ajustar colors.  
4. **Validació (20 min)**
- Utilitza l’eina [WAVE](https://wave.webaim.org/) per a detectar errors ocults i compara el teu resultat amb el formulari original.
- Navega el formulari **només amb teclat** (TAB + ENTER).  
- Prova-ho amb un lector de pantalla (ex: NVDA o VoiceOver).  
- Verifica que tots els camps es descriuen correctament.  

### Autoavaluació

1. Per què és important usar `<fieldset>` i `<legend>` en lloc de `<div>` per a grups de radio buttons?
2. Què faries per a indicar visualment i semànticament un camp amb error?
3. Com garantiries que un usuari d’aplicatiu de veu pugui enviar el formulari sense veure la pantalla?

## Lliuraments  

- Els apunts digitals propis del contingut treballat.  
- L'exercicis als apunts.

## Autoevaluació dels coneixements (0,5 h)  

Respon **aquestes preguntes** als teus apunts per fixar coneixements i identificar dubtes:  

- Sabries integrar HTML semàntic i atributs ARIA per a transformar un formulari no accessible en un que compleixi amb els estàndards WCAG 2.1?
- Coneixes les diferències entre `grid-template-areas` i `grid-column`/`grid-row`. Sabries gestionar l’adaptació a mòbil amb clamp() i media queries."
- Podries optimitzar un projecte existent amb CSS redundant i contrastos deficients, per equilibrar rendiment i accessibilitat? Com mediries l'eficiència i la accesibilitat?