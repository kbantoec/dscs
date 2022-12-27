# Github

## Adding locally hosted code to GitHub

1. Make sure you communicate with SSH keys
1. In your local repository, `git remote add origin <repo>`
1. `git remote -v`
1. `git fetch`
1. `git push -u origin main`

## How to generate SSH Keys on Windows 11
I use the Git bash terminal in order to use Linux commands.
```shell
$ ssh-keygen
$ cat /c/Users/YBant/.ssh/id_rsa.pub | clip
```