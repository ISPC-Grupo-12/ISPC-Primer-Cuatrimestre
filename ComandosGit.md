# Comandos de Git
- **git pull**: Se utiliza para fusionar los cambios del repositorio remoto con el repositorio local. Combina los comandos `git fetch` y `git merge`, primero descarga los cambios y luego los integra en la rama actual.
    ```bash
    git pull origin
    ```
- **git pull --no-commit <remote>**: Obtiene los cambios del repositorio remoto pero no crea una nueva confirmación automáticamente.
    ```bash
    git pull --no-commit origin
    ```
- **git init**: Crea un nuevo repositorio Git o reinicia uno existente en el directorio actual.
    ```bash
    git init
    ```
- **git clone <copied_URL>**: Clona un repositorio remoto en tu máquina local, incluyendo todo el historial y versiones.
    ```bash
    git clone <copied_URL>
    ```
- **git status**: Muestra el estado actual del repositorio, incluyendo archivos modificados, no rastreados y preparados para confirmar.
    ```bash
    git status
    ```
- **git add <file>**: Añade archivos al área de preparación (staging area), indicando que están listos para ser confirmados.
    ```bash
    git add <file>
    ```
- **git commit -m "mensaje"**: Guarda los cambios preparados en el repositorio local con un mensaje descriptivo.
    ```bash
    git commit -m "mensaje"
    ```
- **git remote add <nombre> <url>**: Conecta tu repositorio local con un repositorio remoto, permitiendo sincronizar cambios entre ambos.
    ```bash
    git remote add <nombre> <url>
    ```
- **git push <remote> <branch>**: Sube los commits confirmados localmente al repositorio remoto en la rama especificada.
    ```bash
    git push origin main
    ```
- **git fetch [<remote>] [<branch>]**: Descarga los cambios del repositorio remoto sin fusionarlos automáticamente. Permite revisar los cambios antes de integrarlos.
    ```bash
    git fetch origin
    git fetch origin main
    ```
- **git branch**: Lista, crea o elimina ramas en el repositorio.
    ```bash
    git branch
    ```
- **git checkout -b <nombre-rama>**: Crea y cambia a una nueva rama.
    ```bash
    git checkout -b <nombre-rama>
    ```
- **git checkout <nombre-rama>**: Cambia a una rama existente.
    ```bash
    git checkout <nombre-rama>
    ```
- **git checkout -- <file>**: Descarta los cambios en un archivo y lo restaura a su última versión confirmada.
    ```bash
    git checkout -- <file>
    ```
- **git merge <rama>**: Fusiona la rama especificada con la rama actual, integrando los cambios.
    ```bash
    git merge <rama>
    ```
- **git rebase <rama>**: Integra los cambios de una rama en otra, reescribiendo el historial para mantenerlo lineal y limpio.
    ```bash
    git rebase <rama>
    ```
- **git log**: Muestra el historial de confirmaciones (commits) de la rama actual, incluyendo autor, fecha y mensaje.
    ```bash
    git log
    ```
- **git diff**: Muestra las diferencias entre archivos o ramas en distintos estados del repositorio.
    ```bash
    git diff
    ```
- **git reset [--soft|--mixed|--hard] <commit>**: Restablece el HEAD actual a un commit anterior, con diferentes niveles de preservación de cambios.
    ```bash
    git reset --soft <commit>
    git reset --mixed <commit>
    git reset --hard <commit>
    ```
- **git branch -D <nombre-rama>**: Elimina una rama de forma definitiva.
    ```bash
    git branch -D <nombre-rama>
    ```
- **git merge <rama-con-cambios> [rama-destino]**: Fusiona los cambios de una rama en otra. Si estás en la rama de destino, solo especifica la rama con cambios; si no, indica ambas ramas.
    ```bash
    git merge <rama-con-cambios>
    git merge <rama-con-cambios> <rama-destino>
    ```