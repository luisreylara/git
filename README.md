
comandos configuración GLOBAL
```
$ git config --global user.name "Juan Perez" 
$ git config --global user.email "micorreo@example.com"

$ git config --global -e
$ git config --list

```
Comandos más utilizados
```
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

Comandos intermedios más utilizados

```
$ git log

```

Comandos con filtros
```
$ git status --short
$ git log --oneline
$ git log --oneline --decorate --all --graph


```
# Log
git config --global alias.lg "log --graph --abbrev-commit --decorate --format=format:'%C(bold blue)%h%C(reset) - %C(bold green)(%ar)%C(reset) %C(white)%s%C(reset) %C(dim white)- %an%C(reset)%C(bold yellow)%d%C(reset)' --all"

# Status
git config --global alias.s "status --short"

# Alternativa útil de status
git config --global alias.s "status -sb"

# Trabajando con el contenido del archivo
```
$ git diff
$ git diff nombrearchivo
```
## NOTA: Ver git diff en visual studio code

# Ignorando archivos/carpetas - Git Ignore
```
.gitignore

```
[gitignore](https://github.com/luisreylara/git/blob/main/.gitignore) 

# Branch - Ramas - Merge
```
//Creando una nueva rama
$ git branch nombre_rama

// moverse a una rama
$ git checkout nombre_rama

//verificar
$ git lg
$git log --oneline

// cambiarse a la rama main-master
$ git checkout master



```


