
# Comandos configuración GLOBAL
```
$ git config --global user.name "Juan Perez" 
$ git config --global user.email "micorreo@example.com"

$ git config --global -e
$ git config --list

```
# Comandos iniciales
```
$ git init
$ git status
$ git add nombre_archivo
$ git add .
$ git reset nombre_archivo

$ git commit -m "primer commit"
$ git status
```
* recuperar las ultimas actualizaciones realizadas
```
$git checkout -- .
```

* Saber en que RAMA existen y estamos ubicados

```
$ git branch
$ git status
```
* Cambiar el nombre de la rama
```
$ git branch -m master main
```
* Configurar desde la variables globales que la rama principal sea **main** en lugar de  **master**
```
$ git config --global init.defaultBranch main

```

# Comandos intermedios más utilizados

```
$ git log
```

# Creando alias = Comandos con filtros
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
* Cuantas ramas existen?
```
$ git branch
```

* Creando una nueva rama
```
$ git branch nombre_rama
```
* moverse a una rama
```
$ git checkout nombre_rama
```

* verificar RAMA
```
$ git lg
$git log --oneline
```

* Cambiarse a la rama main-master
```
$ git checkout master
```

* Crear una rama y cambiarse de manera automática en la rama creada
```
$ git checkout -b rama_nueva
$ git branch
```
* Borrar una rama 
```
$ git branch -d rama_nueva
```

* para borrar la branch remota
``` 
$ git push origin --delete remoteBranchName
``` 

* para borrar la branch local
``` 
$ git branch -d localBranchName
```

# Juntar master y una rama_nueva
>[!IMPORTANT]
>
>tiene que estar ubicado en la RAMA  master-main

```
$ git merge rama_nueva
```
>[!NOTE]
>
>corregir los conflictos
```
$ git status
$ git add .
$ git commit -m "conflicto resuelto"
$ git lg

```
# TAGS o etiquetas son una referencia a un commit específico,
>[!IMPORTANT]
>
> Son utilizados para marcar versiones o releases de nuestra app

* Crar una tag
```
$ git tag nuevo_tag
$ git lg
```
* Ver todos los tags que se han creado
```
$ git tag
```
* Borrar un TAG
```
$ git tag -d tag_nuevo
```
>[!IMPORTANT]
>
> Se recomienda utilizar el nombre del TAG relacionado con alguna version

* Creamos un TAG con version
```
$ git tag -a v1.0.0 -m "Version 1.0.0 lista"
$ git lg
```
* Para ver información con respecto a algun TAG
```
$ git show v1.0.0
```
* Subir todos los tags desde git a GitHub
```
$ git push --tags
```


