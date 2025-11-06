# Clase 08 - Git Desarrollo Colaborativo

## Git Rebase
Me permite mover el punto donde se hizo la bifurcación. O sea incluir en la rama destino el commit de la rama actual.

```sh
# Tengo que estar en la rama donde quiero mover la base
git switch feature/rebase 
git rebase main
``` 

## Git Rebase interativo