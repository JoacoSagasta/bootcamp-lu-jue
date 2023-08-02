# Clase 15

## Configuración inicial.

```sh
git config --global user.name "JoacoSagasta" 
git config --global user.email "joacosagasta@hotmail.com"
```
## Verificar si todo quedó bien o si hice estas configuraciones-

```sh
git config --get-regexp user
```
## Crear un repositorio (Inicializar un repo)

```sh
git init
``` 
## Areas del repositorio de GIT

3 Áreas

* Working Directorio (WD): Directorio de trabajo donde se van agregando o quitando los archivos durante el desarrollo
* Staging Area (SA): (Área de control de cambios. Área tempora/intermedia)
* Local Repo (LR): (Una caja donde voy a ir teniendo todas las fotos que vaya sacando)

## El estado de los archivos

3 Estados

* untracked: Archivos que están en el WD pero GIT no les está dando seguimiento.
* unmodified: Archivos que GIt ya está siguiendo y con respecto al WD, no fueron modificados.
* modified: (Archivos que se encuentran en el repositorio (Están siendo seguidos por GIT) pero difieren con lo que se encuentra actualmente en el WD)
* staged: Archivos que están en el área temporal/intermedia

## Saber estado actual de los archivos

```sh
git status (estado en el Staging Area(SA))
También sirve para ver en que rama está
```## Pasos para subir archivos

```sh
git add (subo al SA)
```
```sh
git commit -m "escribo el mensaje acerca de que estoy subiendo"
```
```sh
git log <!-- lo uso para ver la foto de todo lo que voy subiendo - Estado en el LocalRepo (LR)) --> DESPUES APRETAR LA LETRA "Q" para salir
git log --oneline <!-- # para usar en una sola linea -->
``````sh
git restore README.md <!-- Recupero el archivo en la versión anterior -->
```
# Clase 16

## .gitignore

Este archivo sirve para ignorar carpetas o archivos que no quiero que sean parte del repositorio. Normalmente va sobre la raíz del proyecto
```sh
touch .gitignore
```
# Ayuda de GIT

```sh
git restore --help
```

## Agrego a mi repo local la url del repo remoto

```sh
git remote add origin https://github.com/JoacoSagasta/bootcamp-lu-jue.git
```
### Visualizar si se agregó o qué url tengo agregada

```sh
git remote -v
```
Voy a crear una rama
