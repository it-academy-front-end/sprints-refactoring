```markdown
# Qüestionari de Branques i Treball Col·laboratiu amb Git

## Preguntes d'una única resposta (10)

### 1. **Cas pràctic**: Segons Git Flow, quin comandament s'utilitza per iniciar una nova funcionalitat?
- [ ] a) `git start feature/login`  
- [x] b) `git flow feature start login`  
- [ ] c) `git create feature/login`  
- [ ] d) `git branch feature/login`  

---

### 2. Quin és l'objectiu principal d'una branca `release` en Git Flow?
- [ ] a) Desenvolupar funcionalitats noves  
- [x] b) Preparar una versió per producció (tests finals, correccions menors)  
- [ ] c) Corregir errors urgents en producció  
- [ ] d) Documentar el projecte  

---

### 3. **Cas pràctic**: Has fet un fork d'un repositori i vols sincronitzar-lo amb l'original. Quin comandament executaries?
- [ ] a) `git sync upstream main`  
- [x] b) `git fetch upstream && git merge upstream/main`  
- [ ] c) `git pull origin main`  
- [ ] d) `git update --remote`  

---

### 4. Què representa una *Pull Request* (PR)?
- [ ] a) Una petició per eliminar una branca  
- [x] b) Una sol·licitud per fusionar canvis d'una branca a una altra  
- [ ] c) Un informe d'errors  
- [ ] d) Una actualització automàtica del repositori  

---

### 5. **Cas pràctic**: Vols assignar una tasca a un col·lega i fer-ne seguiment. Quina eina de GitHub utilitzaries?
- [ ] a) Projects  
- [ ] b) Milestones  
- [x] c) Issues  
- [ ] d) Wiki  

---

### 6. Quina branca actua com a font de veritat única (*single source of truth*) en un entorn col·laboratiu?
- [ ] a) `develop`  
- [x] b) `main` o `master`  
- [ ] c) `feature/login`  
- [ ] d) `hotfix`  

---

### 7. **Cas pràctic**: Un col·lega ha aprovat la teva PR a GitHub. Quin pas cal seguir?
- [ ] a) Fer `git revert`  
- [x] b) Fer *merge* des de la interfície de GitHub  
- [ ] c) Eliminar la branca automàticament  
- [ ] d) Tornar a enviar els canvis amb `git push`  

---

### 8. Què és un *Milestone* en GitHub?
- [x] a) Un objectiu amb data límit per agrupar tasques o issues  
- [ ] b) Una branca temporal per a experiments  
- [ ] c) Una etiqueta per marcar versions  
- [ ] d) Un informe d'estadístiques del projecte  

---

### 9. **Cas pràctic**: Has de corregir un error crític en producció. Segons Git Flow, quina branca has de crear?
- [ ] a) `feature/hotfix`  
- [x] b) `hotfix/error-login`  
- [ ] c) `release/error`  
- [ ] d) `patch/error`  

---

### 10. Quina ordre mostra les branques fusionades a la branca actual?
- [ ] a) `git branch --merged`  
- [x] b) `git branch --merged`  
- [ ] c) `git log --branches`  
- [ ] d) `git show-branch`  

---

## Preguntes de respostes múltiples (10)

### 1. **Cas pràctic**: Quins elements són clau en Git Flow? (Tria 3)
- [x] a) Branca `develop`  
- [x] b) Branca `hotfix`  
- [ ] c) Branca `experimental`  
- [x] d) Branca `release`  

---

### 2. Quines accions es poden realitzar amb un *fork*? (Tria 2)
- [x] a) Modificar un repositori sense afectar l'original  
- [ ] b) Eliminar l'historial de commits  
- [x] c) Enviar canvis mitjançant PR a l'original  
- [ ] d) Fusionar automàticament branques remotes  

---

### 3. **Cas pràctic**: Quins passos són necessaris per contribuir a un projecte via fork? (Tria 3)
- [x] a) Fer un fork del repositori original  
- [x] b) Clonar el teu fork localment  
- [ ] c) Crear una branca directament a l'original  
- [x] d) Enviar una PR després de fer canvis  

---

### 4. Quins avantatges tenen les *feature branches*? (Tria 2)
- [x] a) Aïllen canvis per a funcionalitats específiques  
- [ ] b) Redueixen el nombre de commits  
- [x] c) Faciliten la revisió de codi  
- [ ] d) Eliminen la necessitat de fer PR  

---

### 5. **Cas pràctic**: Quines accions es poden fer amb *GitHub Projects*? (Tria 2)
- [x] a) Organitzar tasques en columnes (To-Do, In Progress, Done)  
- [ ] b) Executar tests automàtics  
- [x] c) Visualitzar l'estat del projecte amb targetes  
- [ ] d) Configurar servidors de producció  

---

### 6. Quins són els estats possibles d'un *Issue*? (Tria 2)
- [x] a) Open  
- [ ] b) Merged  
- [x] c) Closed  
- [ ] d) Staged  

---

### 7. **Cas pràctic**: Quines eines ajuden a gestionar conflictes en una PR? (Tria 2)
- [x] a) Resolució de conflictes des de la interfície web de GitHub  
- [ ] b) `git cancel`  
- [x] c) `git merge --abort`  
- [ ] d) `git ignore`  

---

### 8. Quins tipus de branques existeixen en Git Flow? (Tria 3)
- [x] a) `feature`  
- [x] b) `release`  
- [ ] c) `patch`  
- [x] d) `hotfix`  

---

### 9. **Cas pràctic**: Què pots fer amb els *Milestones*? (Tria 2)
- [x] a) Associar-los a issues per prioritzar-los  
- [ ] b) Crear branques automàtiques  
- [x] c) Visualitzar el progrés amb un diagrama de Gantt  
- [ ] d) Executar scripts de desplegament  

---

### 10. Quines bones pràctiques s'apliquen al treball amb branques? (Tria 2)
- [x] a) Esborrar branques fusionades per mantenir neteja  
- [ ] b) Treballar directament a `main`  
- [x] c) Posar noms descriptius a les branques (ex: `fix/header-style`)  
- [ ] d) Fer commits amb missatges genèrics com "canvis"  

---

## Respostes correctes

### Preguntes d'una única resposta:
1. b  
2. b  
3. b  
4. b  
5. c  
6. b  
7. b  
8. a  
9. b  
10. b  

### Preguntes de respostes múltiples:
1. a, b, d  
2. a, c  
3. a, b, d  
4. a, c  
5. a, c  
6. a, c  
7. a, c  
8. a, b, d  
9. a, c  
10. a, c  
```