# Clase 03 - git Desarrollo Colaborativo

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

## Tipos de Fusiones y su resolución

* Fast-foward: cuando no hay conflictos, git soluciona autimaticamente la fusión
* Conflicto: Git no puede resolver por si solo la fusión. Por ende necesita la ayuda del desarrollador/es involucrados en el código que se esta fusionando.

```sh
git diff <nombre-rama>
git diff main
```