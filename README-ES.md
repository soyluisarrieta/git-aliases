<div align="center">
  <h1>Alias para Git</h1>
  <p>🔥 Optimice las operaciones de Git con alias que ahorran tiempo.</p>
  
  <a href="https://github.com/soyluisarrieta/git-aliases"> ![Contribuciones Bienvenidas](https://img.shields.io/badge/Contribuciones-bienvenidas-blue.svg) </a>
  
  
  <a href="https://github.com/soyluisarrieta/git-aliases"> ![Alias para git](./terminal-demo.gif) </a>

  [English](./README.md) | Español
</div>

<h2>📜 Tabla de contenidos</h2>

- [✳ Crear un alias global utilizando Git Bash](#✳-crear-un-alias-global-utilizando-git-bash)
- [✨ Configuraciones recomendadas](#✨-configuraciones-recomendadas-por-midudev)
- [📚 Añadir todos los alias recomendados](#📚-añadir-todos-los-alias-recomendados)
- [🧩 Contribuciones](#🧩-contribuciones)

### ✳ Crear un alias global utilizando Git Bash

1. Abre una terminal de **Git Bash** y asegúrate de estar en la ubicación de tu usuario usando el siguiente comando:
    ```bash
    cd ~
    ```
  
2. Ejecuta el siguiente comando para crear o configurar tu perfil:
    ```bash
    notepad .bash_profile
    ```
    Si aún no has creado este archivo, recibirás una solicitud para crear uno nuevo; **confirma y continúa**.

3. Dentro del archivo .bash_profile, puedes agregar tu primer alias. Por ejemplo:
    ```bash
    alias g='git'
    ```
    Cuando guardes los cambios, esto establecerá un alias global "g" para el comando "git".

4. Ahora puedes utilizar este alias en cualquier proyecto Git en tu sistema. Por ejemplo, en lugar de escribir `git -v`, simplemente escribe:
    ```bash
   g -v
    ```

5. Si olvidas alguno de tus alias, puedes ver la **lista completa** ejecutando el siguiente comando:
    ```bash
    alias
    ```

> **Nota:** Estos pasos no son aplicables a terminales como CMD o PowerShell, ya que las configuraciones son específicas de Git Bash y no se reflejarán en otras terminales. Cada entorno de terminal tiene sus propias configuraciones independientes.

### ✨ Configuraciones recomendadas (por [Midudev](https://github.com/midudev))

<details>
<summary>Atajo para el comando git:</summary>

- ⚙️ Configuración:

    ```bash
    alias g='git'
    ```

- 🚀 Uso:

    ```
    g
    ```
</details>

<details>
<summary>Agrega todos los cambios al área de preparación:</summary>

- ⚙️ Configuración:

    ```bash
    alias gaa='git add -A'
    ```

- 🚀 Uso:

    ```
    gaa
    ```
</details>

<details>
<summary>Muestra el estado actual del repositorio:</summary>

- ⚙️ Configuración:

    ```bash
    alias gst='git status'
    ```

- 🚀 Uso:

    ```
    gst
    ```
</details>

<details>
<summary>Realiza una operación pull desde el repositorio remoto:</summary>

- ⚙️ Configuración:

    ```bash
    alias gl='git pull'
    ```

- 🚀 Uso:

    ```
    gl
    ```
</details>

<details>
<summary>Actualiza el repositorio local usando fetch y rebase:</summary>

- ⚙️ Configuración:

    ```bash
    alias gup='git fetch && git rebase'
    ```

- 🚀 Uso:

    ```
    gup
    ```
</details>

<details>
<summary>Sube los cambios al repositorio remoto:</summary>

- ⚙️ Configuración:

    ```bash
    alias gp='git push'
    ```

- 🚀 Uso:

    ```
    gp
    ```
</details>

<details>
<summary>Muestra diferencias con formato mejorado:</summary>

El siguiente alias requiere [diff-so-fancy](https://www.npmjs.com/package/diff-so-fancy):

- ⚙️ Configuración:

    ```bash
    gd() { git diff -w "$@" | diff-so-fancy - }
    ```

- 🚀 Uso:

    ```
    gd
    ```
</details>

<details>
<summary>Realiza un commit con un mensaje:</summary>

- ⚙️ Configuración:

    ```bash
    alias gc='git commit -m'
    ```

- 🚀 Uso:

    ```
    gc "Mensaje del commit"
    ```
</details>

<details>
<summary>Realiza un commit con mensaje y cambios adicionales:</summary>

- ⚙️ Configuración:

    ```bash
    alias gca='git commit -v -a'
    ```

- 🚀 Uso:

    ```
    gca
    ```
</details>

<details>
<summary>Realiza una operación de checkout:</summary>

- ⚙️ Configuración:

    ```bash
    alias gco='git checkout'
    ```

- 🚀 Uso:

    ```
    gco <nombre_de_la_rama_o_commit>
    ```
</details>

<details>
<summary>Cambia al branch "master":</summary>

- ⚙️ Configuración:

    ```bash
    alias gcm='git checkout master'
    ```

- 🚀 Uso:

    ```
    gcm
    ```
</details>

<details>
<summary>Lista las ramas locales:</summary>

- ⚙️ Configuración:

    ```bash
    alias gb='git branch'
    ```

- 🚀 Uso:

    ```
    gb
    ```
</details>

<details>
<summary>Lista todas las ramas, incluyendo las remotas:</summary>

- ⚙️ Configuración:

    ```bash
    alias gba='git branch -a'
    ```

- 🚀 Uso:

    ```
    gba
    ```
</details>

<details>
<summary>Muestra el conteo de commits por autor:</summary>

- ⚙️ Configuración:

    ```bash
    alias gcount='git shortlog -sn'
    ```

- 🚀 Uso:

    ```
    gcount
    ```
</details>

<details>
<summary>Realiza cherry-pick de un commit específico:</summary>

- ⚙️ Configuración:

    ```bash
    alias gcp='git cherry-pick'
    ```

- 🚀 Uso:

    ```
    gcp <hash_del_commit>
    ```
</details>

<details>
<summary>Muestra el registro de commits con estadísticas:</summary>

- ⚙️ Configuración:

    ```bash
    alias glg='git log --stat --max-count=5'
    ```

- 🚀 Uso:

    ```
    glg
    ```
</details>

<details>
<summary>Muestra el registro de commits en forma de gráfico:</summary>

- ⚙️ Configuración:

    ```bash
    alias glgg='git log --graph --max-count=5'
    ```

- 🚀 Uso:

    ```
    glgg
    ```
</details>

<details>
<summary>Muestra el estado actual de manera resumida:</summary>

- ⚙️ Configuración:

    ```bash
    alias gss='git status -s'
    ```

- 🚀 Uso:

    ```
    gss
    ```
</details>

<details>
<summary>Agrega cambios al área de preparación:</summary>

- ⚙️ Configuración:

    ```bash
    alias ga='git add'
    ```

- 🚀 Uso:

    ```
    ga <nombre_del_archivo_o_directorio>
    ```
</details>

<details>
<summary>Realiza una operación de merge:</summary>

- ⚙️ Configuración:

    ```bash
    alias gm='git merge'
    ```

- 🚀 Uso:

    ```
    gm <nombre_de_la_rama_a_mergear>
    ```
</details>

<details>
<summary>Deshace los cambios en el área de preparación:</summary>

- ⚙️ Configuración:

    ```bash
    alias grh='git reset HEAD'
    ```

- 🚀 Uso:

    ```
    grh <nombre_del_archivo_o_directorio>
    ```
</details>

<details>
<summary>Deshace los cambios en el área de preparación de manera forzada:</summary>

- ⚙️ Configuración:

    ```bash
    alias grhh='git reset HEAD --hard'
    ```

- 🚀 Uso:

    ```
    grhh <nombre_del_archivo_o_directorio>
    ```
</details>

<details>
<summary>Crea una nueva rama y cambia a ella:</summary>

- ⚙️ Configuración:

    ```bash
    alias gcb="git switch -c \$1"
    ```

- 🚀 Uso:

    ```
    gcb <nombre_de_la_nueva_rama>
    ```
</details>

### 📚 Añadir todos los alias recomendados

```bash
alias g='git'
alias gaa='git add -A'
alias gst='git status'
alias gl='git pull'
alias gup='git fetch && git rebase'
alias gp='git push'
alias gc='git commit -m'
alias gca='git commit -v -a'
alias gco='git checkout'
alias gcm='git checkout master'
alias gb='git branch'
alias gba='git branch -a'
alias gcount='git shortlog -sn'
alias gcp='git cherry-pick'
alias glg='git log --stat --max-count=5'
alias glgg='git log --graph --max-count=5'
alias gss='git status -s'
alias ga='git add'
alias gm='git merge'
alias grh='git reset HEAD'
alias grhh='git reset HEAD --hard'
alias gcb="git switch -c $1"
```

El siguiente alias requiere [diff-so-fancy](https://www.npmjs.com/package/diff-so-fancy):
```bash
gd() { git diff -w "$@" | diff-so-fancy - }
```

## 🧩 Contribuciones

Te invitamos a compartir tus alias en una [solicitud de extracción](https://github.com/soyluisarrieta/git-aliases/pulls).