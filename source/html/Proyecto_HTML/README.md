![logotipo de GammaTech School](../../assets/Logo_Yellow.png)

# Proyecto: Creación de un Sitio Web para la Conferencia Internacional

En este ejercicio, deberás crear tres archivos HTML que estén relacionados entre sí para formar un sitio web completo sobre una conferencia. La idea es que cada archivo cumpla una función específica y se pueda navegar entre ellos usando enlaces.

---

## Archivos a Crear

1. **index.html**  
   Página principal de la conferencia. Deberá incluir la presentación del evento, información básica y enlaces de navegación a las otras dos páginas.

2. **registro.html**  
   Página que contiene el formulario avanzado de registro para la conferencia. Puedes utilizar como guía los formularios que te proporcionamos en ejercicios anteriores.

3. **contenido.html**  
   Página que muestra la tabla de contenido (o agenda) de la conferencia, indicando sesiones, talleres, horarios y demás actividades.

---



# Creación de la Página Principal para la Conferencia

## Objetivo
Crear la primera página del sitio web para la conferencia, que funcione como la página de presentación y brinde información básica del evento.

## Requisitos para la Página Principal (index.html)

1. **Estructura Básica:**
   - Define un título usando la etiqueta `<title>` (por ejemplo, "Conferencia Internacional 2025").

2. **Encabezado (Header):**
   - Utiliza un `<header>` para mostrar el nombre de la conferencia.
   - Incluye un título principal `<h1>` con el nombre del evento.
   - Agrega un menú de navegación `<nav>` que contenga enlaces a las demás páginas del sitio:
     - Un enlace a la página de Registro (`registro.html`).
     - Un enlace a la Tabla de Contenido (`contenido.html`).

3. **Contenido Principal:**
   - Crea una o varias secciones `<section>` para describir la conferencia.
   - Incluye información como:
     - Una breve descripción del evento.
     - Detalles importantes (fecha, lugar, objetivos, etc.).
   - Puedes agregar imágenes o gráficos relevantes si lo consideras necesario.

4. **Pie de Página (Footer):**
   - Incluye un `<footer>` para mostrar información adicional, como derechos de autor o información de contacto.
   - Ejemplo: "&copy; 2025 Conferencia Internacional".

5. **Buenas Prácticas:**
   - Utiliza etiquetas semánticas para mejorar la accesibilidad.
   - Agrega comentarios en el código para describir cada sección y facilitar la comprensión.

---------------------------

# Formularios: Registro

## Objetivo

Crear un formulario completo para el registro del participante en la conferencia, que recoja información personal, datos de contacto, preferencias del evento, información adicional y datos de pago, utilizando diversos elementos de formulario y validaciones HTML5.

## Requisitos

**Datos Personales:**

- Nombre y Apellido (input de tipo text).
- Email (input de tipo email).
- Contraseña (input de tipo password, con un mínimo de 6 caracteres).
- Fecha de Nacimiento (input de tipo date).

**Información de Contacto:**

- Teléfono (input de tipo tel).
- Dirección (input de tipo text).

**Preferencias del Evento:**

- **País:** Menú desplegable con `<select>` y por lo menos, 6 opciones.
- **Talleres:** Permitir seleccionar uno o varios talleres (utilizar checkboxes, por ejemplo: Desarrollo Web, Inteligencia Artificial, Diseño).
- **Sesión Principal:** Elegir entre sesiones (radio buttons, por ejemplo: Matutina o Vespertina).

**Subir archivo:**

Permitir al usuario enviar su CV o portafolio (input de tipo file).

**Comentarios adicionales:**

Área de texto (textarea) para que el usuario ingrese observaciones o comentarios.

**Información de Pago:**

- Número de Tarjeta de Crédito: Un campo de texto con validación mediante pattern para 16 dígitos.
- Fecha de Expiración: Utilizar el input de tipo month para la fecha de expiración.

**Botones:**

- Botón para enviar el formulario.
- Botón para reiniciar (borrar) los campos del formulario.

**Consideraciones Adicionales:**

- Utiliza `<fieldset>` y `<legend>` para agrupar secciones y mejorar la semántica y accesibilidad.
- Asegúrate de que los campos obligatorios tengan el atributo `required`.
- Incluye validaciones adicionales con atributos como `pattern`, `minlength` y `maxlength` cuando sea necesario.
- Documenta el código con comentarios para facilitar la comprensión.


-------------------

# Ejercicio: Creación de la Tabla de Contenido de la Conferencia

## Objetivo
Crear la tercera página del sitio web para una conferencia, que sirva como tabla de contenido o agenda del evento, donde se detallen las actividades, sesiones y horarios.

## Requisitos para la Página de Tabla de Contenido (contenido.html)

1. **Estructura Básica:**
- Define un título usando la etiqueta `<title>` (por ejemplo, "Tabla de Contenido - Conferencia Internacional 2025").

2. **Encabezado y Navegación:**
   - Utiliza un `<header>` para incluir un título principal, por ejemplo, "Agenda de la Conferencia".
   - Agrega un menú de navegación `<nav>` que contenga enlaces a:
     - La página principal (index.html)
     - La página de registro (registro.html)

3. **Contenido Principal:**
   - Crea una o más secciones `<section>` para organizar la agenda del evento.
   - Presenta la tabla de contenido utilizando:
     - Una tabla `<table>` que contenga un encabezado y cuerpo.
   - La tabla debe incluir al menos:
     - Horario de la actividad.
     - Título o nombre de la sesión/actividad.
     - Una breve descripción o ubicación (opcional).

   **Ejemplo de contenido hecho con una lista desordenada, pero recuerda que se está pidiendo hacer una tabla:**
   ```html
   <ul>
     <li><strong>09:00 AM:</strong> Registro y Bienvenida</li>
     <li><strong>10:00 AM:</strong> Conferencia Magistral: "El Futuro de la Tecnología"</li>
     <li><strong>11:30 AM:</strong> Taller: Desarrollo Web</li>
     <li><strong>01:00 PM:</strong> Almuerzo</li>
     <li><strong>02:00 PM:</strong> Panel: Innovación y Tendencias</li>
     <li><strong>03:30 PM:</strong> Taller: Diseño UX</li>
     <li><strong>05:00 PM:</strong> Clausura</li>
   </ul>


4. Pie de Página (Footer):
Incluye un `<footer>` que muestre información adicional, como derechos de autor o notas relevantes (por ejemplo, "© 2025 Conferencia Internacional").

¡Buena suerte creando el contenido para la conferencia!
