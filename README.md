# Mis recursos de Git y Github

## Aliases

| Alias  | Comando Correspondiente                                        | Descripción                                      |
|--------|--------------------------------------------------------------|--------------------------------------------------|
| g      | git                                                          | Atajo para el comando git.                      |
| gaa    | git add -A                                                   | Agrega todos los cambios al área de preparación. |
| gst    | git status                                                   | Muestra el estado actual del repositorio.        |
| gl     | git pull                                                     | Realiza una operación pull desde el repositorio remoto. |
| gup    | git fetch && git rebase                                      | Actualiza el repositorio local usando fetch y rebase. |
| gp     | git push                                                     | Sube los cambios al repositorio remoto.         |
| gd()   | git diff -w "$@" \| diff-so-fancy -                          | Muestra diferencias con formato mejorado.       |
| gc     | git commit -m                                                | Realiza un commit con un mensaje.                |
| gca    | git commit -v -a                                             | Realiza un commit con mensaje y cambios adicionales. |
| gco    | git checkout                                                 | Realiza una operación de checkout.              |
| gcm    | git checkout master                                          | Cambia al branch "master".                      |
| gb     | git branch                                                   | Lista las ramas locales.                         |
| gba    | git branch -a                                                | Lista todas las ramas, incluyendo las remotas.   |
| gcount | git shortlog -sn                                             | Muestra el conteo de commits por autor.         |
| gcp    | git cherry-pick                                              | Realiza cherry-pick de un commit específico.     |
| glg    | git log --stat --max-count=5                                 | Muestra el registro de commits con estadísticas. |
| glgg   | git log --graph --max-count=5                                | Muestra el registro de commits en forma de gráfico. |
| gss    | git status -s                                                | Muestra el estado actual de manera resumida.     |
| ga     | git add                                                      | Agrega cambios al área de preparación.           |
| gm     | git merge                                                    | Realiza una operación de merge.                 |
| grh    | git reset HEAD                                               | Deshace los cambios en el área de preparación.   |
| grhh   | git reset HEAD --hard                                        | Deshace los cambios en el área de preparación de manera forzada. |
| gcb    | git switch -c $1                                             | Crea una nueva rama y cambia a ella.            |
