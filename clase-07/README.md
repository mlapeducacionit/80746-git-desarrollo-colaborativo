# Clase 07 - Git Desarrollo Colaborativo

## Git tags

* Marcar versiones de lanzamiento
* Facilitar despligues y rollbacks
* Automatizar versiones en CI/CD
* Compartir versiones con otros

## Listar tags

```sh
git tag
```

## Mostrar información sobre el tag y el commit tagueado

```sh
git show <nombre-tag>
git show v2.0.0
```

## Creando un tag 

> En el último commit de la rama actual

```sh
git tag -a v2.0.0 -m "Segunda versión de la documentación"
```

> Generamos un tag en un commit especifico

```sh
git tag -a v1.0.0 <hash> -m "Primera versión lista"
git tag -a v1.0.0 f80c5f2 -m "Primera versión lista"
# a:annotate | m:mensaje
```

## Para subir un tag al remoto

```sh
git push origin <identificador-tag>
git push origin v2.0.0
```

## Borrar un tag

```sh
git tag -d <identificador-tag>
git tag -d v0.5.0
```