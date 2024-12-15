# a. Como se inicializa un repositorio en github?
## Ejecutando el comando:
```bash 
 git init 
 ```
# b. Como creas un repositorio en github?
## Para crear un repositorio remoto se debe iniciar sesion en la interfaz de git bash y tras vincular la carpeta en uso con el comando mencionado se prodra corroborar la existencia del repositorio remoto en el sitio de github 
# c. Como vinculas un repositorio local y uno remoto de github? 
## Tras exisitir ambos, ejecutar los siguientes comandos: 
 ```bash 
 git branch -M main
 git remote add origin https://github.com/usuario/repositorio.git
 git push -u origin main 
 ```
# d. Cual es el flujo basico de trabajo de Git y Github?
## Consiste en tres estdos locales: _modified,staged,commited,remote_ ![git flow](imgs/git-flow.jpg)
# e. Para que sirve el archivo .gitignore?
## Para marcar que tipo de archivos que aunque se encuentren dentro de la carpeta no se incluya en el repositorio 
# f. Cual es el proposito de una rama?
## Segregar funcionalidades en el codigo previo a su adicion a la version principal
```bash
git branch nombre-ramag
git checkout nombre-rama
git branch -d nombre-rama
```
# g. Que es una fusion?
## Unir las versiones del codigo aisladas en las ramas a la version principal 
```bash
git checkout rama-principal
git merge rama-secundaria
```
# h. Explica los diferentes tipos de fusion que existen 
## Fast-Forward: Cuando la fusion se realiza sin conflictos en el codigo                
## Manual Merge: Realizar la fusion manualmente para resolver los conflictos 
# i. Como puedes ver el hsitrial de tu repositorio
## Ejecutando uno de los siguientes comandos: 
```bash
git log
git log --oneline
```
## Para un analisis mas completo: 
```bash
git reflog
```
# Cual es el proposito de una etiqueta?
## Numerar las versiones del codigo para remarcar los cambios mediante nomenclatura semver
```bash
git tag numero-versión
git show numero-versión
git tag -d numero-versión
```