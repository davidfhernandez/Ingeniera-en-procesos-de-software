# Taller de Git: LearnGitBranching

**Herramienta:** [LearnGitBranching](https://learngitbranching.js.org/)

---

## 🛠️ Niveles Completados

### 1. Introducción (Niveles 1-4)
* **Git Commit:** Crea una captura del estado actual.
    ```bash
    git commit; git commit
    ```
    * ![commit](image/README/1770934118102.png)
* **Git Branch:** Crea una nueva línea de tiempo.
    ```bash
    git branch bugFix; git checkout bugFix
    ```
    * ![checkout](image/README/1770934367714.png)
* **Git Merge:** Une dos ramas en un nuevo commit.
    ```bash
    git checkout -b bugFix; git commit; git checkout main; git commit; git merge bugFix
    ```
    * ![merge](image/README/1770934711952.png)
* **Git Rebase:** Mueve el trabajo a una nueva base para un historial lineal.
    ```bash
    git checkout -b bugFix; git commit; git checkout main; git commit; git checkout bugFix; git rebase main
    ```
    * ![rebase](image/README/1770934979628.png)

---

### 2. Ramping Up (Niveles 1-4)
* **Detach HEAD:** Desconecta el puntero de la rama para apuntar a un commit.
    ```bash
    git checkout C4
    ```
    * ![HEAD](image/README/1770935224037.png)
* **Referencias Relativas (^):** Sube un nivel en el árbol.
    ```bash
    git checkout C4^
    ```
    * ![DETACH^](image/README/1770935449489.png)
* **Referencias Relativas (~):** Sube varios niveles de golpe.
    ```bash
    git branch -f main C6; git branch -f bugFix C0; git checkout C1
    ```
    * ![HEAD~](image/README/1770936346710.png)
* **Reset & Revert:** Borra cambios o crea un commit que deshace lo anterior.
    ```bash
    git reset HEAD~1; git checkout pushed; git revert pushed
    ```
    * ![REVERT-RESET](image/README/1770936642410.png)

---

### 3. Moving Work Around (Niveles 1-2)
* **Cherry-pick:** Copia commits específicos a la rama actual.
    * ![CHERRY-PICK](image/README/1770936916778.png)
* **Interactive Rebase:** Modifica, omite o reordena el historial.
    * ![INTERACTIVE REBASE](image/README/1770937196746.png)

---

### 4. Mixed Bag (Niveles 1-5)
* **Grabbing Just 1 Commit:** 
    * ![GRAB 1 COMMINT](image/README/1771003244525.png)

* **Juggling Commits:**
    * ![JUGGLING](image/README/1771003515684.png)

* **Juggling Commits #2:**
    * ![JUGGLING 2](image/README/1771003648206.png)

* **Git Tags:**
    * ![TAGS](image/README/1771003822284.png)

* **Git Describe:**
    * ![DESCRIBE](image/README/1771004112557.png)

---

### 5. Advanced Topics
* **9000 Rebase:**
    * ![9000 REBASE](image/README/1771004317523.png)

* **Multiple parents:**
    * ![MULTIPLE PARENTS](image/README/1771004651079.png)

* **Branch Spaghetti**
    * ![SPAGHETTI](image/README/1771004920877.png)