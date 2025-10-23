# Clase 04 - Git Desarrollo Colaborativo

## Trabajando con ramas

### Creando un rama

```sh
git branch <nombre-rama>
git branch feature/ramas
```

## Listar las ramas locales

```sh
git branch
```

## Listar las ramas remotas

```sh
git branch -r
```

## Listar las ramas remotas y locales

```sh
git branch -a
```

## Listas todas las ramas en detalle (locales y remotas)

```sh
git branch -av
```

## Cambiar entre ramas

```sh
git switch <nombre-rama>
git switch feature/ramas
```

> Y si quiero cambiar entre las últimas 2 ramas que se usaron

```sh
git switch -
```

## Ver el estado con detalle de las ramas (En que commits están)

```sh
git branch -av
```

## Crear una rama y mover a esa rama

```sh
git switch -c feature/fusiones
```

## Trabajando con fusiones
**IMPORTANTE**: Es que para hacer una fusión. Tengo que estar en la rama destino. O sea si me quiero traer los cambios de la rama feature/ramas a la rama main, tnego que estar parado en la rama main y traerme los cambios de la otra rama

```sh
git switch main
git merge feature/ramas
```

Pueden suceder 3 cosas

* Fast-forward -> Fusión automatica -> Git se encarga de resolver la fusión
* Tercer Vía -> Diferentes algoritmos para resolver la fusión -> Automatico
* Conflicto -> El proceso de fusión es manual. Voy a tener que solventar el conflicto y avisarle a git que lo hice para terminar el proceso de fusión.

## Herramientas con interfaz gráfica de GIT

* GitHub Desktop <https://desktop.github.com/download/>
* GitKraken <https://www.gitkraken.com/b>