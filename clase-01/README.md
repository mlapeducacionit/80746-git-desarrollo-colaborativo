# Clase 01 - Git Desarrollo Colaborativo

# Configuración inicial de GIT

```sh
git config --global user.name "Maximiliano Príncipe"
git config --global user.email "mlapeducacionit@gmail.com"
```

## Visualizar si la configuración impacto.

```sh
git config --global --list
```

## Editar la configuración

```sh
git config --global -e
```

## Estados de los archivos en un repositorio de GIT

* Untracked (Sin seguimiento) => archivos que no se agregaron al index/stage y por consecuente no se les da seguimiento.
* Staged => Archivos que fueron agregados al index/stage area y cuyos cambios van a ser incorporados al repositorio
* Unmodified => Archivos que se cuentran en en el respositorio y no fueron modificado (Con respecto al repositorio)
* Modified => Archivos que se encuentro en el repositorio pero difieren con lo que se encuentra actualmente en el directorio trabajo (Working directory)

## Areas posibles en las que pueden estar los archivos

* Working Directory (Directorio de trabajo) donde se van agregando y borrando archivos en desarrolllos

* Staging Area (Area de control de cambios) Se agregan los archivos para darle seguimiento y posteriormente sacarles una foto (commit)

* Local Repo (Area de validación de cambios, donde se registran las modificaciones realizadas) Donde van a estar todas las fotos (commit) que vaya sacando.

