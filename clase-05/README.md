# Clase 05 - Git desarrollado colaborativo

## GIT Reset

### GIT RESET SOFT
Git reset soft agarra los commits que le diga y los borra. Dejando los cambios que lestaban dentro de los commits en el SA.

```sh
git reset --soft <hash>
```

### GIT RESET MIXED (Default)
Git reset mixed (Es el reset por defecto). Agarra los commits que le diga y los borra. Dejando el contenido de los commits dentro del WD.

```sh
git reset <hash>
git reset --mixed <hash>
```

### GIT RESET HARD (Peligroso)
Git reset hard (es el más agresivo de todos). Agarra los commits que le diga y el contenido lo descarta.

```sh
git reset -hard
```

## GIT STASH

### Listar stashes

```sh
git stash list
```

## Ver el contenido del stash

```sh
git stash show -p <stash>
```

## Recuperar un stash

```sh
git stash pop # recupera el ultimo stash creado. Si hay conflicto no lo borra stash.
git stash apply <numero-stash>
git stash apply 1 # stash@{1}
```

## Borrar un stash

```sh
git stash drop # borra el último stash (el de arriba) 
git stash drop <numero-stash> # borra el stash que le paso
git stash drop 0
```

### Crear un branch a partir de un stash

```sh
git stash branch <nombre-rama> 
git stash branch rama-stash
``` 