![logo de GammaTech School](../assets/Logo_Yellow.png)

# Git y GitHub

- 📋 [Guía](../../README.md)
---
+ [¿qué es git?](#¿qué-es-git)
+ [¿qué es github?](#¿qué-es-github)
    - [Comandos de Git para configurar Github](#comandos-de-git-para-configurar-github)
    - [Primeros pasos](#primeros-pasos)
    - [Comandos de git para trabajar con repositorios](#comandos-de-git-para-trabajar-con-repositorios)

## ¿Qué es Git?  
<br>

>“Git es un **software de control de versiones** que permite llevar el registro de los cambios en los archivos de tu ordenador y coordinar el trabajo que varias personas realizan sobre archivos compartidos."<div style="text-align: right"> Wikipedia </div>

<br>

Nos permite trabajar en equipo de una manera mucho más simple y optima cuando estamos desarrollando software. En la actualidad es una herramienta imprescindible para cualquier desarrollador o equipo de desarrolladores.

Con **Git** podemos controlar todos los cambios que se hacen en nuestro código y tenemos control absoluto de todo lo que pasa con él, pudiendo **volver atrás en el tiempo**, **abrir diferentes ramas de desarrollo**, etc.

Cuando haces modificaciones en un fichero de código y haces un **commit**, Git almacena solo las líneas que has modificado desde tu útlimo **commit**.

<br>
<a href="#git-y-github">⬆️</a>

## ¿Qué es GitHub?

<br>

Es un servicio basado en **Git** que nos provee la posibilidad de **alojar repositorios en la nube**. 

Un **repositorio** es una **carpeta controlada por Git**

Con GitHub podemos acceder de manera remota a nuestros repositorios, clonarlos, compartirlos con otros desarrolladores, etc. 

<br>

## Instalación y configuración

### En Mac desde la terminal
*Deberás tener previamente instalado [Homebrew](https://brew.sh/)*

```
 brew install git
```

### En Linux desde la terminal (Debian/Ubuntu)

```
apt-get install git
```

### En Windows [descargando el ejecutable desde aquí](https://git-scm.com/download/win)
<a href="#git-y-github">⬆️</a>

<br>

## Comandos de Git para configurar Github
Para comprobar que tenemos instalado Git y `ver la versión`, podemos escribir lo siguiente en la terminal:

```
git --version
```


Para ingresar el `nombre de usuario`:
```
git config --global user.name <nombre-de-usuario-en-github>
```


Para ingresar el `email del usuario`:
```
git config --global user.email <tu@email.com>
```


Para `verificar` cuál es el nombre de usuario que tenemos `configurado`:

```
git config --global user.name
```


Para ver la `configuración actual`:
```
git config --list
``` 

<a href="#git-y-github">⬆️</a>  

## Primeros pasos

1. Creamos una cuenta en [GitHub](https://github.com/).
2. [Instalamos](https://git-scm.com/downloads) y configuramos `Git` en nuestro ordenador.
3. Ingresamos a nuestra cuenta en `GitHub` y hacemos click en el botón para crear un `repositorio nuevo`.
4. Ingresamos el `nombre` de nuestro repositorio nuevo.
5. Elegimos si queremos que sea `público o privado`.
6. Elegimos si queremos inicializar nuestro repositorio con un fichero `README file`, un fichero `.gitignore `y/o` una licencia` (por el momento solo seleccionaremos la opción de añadir un fichero `README file`).
7. Hacemos click en `crear repositorio`.
8. Una vez dentro de tu repositorio de GitHub, clickeamos en `code` para copiar la url.
9. En la terminal abrimos la carpeta donde queremos hacer la copia de nuestro repositorio y lo clonamos con el comando `git clone <url>`
10. Con el comando `cd <nombre-del-repositorio>` ingresamos a la carpeta.
11. Abrimos nuestro repositorio en Visual Studio Code y hacemos las modificaciones que deseamos. Una vez terminado guardamos todo. 
12. Desde la terminal ejecutamos `git status` para visualizar qué ficheros han sufrido cambios y aún no están `commiteados`.
13. Ejecutamos `git add <nombre-de-los-ficheros-modificados>` o `git add -A` para agregar todos los ficheros al staging area.
14. Ejecutamos `git commit -m "<tu mensaje>"` para agregar un mensaje al commit que nos permita identificar los cambios realizados en esta versión del fichero.
15. Ejecutamos `git push` para subir todos los cambios que tenemos en local a nuestro repositorio remoto.

<a href="#git-y-github">⬆️</a>

### Comandos de git para trabajar con repositorios:

Para `clonar` (hacer una copia) de tu repositorio de GitHub en local:

```
git clone <url-del-repo-que-quieres-clonar> <nombre-alternativo-para-carpeta-local> (opcional)
``` 


Para `añadir al staging area` (preaprar para guardar archivos en git) uno o más ficheros determinados:
```
git add <nombre-del-fichero>
```


Para `añadir al staging area` todos los ficheros que han sufrido modificaciones:
```
git add -A` o `git add .
```


Para realizar un `commit` y agregar un mensaje que lo identifique:
```
git commit -m "<tu-mensaje>"
``` 


Para `subir los cambios` al repositorio en remoto (GitHub):
```
git push
``` 


Para `descargar los cambios` que estén en remoto y no tenga en mi ordenador:
```
git pull
```

Para ver el `historial de todos los commits` realizados en ese repositorio:

```
git log
```



## Recursos adicionales

- [Te lo explico con gatitos](https://teloexplicocongatitos.com/poster/tlecg04) 

- [Taller de Introducción a Git](https://www.youtube.com/watch?v=HiXLkL42tMU)

- [Learn Git Branching Game](https://learngitbranching.js.org/)

- [Sitio oficial de Git](https://git-scm.com/)
