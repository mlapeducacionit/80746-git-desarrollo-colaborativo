# Clase 02 - Git Desarrollo Colaborativo

## Para ver el estado de los archivos y en que área de git están

```sh
git status
```

## Para pasar los archivos del Working Directory al Staging Area (index area)

```sh
git add .
git add <carpeta>/<archivo>
git add <carpeta1>/<archivo1> <carpeta1>/<archivo2> <carpeta1>/<archivo3>
```

## Para pasar de SA a el LR

```sh
git commit # Editor de texto para colocar el mensaje
git commit -m "mensaje descriptivo"
```

## Diferencia entre el archivo/s que están Working Directory contra el Local Repo

```sh
git diff # compara el archivo que está en WD con el archivo que está en LR
```

## Ver el contenido del commit

```sh
git show <hash>
git show 01b82c5
```

## Ver de manera corta el status de los archivos y en que área están

```sh
git status --short
```

## Ver timeline de commits

```sh
git log --oneline # forma corta
git log # forma larga (detallada)
git log --oneline -<cantidad de commits> 
git log --oneline -2 # ver una cantidad de commit especifica
```

# Subir el repo local al remoto

```sh
git push
```