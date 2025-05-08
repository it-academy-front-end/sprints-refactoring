## Introducció  

En aquesta unitat, treballaràs els fonaments de les aplicacions web per comprendre com es construeixen, quins elements les formen i com funcionen.  
Al final de l'unitat seràs capaç de manejar el vocabulari i els conceptes de les aplicacions web.  
La durada estimada d'aquest mòdul és de **3 hores**.  

## Objectius d'aprenentatge  

1. Explicar el funcionament bàsic de l'arquitectura client-servidor.  
2. Diferenciar entre *front-end*, *back-end* i *full-stack*.  
3. Reconèixer les característiques d'aplicacions estàtiques, dinàmiques o SPA.  
4. Entendre la importància de l'accessibilitat (WCAG) i el SEO.  
5. Identificar termes com API, DOM o CORS en contextos tècnics.  

## Metodologia  
El mòdul consta de tres apartats diferenciats: teòric, pràctic i qüestionari d'autoconeixement.  

- Per a la teoria, hauràs d'**el·laborar** uns apunts i lliurar la **URL** al final d'aquesta unitat.  

> **Important**  
> Pots crear el teu espai personal a Notion, Obsidian o GitBook per desar els conceptes, exemples i trucs. Pots organitzar-ho per temes (HTML, JS, Git...) i així tindràs el teu propi manual tècnic a mà.  
> ✏ **Fes-ho ara**: obre una pàgina i comença amb el primer tema.  

- Per a la part pràctica, hauràs de crear un document escrit que incorporaràs als apunts.  
- El qüestionari el resoldràs a la plataforma **Moodle**.  

## Fonaments teòrics (1,5 h)  
Per construir la teva base teòrica, hauràs d'investigar **una sèrie de temes** i elaborar un glossari de termes que has de conèixer.  

### Temes d'investigació  

- Arquitectura client-servidor: funcionament bàsic i components (navegador, servidor, API).  
- Diferència entre *front-end*, *back-end* i *full-stack*.  
- Protocol HTTP/HTTPS: peticions, respostes, codis d'estat.  
- Tipus d'aplicacions web: estàtiques vs dinàmiques, SPAs (*Single-Page Applications*), PWAs (*Progressive Web Apps*).  
- Rol dels navegadors web: motor de renderització, compatibilitat amb estàndards (HTML/CSS/JS).  
- Conceptes bàsics de responsivitat, accessibilitat (WCAG) i SEO.  
- Terminologia comuna: DOM, API, CMS, *framework* vs llibreria.  
- Seguretat bàsica: HTTPS, *Cross-Site Scripting* (XSS), *Cross-Origin Resource Sharing* (CORS).  

### Recursos  

- [Com funciona la web?](https://developer.mozilla.org/es/docs/Learn_web_development/Getting_started/Web_standards/How_the_web_works)  
- [Com funciona Internet?](https://developer.mozilla.org/es/docs/Learn_web_development/Howto/Web_mechanics/How_does_the_Internet_work)  
- [Quina és la diferència entre *front end* i *back end* en el desenvolupament d'aplicacions?](https://aws.amazon.com/es/compare/the-difference-between-frontend-and-backend/#:~:text=El%20front%20end%20es%20aquello,permiten%20que%20la%20aplicaci%C3%B3n%20funcione)  
- [Generalitats del protocol HTTP](https://developer.mozilla.org/es/docs/Web/HTTP/Guides/Overview)  
- [Renderització a la web](https://web.dev/articles/rendering-on-the-web?hl=es-419)  
- [Introducció als *frameworks* de client](https://developer.mozilla.org/en-US/docs/Learn_web_development/Core/Frameworks_libraries/Introduction)  
- [Què és una aplicació web progressiva?](https://developer.mozilla.org/en-US/docs/Web/Progressive_web_apps/Guides/What_is_a_progressive_web_app)  

### Glossari  

Internet, *World Wide Web*, HTTP/HTTPS, Cau, *Proxy*, CORS, CSRF, *SQL Injection*, XSS, SSH, API REST, GraphQL, *WebSockets*, JWT, OAuth, DNS, URL/URI, *Cookie*, SEO, DevOps, Servidor de desenvolupament, Servidor de preproducció (*staging*), Servidor de producció, CI/CD, GitHub Actions, Jenkins, Nginx, Apache, Docker, Kubernetes, AWS, Google Cloud, Azure, Vercel, Netlify, SPA, PWA, SSR/Isomòrfiques, Aplicacions en temps real, Microserveis, *Serverless*, IA generativa, Models d'IA, Assistents virtuals, Aplicacions híbrides, Git/GitHub/GitLab/BitBucket, A11Y, ARIA, Disseny responsiu (*Responsive Design*), *Mobile First*, *Media Queries*, HTML5, CSS3, DOM, SASS, JavaScript, ECMAScript, TypeScript, *Web Components*, *Web Assembly*, *Frontend*, *Backend*, Sistema de gestió de bases de dades, Base de dades relacional, NoSQL, SQL, JOINs, Índexs, ORMs, Test unitari, Test e2e, Microserveis, Arquitectura de *software*, Rendiment web (*Web Performance*), *Lazy Loading*, CDN, Lighthouse, UX/UI, Àgil (*Agile*), Scrum, Terminal/CLI.  

## Exercici pràctic (1 h)  

Aquí posaràs a prova els teus coneixements **fent una anàlisi** de 6 aplicacions web diferents de dues categories: webs comercials i aplicacions.  

Per a cada aplicació web, hauràs de:  
1. Identificar-ne la tipologia.  
2. Justificar-ho amb evidències tècniques.  
3. Documentar-ne les característiques principals.  

### Recursos  

1. **Aplicacions a analitzar:**  

| Grup | Exemples |  
|------|----------|  
| **Grup 1: Webs comercials** | - Amazon.com<br>- Blog personal WordPress<br>- Portafoli estàtic |  
| **Grup 2: Aplicacions web** | - Airbnb<br>- Twitter<br>- Pàgina de documentació de MDN |  

2. **Exemple d'estructura de l'anàlisi**  

Per a cada aplicació, completa la següent taula:  

**Nom de l'aplicació**  

| Criteri | Descripció |  
|---------|------------|  
| Tipologia | Estàtica/Dinàmica/SPA |  
| URL | [URL de l'aplicació](#) |  
| Evidències tècniques | - Llista de característiques observades |  
| Comportament de navegació | Descripció del comportament |  
| Temps de càrrega | Anàlisi amb DevTools |  
| Interacció amb el servidor | Patrons observats |  

### Lliuraments  

- Els apunts digitals propis del contingut treballat.  
- L'anàlisi de les 6 aplicacions web als teus apunts digitals.  

## Autoevaluació dels coneixements (0,5 h)  

Respon **aquestes preguntes** als teus apunts per fixar coneixements i identificar dubtes:  

1. Per què és important l'accessibilitat web?  
2. Quins components formen part de l'arquitectura d'un navegador web?  
3. Quines són les diferències entre *front-end* i *back-end*?  
4. Quins elements es poden controlar amb HTTP?  
5. Quins tipus d'emmagatzematge local suporta un navegador modern?  
