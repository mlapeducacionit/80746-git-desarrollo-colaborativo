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

## Trabajar colaborativamente con personas que no conozco (Fork y Pull Request)

Me permite trabajar colaborativamente en proyectos donde no conozco a las personas o no tengo la suficiente confianza para darle permisos al repositorio de trabajo. 

Normalmente cuando trabajo con Fork y Pull Request lo hago en proyectos Open Source.

* Fork es una copia del respositorio remoto de alguien a mi cuenta de GitHub.
* Pull Request. Solicitud  a los dueños originales del repositorio para proponerles un cambio. Es una propuesta de cambio a alguien que no conozco pero quiero ayudar.

1. Hacer un fork del proyecto. Del proyecto del cual quiero contribuir (Me voy copiar en mi cuenta el repo del proyecto original)
2. Me clono el fork desde mi cuenta github
3. Trabajo normalmente. Subo los cambios (A repo propio)
4. Me voy al proyecto original en el apartado Pull Request. Creo un nuevo Pull Request. Algunas veces aparece en mi repo la posibilidad Pull Request.
---
5. Si el repo original sufrió más modificaciones. (Commits). Voy a tener que actualizar mi fork.
6. Voy a la cuenta del proyecto original y me copio la url del repositorio
7. Y agrego en mi repositorio local, la url (el remoto) del proyecto original.

    git remote add upstream <URL-repositorio-original>

8. Me traigo los cambios del repositorio original a mi repo local

    git pull upstream <rama-que-quiero-actualizar>

9. Subo a mi repositorio remoto (Fork) las actualizaciones del repo local

    git push origin <rama-a-actualizar>