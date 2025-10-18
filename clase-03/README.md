# Clase 03 - Git Desarrollo Colaborativo

## Ayuda de comandos

```sh
git <comando> --help
git pull --help
git add --help
```

## Como subir los cambios al remoto

```sh
git push
``` 

## Para actualizar el local con el remoto

```sh
git fetch # Me traigo la metadata (Actualizo el .git de mi repo local)
git pull # Me traigo los cambios

# Si yo ya se lo que va estar dentro del repo remoto
git pull # <---- git fetch + git pull
```

## Dividir lo que voy a commitear en varios commits

```sh
git add --patch
# e -> Editar manual lo que quiero guardar en el SA
```

## Referencias estaticas y referencias dinamicas

* Referencias estáticas --> ramas, tags
* Referencias dinamicas --> HEAD

![referencias](_ref/refer.png)