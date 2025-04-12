# Exercici Pràctic: Anàlisi de Tipologies d'Aplicacions Web
## Objectiu
Analitzar diferents aplicacions web i classificar-les segons la seva tipologia (estàtica, dinàmica o SPA), justificant tècnicament la classificació.

## Metodologia
1. Analitzar 6 aplicacions web diferents
2. Per a cada aplicació:
    - Identificar la seva tipologia
    - Justificar amb evidències tècniques
    - Documentar característiques principals
## Aplicacions a Analitzar

Grup 1: **Webs Comercials**
    - Amazon.com
    - Blog personal WordPress
    - Portafoli estàtic

Grup 2: **Aplicacions Web**
    - Airbnb
    - Twitter
    - Pàgina de documentació de MDN

## Estructura de l'Anàlisi

Per a cada aplicació, hauràs de completar la següent taula:

### [Nom de l'Aplicació]

| Criteri | Descripció |
|----------|-------------|
| Tipologia | [Estàtica/Dinàmica/SPA] |
| URL | [URL de l'aplicació] |
| Evidències tècniques | - Llista de característiques observades |
| Comportament de navegació | Descripció del comportament |
| Temps de càrrega | Anàlisi amb DevTools |
| Interacció amb servidor | Patrons observats |

## Criteris d'Avaluació

1. Identificació de Tipologia (30%)
    - Correcta classificació de l'aplicació
    - Argumentació tècnica sòlida
2. Anàlisi Tècnic (40%)
    - Ús de DevTools per a l'anàlisi
    - Identificació de patrons de càrrega
    - Anàlisi de peticions al servidor
3. Documentació (30%)
    - Claredat en l'explicació
    - Exemples concrets
    - Ús correcte de terminologia tècnica

## Lliurament
Format

```markdown
# Anàlisi de Tipologies Web

## 1. [Nom Aplicació 1]
[Completar taula d'anàlisi]

## 2. [Nom Aplicació 2]
[Completar taula d'anàlisi]

[...]
## Conclusions
- Patrons observats
- Comparativa entre tipologies
- Casos d'ús ideals per a cada tipus

```
## Exemple d'Anàlisi

```markdown
## Gmail

| Criteri | Descripció |
|----------|-------------|
| Tipologia | SPA (Single Page Application) |
| URL | https://mail.google.com |
| Evidències tècniques | - No hi ha recàrregues completes de pàgina
                       - Ús intensiu de JavaScript
                       - Estat mantingut en client
                       - Peticions AJAX per a dades |
| Comportament de navegació | - La URL canvia sense recàrrega
                            - Transicions suaus
                            - Manteniment d'estat |
| Temps de càrrega | - Càrrega inicial més pesada
                    - Navegació posterior instantània |
| Interacció amb servidor | - API REST
                          - WebSocket per actualitzacions
                          - Càrrega sota demanda |
```


## Rúbrica d'Avaluació
|Criteris d'Assoliment| Notable (7-8)|Excel·lent (9-10)|
|---|---|---|
|Identificació|	Correcta classificació amb arguments bàsics|Classificació precisa amb arguments tècnics detallats|
|Anàlisi Tècnic|Ús bàsic de DevTools i anàlisi de patrons|Anàlisi profund amb múltiples eines i mètriques|
|Documentació|Documentació clara i estructurada|Documentació exhaustiva amb exemples i referències|

## Lliurament Final
- Document Markdown amb l'anàlisi
- Captures de pantalla rellevants
- Mètriques de rendiment
- Conclusions comparatives

