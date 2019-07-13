# Curso git y github de platzi

## Si queremos conectar el repositorio de GitHub con nuestro repositorio local, el que creamos con git init, debemos ejecutar las siguientes instrucciones:
 
### Primero: Guardar la URL del repositorio de GitHub con el nombre de origin
```bash
git remote add origin URL
```
### Segundo: Verificar que la URL se haya guardado correctamente:
```bash
git remote
git remote -v
```

### Tercero: Traer la versión del repositorio remoto y hacer merge para crear un commit con los archivos de ambas partes. Podemos usar git fetch y git merge o solo el git pull con el flag --allow-unrelated-histories:
```bash
git pull origin master --allow-unrelated-histories
```
### Por último, ahora sí podemos hacer git push para guardar
### los cambios de nuestro repositorio local en GitHub:
```bash
git push origin master
```
## Comandos
```bash
git stash
```
Guarda un estado temporal

```bash
git stash list
```
Muestra la lista de stash que tenemos

```bash
git stash pop
```
Restablece el estado que teniamos guardados

```bash
git stash branch nameBranch 
```
Se le asigna el stash a una rama

```bash
git stash drop
```
Elimina un stash

////

```bash
git clean --dry-run
```
Muestra una lista de archivos que no son necesarios en el proyecto

```bash
git clean -f
```
Borra los archivos listado (exepto los que se encuentran en .gitignore)

```bash
git cherry-pick idCommit
```
Permite sacar cambios (commits) especifícos de una rama y pasarlos a otra

```bash
git commit --amend --no-edit
```
Permite editar el mensaje del commit

```bash
git --amend
```
Permite editar el commit y los archivos

```bash
git reflog
```
muestra una lista de toda la historia de commits, cada uno con su hash y HEAD

```bash
git reset --soft idHead 
```
mantiene lo que tengas en staging ahí.

```bash
git reset --hasrd idHead 
```
Resetea absolutamente todo incluyendo lo que tengas en staging.