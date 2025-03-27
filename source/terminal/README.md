![logo de GammaTech School](../assets/Logo_Yellow.png)


# Terminal
- 💻 [Guía](../../README.md)
- 💻 [Ejercicios](#ejercicios)  

La terminal es una herramienta indispensable en el desarrollo de software de cualquier tipo. A través de ella tenemos acceso inmediato a cualquier rincón de nuestro ordenador, y  con ella podemos también descargarnos y manejar diversas librerías que nos serán útiles para nuestro trabajo (por ejemplo, **React**).
Por eso, es fundamental que aprendamos a movernos por ella con cierta soltura.  

Podemos pensar en la terminal como una ventana a nuestro PC, pero una ventana que sólo dispone de texto para mostrarnos lo que contiene nuestro ordenador, y sólo podemos comunicarnos con ella a través de texto (comandos de terminal).

De momento, basta con que aprendamos los comandos más básicos.

#### `pwd`
Usando el comando `pwd` (print working directory), sabremos en qué lugar de nuestro ordenador nos encontramos, ya que nos devuelve nuestra posición en la estructura de directorios.

#### `ls`
El comando `ls` (list) nos devuelve una lista de las carpetas y archivos existentes en el directorio en el que nos encontremos.

#### `cd` + nombre
Usando `cd` (change directory), nos moveremos a alguna carpeta que se encuentre por debajo de la carpeta/directorio en el que nos encontremos: `cd Desktop` nos introducirá en el escritorio, `cd Desktop/Programación` entrará en el escritorio y, dentro de él, en la carpeta "Programación", etc.

`cd` sólo puede acceder a carpetas que estén dentro de la carpeta en la que nos encontramos. Para volver atrás y salir de la carpeta, usamos `cd ..`, o `cd ../../..` para salir varios niveles.

#### `mkdir` + nombre / `rmdir` + nombre
Con este comando (`mkdir`: make directory), crearemos una carpeta nueva en el directorio donde nos encontremos: `mkdir mis_notas` crea una carpeta llamada "mis_notas" dentro de la carpeta en la que nos encontremos.
Para borrar una carpeta, usamos `rmdir` (remove directory) y el nombre de la carpeta: `rmdir mis_notas` eliminará la carpeta "mis_notas".

#### `touch`+ nombre / `rm` + nombre
Con este comando creamos un archivo: `touch index.html` crea un archivo HTML llamado "index" en el directorio en el que nos encontremos. El comando `rm` elimina un archivo: `rm index.html`eliminará el archivo "index" que se encuentre en la carpeta en la que estemos.

#### `mv` + nombre + dirección
Con `mv` (move), podemos copiar un archivo o carpeta y pegarlo en otra localización. `mv index.html mi_proyecto` moverá el archivo "index.html" que haya en ese directorio a la carpeta "mi_proyecto".

<a href="#terminal">⬆️</a>

### Recursos para profundizar en la terminal
- [Most Common and Useful Commands to Use](https://www.freecodecamp.org/news/command-line-for-beginners/#mostcommonandusefulcommandstouse)
- [La guía definitiva para aprender a usar la terminal de Linux](https://openwebinars.net/blog/La-guia-definitiva-para-aprender-a-usar-la-terminal-de-Linux/)
- [Comandos básicos para usar en el terminal](https://www.swhosting.com/es/comunidad/manual/comandos-basicos-para-usar-en-el-terminal)

## Ejercicios

1. Abre la terminal y ve a tu escritorio usando los comandos necesarios.
2. Crea una carpeta llamada "ejercicio_terminal".
3. Entra en al carpeta y crea dos carpetas más: "web1" y "web2".
4. Entra en "web1" y crea un archivo "index.html" y otro "style.css".
5. Entra en "web2" t crea un archivo "README.md".
6. Entra en a carpeta "web1" y borra el archivo "style.css". Luego, abre en Visual Studio Code el archivo "index.html" (desde la terminal, obviamente).
7. Ahora, sal al escritorio y borra la carpeta "ejercicio_terminal".

### Terminus
Todo el que acabe los ejercicios puede probar este juego entrando a este enlace.
+ <a target="_blank">[Terminus game](https://web.mit.edu/mprat/Public/web/Terminus/Web/main.html)</a>

<a href="#terminal">⬆️</a>
