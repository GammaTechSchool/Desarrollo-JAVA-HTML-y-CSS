![logotipo de GammaTech School](../../assets/Logo_Yellow.png)


## HTML - Formulario

- 💻 [HTML](../README.md)

### Formularios
# Material de Clase: Formularios en HTML

## 1. Introducción

Los **formularios** en HTML son la forma en que las páginas web interactúan con los usuarios. Permiten recolectar datos que luego pueden ser enviados a un servidor para procesarlos, ya sea para iniciar sesión, registrarse, realizar búsquedas, enviar comentarios, etc.

### ¿Por qué usar formularios?
- **Interacción:** Permiten que los usuarios ingresen información.
- **Procesamiento de datos:** Los datos pueden ser enviados a un servidor para su análisis o almacenamiento.
- **Accesibilidad:** Con un buen uso de etiquetas, se mejora la experiencia para todos los usuarios.

---

## 2. Estructura Básica de un Formulario

El elemento principal es la etiqueta `<form>`, que delimita el formulario. Los atributos más importantes son:


**Ejemplo básico:**

```html
<form>
  <!-- Aquí irán los elementos del formulario -->
</form>
```


3. Elementos Comunes en los Formularios
a) Entradas de Texto
Campo de texto: Para introducir información alfanumérica.

```html
<label for="nombre">Nombre:</label>
<input type="text" id="nombre" name="nombre" placeholder="Ingresa tu nombre" required>
```

Contraseña: Para campos sensibles como contraseñas.

```html
<label for="password">Contraseña:</label>
<input type="password" id="password" name="password" required>
```

Email: Permite validar que se ingrese un correo electrónico.

```html
<label for="email">Email:</label>
<input type="email" id="email" name="email" placeholder="ejemplo@dominio.com" required>
```

b) Botones y Otros Controles
Botón de envío:

```html
<input type="submit" value="Enviar">
```

Botón de reinicio: Permite borrar todos los campos del formulario.
```html
<input type="reset" value="Borrar">
```

Radio Buttons: Para seleccionar una opción de un conjunto.

```html
<p>Género:</p>
<label>
  <input type="radio" name="genero" value="masculino" required> Masculino
</label>
<label>
  <input type="radio" name="genero" value="femenino" required> Femenino
</label>
```

Checkbox: Permite seleccionar una o más opciones.
```html
<p>Intereses:</p>
<label>
  <input type="checkbox" name="intereses" value="deportes"> Deportes
</label>
<label>
  <input type="checkbox" name="intereses" value="musica"> Música
</label>
```

Área de texto: Para textos largos, como comentarios.

```html
<label for="comentario">Comentario:</label>
<textarea id="comentario" name="comentario" rows="4" cols="50" placeholder="Escribe tu comentario aquí..."></textarea>
```

c) Agrupación de Elementos
Para mejorar la organización y la semántica, se pueden agrupar elementos relacionados usando:

```html
<fieldset>: Agrupa elementos dentro de un recuadro.
<legend>: Proporciona un título al grupo.

<fieldset>
  <legend>Información Personal</legend>
  <label for="nombre">Nombre:</label>
  <input type="text" id="nombre" name="nombre" required>
  <br>
  <label for="email">Email:</label>
  <input type="email" id="email" name="email" required>
</fieldset>
```


4. Ejemplo Completo de Formulario
A continuación, se muestra un ejemplo completo que reúne varios de los elementos mencionados:

```html
<!DOCTYPE html>
<html lang="es">
<head>
  <meta charset="UTF-8">
  <title>Formulario de Registro</title>
</head>
<body>
  <h1>Registro de Usuario</h1>
  <form action="procesar_registro.php" method="post">
    <fieldset>
      <legend>Datos Personales</legend>
      <label for="nombre">Nombre:</label>
      <input type="text" id="nombre" name="nombre" placeholder="Ingresa tu nombre" required>
      <br><br>
      <label for="email">Email:</label>
      <input type="email" id="email" name="email" placeholder="ejemplo@dominio.com" required>
      <br><br>
      <label for="password">Contraseña:</label>
      <input type="password" id="password" name="password" required>
    </fieldset>
    <br>
    <fieldset>
      <legend>Preferencias</legend>
      <p>Género:</p>
      <label>
        <input type="radio" name="genero" value="masculino" required> Masculino
      </label>
      <label>
        <input type="radio" name="genero" value="femenino" required> Femenino
      </label>
      <br><br>
      <p>Intereses:</p>
      <label>
        <input type="checkbox" name="intereses" value="deportes"> Deportes
      </label>
      <label>
        <input type="checkbox" name="intereses" value="musica"> Música
      </label>
    </fieldset>
    <br>
    <input type="submit" value="Registrar">
    <input type="reset" value="Borrar">
  </form>
</body>
</html>
```

Explicación del ejemplo:

Se definen dos grupos de datos con `<fieldset>` y `<legend>`: uno para los datos personales y otro para las preferencias.
Cada campo tiene un <label> asociado para mejorar la accesibilidad.
Se utilizan los atributos placeholder y required para mejorar la usabilidad.
Se incluyen botones para enviar y reiniciar el formulario.

5. Buenas Prácticas
Accesibilidad: Usa siempre etiquetas <label> con el atributo for para relacionarlas con sus correspondientes campos de entrada.
Validación: Utiliza atributos como required, minlength, maxlength y tipos específicos (email, number, etc.) para mejorar la validación de los datos.
Estructura semántica: Organiza el formulario con <fieldset> y <legend> para agrupar campos relacionados.
Comentarios en el código: Comenta el código para que los estudiantes puedan entender cada parte.



Select (Lista Desplegable):

El elemento <select> permite crear un menú desplegable con opciones. Se definen mediante elementos <option>. Puedes establecer una opción preseleccionada utilizando el atributo selected en la opción deseada.

```html
<label for="pais">País:</label>
<select id="pais" name="pais">
  <option value="mx">México</option>
  <option value="es" selected>España</option>
  <option value="us">Estados Unidos</option>
</select>
```


Input de Color:
El elemento <input type="color"> muestra un selector de color, permitiendo al usuario elegir un color. El valor se define en formato hexadecimal.

```html
<label for="color">Elige un color:</label>
<input type="color" id="color" name="color" value="#ff0000">
```


