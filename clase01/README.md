# Clase 01 - GIT desarrollo colaborativo

## Configuración inicial

### Configurando nombre y correo


### Configuracion del editor
```sh
git config --global core.editor "nano"
```
### Chequear editor
```sh
git config --get-regexp editor
```
### Por defecto rama main
```sh
git config --global init.defaultBranch main
```
# Incializando un repositorio de GIT
```sh
git init
```
# Controlar el status de los archivos del proyecto
```sh
git status
```
## Areas posibles en las que pueden estar los archivos
* Working Directory (Directo de trabajo) donde van agregando, borrando al archivo el desarrolllo
* Staging Area (Area de control de cambios) Se agregan los archivos para darle seguimiento y posteriormente sacarles una foto (commit)
* Local Repo (Area de validación de cambios, donde se registran las modificaciones realizadas) Donde van a estar todas las fotos (commit) que vaya sacando.
## Estados de los archivos
* Untracked (Sin seguimiento) => archivos que no se agregaron al index/stage y por consecuente no se les da seguimiento.
* Staged => Archivos que fueron agregados al index/stage area y cuyos cambios van a ser incorporados al repositorio
* Unmodified => Archivos que se cuentran en en el respositorio y no fueron modificado (Con respecto al repositorio)
* Modified => Archivos que se encuentro en el repositorio pero difieren con lo que se encuentra actualmente en el directorio trabajo (Working directory)

# Agregar a la zona de staging
Marcar el archivo o archivos para que formen parte del siguiente commit

```sh
git add -m < nombre-archivo >
git add clase01/README.md
git add . #agregar todo a la zona de confirmación
```


# Hacer un commit (backup, snapshot)
```sh
git commit -m "mensaje descriptivo"
git commit -m "agrego el git lof y el git diff en la docu"
git commit #me abre el editor para yo poder escribir el titulo y el cuerpo del mensaje
```

# Ver la diferencia entre el working directory y el local repo

```sh
git diff
git diff < nombre-archivo >
git diff < clase01/README.ms >

```






<!-- ! GIT no versiona carpetas vacias->
