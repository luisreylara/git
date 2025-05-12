
comandos básicos de git
```
$ git config --global user.name "John Doe" 
$ git config --global user.email "johndoe@example.com"

$ git config --global -e
$ git config --list

$ git init
$ git status
$ git add nombre_archivo
$ git add .
$ git reset nombre_archivo

$ git commit -m "primer commit"
$ git status

// recuperar las ultimas actualizaciones realizadas
$git checkout -- .

// Saber la rama 
$ git branch
$ git status

// cambiar el nombre de la rama
$ git branch -m master main

// configurar desde la variables globales que la rama principal sea main por master
$ git config --global init.defaultBranch main

```
