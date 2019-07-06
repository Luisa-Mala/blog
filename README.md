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

### Tercero: Traer la versión del repositorio remoto y
### hacer merge para crear un commit con los archivos
### de ambas partes. Podemos usar git fetch y git merge
### o solo el git pull con el flag --allow-unrelated-histories:
```bash
git pull origin master --allow-unrelated-histories
```
### Por último, ahora sí podemos hacer git push para guardar
### los cambios de nuestro repositorio local en GitHub:
```bash
git push origin master
```
