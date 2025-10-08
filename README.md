# pp-java

## …or create a new repository on the command line

```bash
echo "# pp" >> README.md
git init
git add README.md
git commit -m "first commit"
git branch -M main
git remote add origin  [rutarepo]
git push -u origin main
```


  ```bash
  git push -u origin main
```
> [!WARNING]  
> $ git push -u origin main To https://github.com/Serio120/api-rest-libros.git
> 
> ! [rejected]        main -> main (fetch first) error: failed to push some refs to 'https://github.com/Serio120/api-rest-libros.git'
> 
> hint: Updates were rejected because the remote contains work that you do not
> 
> hint: have locally. This is usually caused by another repository pushing to
> 
> hint: the same ref. If you want to integrate the remote changes, use
> 
> hint: 'git pull' before pushing again. hint: See the 'Note about fast-forwards' in 'git push --help' for details.

```bash
  git pull origin main --rebase
```
> [!WARNING]
> 
> error: cannot pull with rebase: Your index contains uncommitted changes.
> 
> error: Please commit or stash them.

```bash
  git add .
```

```bash
  git commit -m "Guardando cambios antes del rebase"
```

```bash
  git pull origin main --rebase
```
> [!TIP]
>  [main 7e6f627] Guardando cambios antes del rebase
> 
> 1 file changed, 6 insertions(+)
> 
> create mode 100644 .idea/vcs.xml
> 
> remote: Enumerating objects: 5, done.
> 
> remote: Counting objects: 100% (5/5), done.
> 
> remote: Compressing objects: 100% (5/5), done.
> 
> remote: Total 5 (delta 0), reused 0 (delta 0), pack-reused 0 (from 0)
> 
> Unpacking objects: 100% (5/5), 1.81 KiB | 132.00 KiB/s, done.
> 
> From https://github.com/Serio120/api-rest-libros
> 
> * branch            main       -> FETCH_HEAD
> * [new branch]      main       -> origin/main
>  
> Successfully rebased and updated refs/heads/main.

```bash
  git status
```

```bash
  git push -u origin main
```
