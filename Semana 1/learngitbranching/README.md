# Taller de Git: LearnGitBranching

**Herramienta:** [LearnGitBranching](https://learngitbranching.js.org/)

---

## 🛠️ Niveles Completados

### 1. Introducción (Niveles 1-4)
* **Git Commit:** Crea una captura del estado actual.
    ```bash
    git commit
    ```
    * ![commit](image/README/1770934118102.png)
* **Git Branch:** Crea una nueva línea de tiempo.
    ```bash
    git checkout -b bugFix
    ```
    * ![checkout](image/README/1770934367714.png)
* **Git Merge:** Une dos ramas en un nuevo commit.
    ```bash
    git merge bugFix
    ```
    * ![merge](image/README/1770934711952.png)
* **Git Rebase:** Mueve el trabajo a una nueva base para un historial lineal.
    ```bash
    git rebase main
    ```
    * ![rebase](image/README/1770934979628.png)

---

### 2. Ramping Up (Niveles 1-4)
* **Detach HEAD:** Desconecta el puntero de la rama para apuntar a un commit.
    * ![HEAD](image/README/1770935224037.png)
* **Referencias Relativas (^):** Sube un nivel en el árbol.
    * ![DETACH^](image/README/1770935449489.png)
* **Referencias Relativas (~):** Sube varios niveles de golpe.
    * `git checkout HEAD~3`
    * ![HEAD~](image/README/1770936346710.png)
* **Reset & Revert:** Borra cambios o crea un commit que deshace lo anterior.
    * `git reset HEAD~1` / `git revert HEAD`
    * ![REVERT-RESET](image/README/1770936642410.png)

---

### 3. Moving Work Around (Niveles 1-2)
* **Cherry-pick:** Copia commits específicos a la rama actual.
    * `git cherry-pick C2 C4`
    * ![CHERRY-PICK](image/README/1770936916778.png)
* **Interactive Rebase:** Modifica, omite o reordena el historial.
    * `git rebase -i HEAD~4`
    * ![INTERACTIVE REBASE](image/README/1770937196746.png)

---

### 4. Mixed Bag (Niveles 1-5)
* **Grabbing Just 1 Commit:** 
    * `git cherry-pick C4`
    * ![GRAB 1 COMMINT](image/README/1771003244525.png)

* **Juggling Commits:**
    * `git rebase -i HEAD~2`
    * ![JUGGLING](image/README/1771003515684.png)

* **Juggling Commits #2:**
    * `git rebase -i HEAD~2`
    * ![JUGGLING 2](image/README/1771003648206.png)

* **Git Tags:**
    * `git tag v1 C1`
    * ![TAGS](image/README/1771003822284.png)

* **Git Describe:**
    * `git describe main`
    * ![DESCRIBE](image/README/1771004112557.png)

---

### 5. Advanced Topics
* **9000 Rebase:**
    * `git rebase main bugFix`
    * ![9000 REBASE](image/README/1771004317523.png)

* **Multiple parents:**
    * `git checkout HEAD~^2`
    * ![MULTIPLE PARENTS](image/README/1771004651079.png)

* **Branch Spaghetti**
    * `git checkout one; git rebase main; git merge three`
    * ![SPAGHETTI](image/README/1771004920877.png)