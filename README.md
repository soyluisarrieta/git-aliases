<div align="center">
  <h1>Git aliases</h1>
  <p>Streamline Git Operations with Time-Saving Aliases</p>
</div>

<h2>Table of contents</h2>

- [How to create a global alias using Git Bash](#how-to-create-a-global-alias-using-git-bash)
- [Recommended configurations (by Midudev)](#recommended-configurations-by-midudev)
- [Add all recommended aliases](#add-all-recommended-aliases)

### How to create a global alias using Git Bash

1. Open a **Git Bash** terminal and make sure you're in your user's location using the following command:
    ```bash
    cd ~
    ```
  
2. Run the following command to create or configure your profile:
    ```bash
    notepad .bash_profile
    ```
    If you haven't created this file yet, you'll be prompted to create a new one; **confirm and proceed**.

3. Inside the .bash_profile file, you can add your first alias. For example:
    ```bash
    alias g='git'
    ```
    When you save the changes, this will set a global alias "g" for the "git" command.

4. Now you can use this alias in any Git project on your system. For example, instead of typing `git -v`, simply type:
    ```bash
    g -v
    ```

5. If you forget any of your aliases, you can view the **complete list** by running the following command:
    ```bash
    alias
    ```

> **Note:** These steps are not applicable to terminals like CMD or PowerShell since the configurations are specific to Git Bash and won't reflect in other terminals. Each terminal environment has its independent configurations.

### Recommended configurations (by [Midudev](https://github.com/midudev))

<details>
<summary>Alias for the git command:</summary>

- Configuration:

    ```bash
    alias g='git'
    ```

- Usage:

    ```
    g
    ```
</details>

<details>
<summary>Add all changes to the staging area:</summary>

- Configuration:

    ```bash
    alias gaa='git add -A'
    ```

- Usage:

    ```
    gaa
    ```
</details>

<details>
<summary>Show the current repository status:</summary>

- Configuration:

    ```bash
    alias gst='git status'
    ```

- Usage:

    ```
    gst
    ```
</details>

<details>
<summary>Perform a pull operation from the remote repository:</summary>

- Configuration:

    ```bash
    alias gl='git pull'
    ```

- Usage:

    ```
    gl
    ```
</details>

<details>
<summary>Update the local repository using fetch and rebase:</summary>

- Configuration:

    ```bash
    alias gup='git fetch && git rebase'
    ```

- Usage:

    ```
    gup
    ```
</details>

<details>
<summary>Push changes to the remote repository:</summary>

- Configuration:

    ```bash
    alias gp='git push'
    ```

- Usage:

    ```
    gp
    ```
</details>

<details>
<summary>Show differences with enhanced formatting:</summary>

The following alias requires [diff-so-fancy](https://www.npmjs.com/package/diff-so-fancy):

- Configuration:

    ```bash
    gd() { git diff -w "$@" | diff-so-fancy - }
    ```

- Usage:

    ```
    gd
    ```
</details>

<details>
<summary>Commit with a message:</summary>

- Configuration:

    ```bash
    alias gc='git commit -m'
    ```

- Usage:

    ```
    gc "Commit message"
    ```
</details>

<details>
<summary>Commit with a message and additional changes:</summary>

- Configuration:

    ```bash
    alias gca='git commit -v -a'
    ```

- Usage:

    ```
    gca
    ```
</details>

<details>
<summary>Perform a checkout operation:</summary>

- Configuration:

    ```bash
    alias gco='git checkout'
    ```

- Usage:

    ```
    gco <branch_name_or_commit>
    ```
</details>

<details>
<summary>Switch to the "master" branch:</summary>

- Configuration:

    ```bash
    alias gcm='git checkout master'
    ```

- Usage:

    ```
    gcm
    ```
</details>

<details>
<summary>List local branches:</summary>

- Configuration:

    ```bash
    alias gb='git branch'
    ```

- Usage:

    ```
    gb
    ```
</details>

<details>
<summary>List all branches, including remote ones:</summary>

- Configuration:

    ```bash
    alias gba='git branch -a'
    ```

- Usage:

    ```
    gba
    ```
</details>

<details>
<summary>Show commit count per author:</summary>

- Configuration:

    ```bash
    alias gcount='git shortlog -sn'
    ```

- Usage:

    ```
    gcount
    ```
</details>

<details>
<summary>Cherry-pick a specific commit:</summary>

- Configuration:

    ```bash
    alias gcp='git cherry-pick'
    ```

- Usage:

    ```
    gcp <commit_hash>
    ```
</details>

<details>
<summary>Show commit log with statistics:</summary>

- Configuration:

    ```bash
    alias glg='git log --stat --max-count=5'
    ```

- Usage:

    ```
    glg
    ```
</details>

<details>
<summary>Show commit log as a graph:</summary>

- Configuration:

    ```bash
    alias glgg='git log --graph --max-count=5'
    ```

- Usage:

    ```
    glgg
    ```
</details>

<details>
<summary>Show the current status in a summarized form:</summary>

- Configuration:

    ```bash
    alias gss='git status -s'
    ```

- Usage:

    ```
    gss
    ```
</details>

<details>
<summary>Add changes to the staging area:</summary>

- Configuration:

    ```bash
    alias ga='git add'
    ```

- Usage:

    ```
    ga <file_or_directory_name>
    ```
</details>

<details>
<summary>Perform a merge operation:</summary>

- Configuration:

    ```bash
    alias gm='git merge'
    ```

- Usage:

    ```
    gm <branch_name_to_merge>
    ```
</details>

<details>
<summary>Undo changes in the staging area:</summary>

- Configuration:

    ```bash
    alias grh='git reset HEAD'
    ```

- Usage:

    ```
    grh <file_or_directory_name>
    ```
</details>

<details>
<summary>Forcefully undo changes in the staging area:</summary>

- Configuration:

    ```bash
    alias grhh='git reset HEAD --hard'
    ```

- Usage:

    ```
    grhh <file_or_directory_name>
    ```
</details>

<details>
<summary>Create a new branch and switch to it:</summary>

- Configuration:

    ```bash
    alias gcb="git switch -c \$1"
    ```

- Usage:

    ```
    gcb <new_branch_name>
    ```
</details>

### Add all recommended aliases

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

The following alias requires [diff-so-fancy](https://www.npmjs.com/package/diff-so-fancy):
```bash
gd() { git diff -w "$@" | diff-so-fancy - }
```
