# Clase 03 - git Desarrollo Colaborativo

<<<<<<< HEAD

=======
>>>>>>> repaso-branches
## Crear una nueva rama

```sh
git switch -c <nombre-rama>
```



## Repasando las fusiones en GIT
Estando en la rama que me quiero traer los cambios, ejecuto el siguiente comando.
Por ejemplo si me quiero traer la rama repaso-brancges a main, tengo que estar parado en la rama main y luego ejecutar el comando siguiente

```sh
git merge <nombre-rama-que-me-quiero-traer>
git merge repaso-branches
```

## Comparando ramas con git diff (Tambien puedo hacer ver la diferencia entre ramas)

```sh
git diff <nombre-rama>
git diff main
```

# Para obtener ayuda

```sh
git merge --help
```

## Tipos de Fusiones y su resolución

* Fast-foward: cuando no hay conflictos, git soluciona autimaticamente la fusión
* Algoritmo: cuando GIT detecta cierto grado de modificaci+on, no utiliza el fast-foward. Utiliza diferentes tipos de algortimos. Tambien soluciona por si mismo los posibles incovenientes en la fusion, pero crea un nuevo commit intermedio, usando el ultimo commit de cada rama.
* Conflicto: Git no puede resolver por si solo la fusión. Por ende necesita la ayuda del desarrollador/es involucrados en el código que se esta fusionando.

# Herramientas con GUI para la gestion de un repositorio de GIT ///

* GitHub Desktop:
* GitKraken:

# Stashes


## Crear un stash

```sh
git stash
```

## Recuperar un stash

```sh
git stash pop
```

## Ver los stash

```sh
git stash list
```

## Ver los stash

```sh
git stash 0
```


# Aplicar un stash en particular

```sh
git stash apply <numero-de-stash>
git stash apply 1
```

## Borrar un stash

```sh
git stash drop #Borra el ultimo stash
git stash drop 2 #borra el stash elegido, en este caso el 2
```

```sh
git stash
```

## RESET
Me permite deshacer commits en el arbol de trabajo (Working directory) y en area de preparacion (Staging Area)

### Tipos de reset

* reset soft: borrar el commit seleccionado y coloca el contenido de esos commits en el SA

