# Qüestionari de GitHub Actions, GitHub Pages i Git Hooks

## Preguntes d'una única resposta (10)

### 1. **Cas pràctic**: Vols executar tests automàticament en fer `git push` a la branca `main`. Quina eina de GitHub utilitzaries?
- [ ] a) Git Hooks  
- [x] b) GitHub Actions  
- [ ] c) GitHub Pages  
- [ ] d) Git Tags  

---

### 2. Quin fitxer defineix un workflow de GitHub Actions?
- [ ] a) `actions.yml`  
- [x] b) `.github/workflows/main.yml`  
- [ ] c) `github-actions.yaml`  
- [ ] d) `workflow.config`  

---

### 3. **Cas pràctic**: Has creat un hook `pre-commit` però no s'executa. Quin és el problema més probable?
- [x] a) El fitxer no té permisos d'execució  
- [ ] b) Falta instal·lar GitHub CLI  
- [ ] c) S'ha d'activar a la configuració de GitHub  
- [ ] d) Requereix una branca `hooks`  

---

### 4. Què desplega GitHub Pages per defecte?
- [ ] a) Una API REST  
- [x] b) Contingut estàtic (HTML/CSS/JS)  
- [ ] c) Bases de dades en temps real  
- [ ] d) Aplicacions amb backend PHP  

---

### 5. **Cas pràctic**: Vols evitar commits amb missatges buits. Quin Git Hook utilitzaries?
- [x] a) `commit-msg`  
- [ ] b) `pre-push`  
- [ ] c) `post-merge`  
- [ ] d) `pre-rebase`  

---

### 6. Quin event de GitHub Actions s'activa quan es crea una *pull request*?
- [ ] a) `on: push`  
- [x] b) `on: pull_request`  
- [ ] c) `on: pr_created`  
- [ ] d) `on: request`  

---

### 7. **Cas pràctic**: Vols desplegar el teu lloc web a GitHub Pages des d'una branca `docs`. Quin pas és necessari?
- [ ] a) Configurar un servidor Node.js  
- [x] b) Habilitar GitHub Pages a les opcions del repositori i seleccionar la branca  
- [ ] c) Afegir un fitxer `deploy.py`  
- [ ] d) Executar manualment `git push origin docs`  

---

### 8. On s'emmagatzemen els Git Hooks per defecte en un repositori local?
- [ ] a) `.git/hooks/`  
- [x] b) `.git/hooks/`  
- [ ] c) `hooks/`  
- [ ] d) `.github/hooks/`  

---

### 9. **Cas pràctic**: Quin comandament instala un hook `pre-commit` des d'una plantilla?
- [ ] a) `git hook install pre-commit`  
- [x] b) `git init` (si la plantilla està a `.githooks`)  
- [ ] c) `git config --global hook.pre-commit`  
- [ ] d) `npm install husky`  

---

### 10. Quina acció de GitHub es fa servir habitualment per desplegar a GitHub Pages?
- [ ] a) `actions/checkout`  
- [ ] b) `actions/setup-node`  
- [x] c) `peaceiris/actions-gh-pages`  
- [ ] d) `docker/build-push-action`  

---

## Preguntes de respostes múltiples (10)

### 1. **Cas pràctic**: Quines parts són obligatòries en un workflow de GitHub Actions? (Tria 2)
- [x] a) `jobs`  
- [x] b) `on` (events que activen el workflow)  
- [ ] c) `environment`  
- [ ] d) `tags`  

---

### 2. Quins tipus de Git Hooks existeixen? (Tria 2)
- [x] a) Client-side (ex: `pre-commit`)  
- [ ] b) Cloud-side  
- [x] c) Server-side (ex: `pre-receive`)  
- [ ] d) Hybrid-side  

---

### 3. **Cas pràctic**: Quines accions pots automatitzar amb GitHub Actions? (Tria 3)
- [x] a) Executar tests unitaris  
- [x] b) Desplegar a un servidor  
- [ ] c) Crear branques automàticament  
- [x] d) Generar documentació  

---

### 4. Quins formats són compatibles amb GitHub Pages? (Tria 2)
- [x] a) HTML/CSS/JS estàtic  
- [x] b) Jekyll (Markdown)  
- [ ] c) Django  
- [ ] d) WordPress  

---

### 5. **Cas pràctic**: Quins passos calen per usar un hook `pre-push`? (Tria 2)
- [x] a) Crear un fitxer a `.git/hooks/pre-push`  
- [ ] b) Configurar-lo a GitHub.com  
- [x] c) Assegurar-se que té permisos d'execució  
- [ ] d) Afegir-lo al `.gitignore`  

---

### 6. Quines eines s'integren amb GitHub Actions? (Tria 3)
- [x] a) Docker  
- [x] b) npm  
- [x] c) pytest  
- [ ] d) MySQL Server (instal·lació directa)  

---

### 7. **Cas pràctic**: Quines opcions tens si un workflow de GitHub Actions falla? (Tria 2)
- [x] a) Revisar els logs de l'execució  
- [ ] b) Reiniciar el servidor de GitHub  
- [x] c) Corregir el codi i fer push de nous canvis  
- [ ] d) Eliminar el repositori  

---

### 8. Quins hooks són útils per a control de qualitat de codi? (Tria 2)
- [x] a) `pre-commit` (executar linters)  
- [ ] b) `post-checkout`  
- [x] c) `pre-push` (executar tests)  
- [ ] d) `post-rewrite`  

---

### 9. **Cas pràctic**: Quins elements defineixen un *job* en GitHub Actions? (Tria 3)
- [x] a) `runs-on` (sistema operatiu)  
- [x] b) `steps`  
- [ ] c) `branch`  
- [x] d) `env` (variables d'entorn)  

---

### 10. Quines funcionalitats ofereix GitHub Pages? (Tria 2)
- [x] a) Hosting gratuït per a llocs estàtics  
- [ ] b) Execució de codi PHP  
- [x] c) Domini personalitzat (ex: `www.elmeudomini.cat`)  
- [ ] d) Bases de dades SQL integrades  

---

## Respostes correctes

### Preguntes d'una única resposta:
1. b  
2. b  
3. a  
4. b  
5. a  
6. b  
7. b  
8. b  
9. b  
10. c  

### Preguntes de respostes múltiples:
1. a, b  
2. a, c  
3. a, b, d  
4. a, b  
5. a, c  
6. a, b, c  
7. a, c  
8. a, c  
9. a, b, d  
10. a, c  
