# Clase 03 - git Desarrollo Colaborativo


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

# Herramientas visuales

* GitDesktop