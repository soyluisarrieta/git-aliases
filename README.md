# Mis recursos de Git y Github

## Aliases

| Alias  | Comando Correspondiente                                        | Descripción                                      | Comando |
|--------|--------------------------------------------------------------|--------------------------------------------------|---------|
| g      | git                                                          | Atajo para el comando git.                      | [Configurar](#configurar-g) |
| gaa    | git add -A                                                   | Agrega todos los cambios al área de preparación. | [Configurar](#configurar-gaa) |
| gst    | git status                                                   | Muestra el estado actual del repositorio.        | [Configurar](#configurar-gst) |
| gl     | git pull                                                     | Realiza una operación pull desde el repositorio remoto. | [Configurar](#configurar-gl) |
| gup    | git fetch && git rebase                                      | Actualiza el repositorio local usando fetch y rebase. | [Configurar](#configurar-gup) |
| gp     | git push                                                     | Sube los cambios al repositorio remoto.         | [Configurar](#configurar-gp) |
| gd()   | git diff -w "$@" \| diff-so-fancy -                          | Muestra diferencias con formato mejorado.       | [Configurar](#configurar-gd) |
| gc     | git commit -m                                                | Realiza un commit con un mensaje.                | [Configurar](#configurar-gc) |
| gca    | git commit -v -a                                             | Realiza un commit con mensaje y cambios adicionales. | [Configurar](#configurar-gca) |
| gco    | git checkout                                                 | Realiza una operación de checkout.              | [Configurar](#configurar-gco) |
| gcm    | git checkout master                                          | Cambia al branch "master".                      | [Configurar](#configurar-gcm) |
| gb     | git branch                                                   | Lista las ramas locales.                         | [Configurar](#configurar-gb) |
| gba    | git branch -a                                                | Lista todas las ramas, incluyendo las remotas.   | [Configurar](#configurar-gba) |
| gcount | git shortlog -sn                                             | Muestra el conteo de commits por autor.         | [Configurar](#configurar-gcount) |
| gcp    | git cherry-pick                                              | Realiza cherry-pick de un commit específico.     | [Configurar](#configurar-gcp) |
| glg    | git log --stat --max-count=5                                 | Muestra el registro de commits con estadísticas. | [Configurar](#configurar-glg) |
| glgg   | git log --graph --max-count=5                                | Muestra el registro de commits en forma de gráfico. | [Configurar](#configurar-glgg) |
| gss    | git status -s                                                | Muestra el estado actual de manera resumida.     | [Configurar](#configurar-gss) |
| ga     | git add                                                      | Agrega cambios al área de preparación.           | [Configurar](#configurar-ga) |
| gm     | git merge                                                    | Realiza una operación de merge.                 | [Configurar](#configurar-gm) |
| grh    | git reset HEAD                                               | Deshace los cambios en el área de preparación.   | [Configurar](#configurar-grh) |
| grhh   | git reset HEAD --hard                                        | Deshace los cambios en el área de preparación de manera forzada. | [Configurar](#configurar-grhh) |
| gcb    | git switch -c $1                                             | Crea una nueva rama y cambia a ella.            | [Configurar](#configurar-gcb) |

