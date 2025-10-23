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