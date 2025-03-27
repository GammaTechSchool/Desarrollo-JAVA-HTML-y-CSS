
![](/source/assets/mediaQueries.png)  

## Qué es RESPONSIVE?

"Responsive" se refiere a la capacidad de un sitio web o aplicación de adaptarse de manera óptima a diferentes tamaños y resoluciones de pantalla, como las de computadoras, tabletas o teléfonos móviles. Esto se logra mediante técnicas de diseño y desarrollo web que permiten que el contenido se reordene, redimensione y ajuste según el dispositivo del usuario, garantizando así una experiencia de usuario consistente y accesible en cualquier plataforma.

Entre las técnicas utilizadas en el DISEÑO responsive se encuentran las Media queries en CSS.

## @Media queries

Permiten aplicar estilos específicos según el tamaño o las características del dispositivo.

- Utiliza la regla `@media` para incluir CSS sólo si se cumple una determinada condición, que normalmente es el tamaño de la pantalla y esto nos asegura que los usuarios puedan acceder y navegar por un sitio web de manera efectiva sin importar el dispositivo que utilicen.

- Diferentes estilos para ordenadores de sobremesa, tabletas y móviles   


## Uso de Herramientas de Desarrollo. Cómo lo ajustamos?

Se recomienda utilizar las herramientas de desarrollador de los navegadores (por ejemplo, el modo responsive en Chrome o Firefox) para:
- Probar y depurar las media queries.
- Ajustar los puntos de ruptura y ver cómo se adapta el diseño en diferentes dispositivos.



## Qué son Breakpoints (punto de quiebre)

Son puntos estratégicos en los que el diseño cambia para adaptarse a diferentes tamaños de pantalla. Estos valores se eligen según las necesidades del proyecto y permiten ajustar el contenido para que se vea bien en cada dispositivo.

Ejemplos de breakpoints comunes:

```css
/* Extra small phones */
@media only screen and (max-width: 600px) {
}

/* Portrait tablets and large phones */
@media only screen and (min-width: 600px) {
}

/* Landscape tablets */
@media only screen and (min-width: 768px) {
}

/* Laptops/desktops */
@media only screen and (min-width: 992px) {
}

/* Large laptops and desktops */
@media only screen and (min-width: 1200px) {
}
```



- Ejemplo sencillo

```css
// Si la ventana del navegador es menor a 500px, el color de fondo cambiará a lightblue:

@media only screen and (max-width: 500px) {
    body {

        background-color: lightblue;
    }
}
```



#### **Always Design for Mobile First** / Siempre se diseña Mobile First

- Esto significa que se codifica el estilo para móviles primero, y se avanza a las otras dimensiones.  
- En el siguiente ejemplo, creamos una clase para estilos móviles y otra para estilos de dispositivos de mayor tamaño.

```css
/* Estilos predeterminados para teléfonos móviles */
.mobile-styles {
    width: 100%;
}

/* Estilos para escritorio en media queries */
@media only screen and (min-width: 768px) {
    /* Estilos para escritorio: */
    .desktop-styles {
        width: 100%;
    }
}
```

#### **Orientation: Portrait / Landscape (horizontal)**

- Se trata de consultas que se aplican en función de la orientación del navegador/dispositivo

```css
@media only screen and (orientation: landscape) {
    body {
        background-color: lightblue;
    }
}
```

### Let's talk about the sizes - `px` vs `em` vs `rem`

- los `Pixels` son una medida absoluta. Hay que moderar el uso excesivo de píxeles, ya que pueden limitar la escalabilidad y accesibilidad del diseño. Sin embargo, esto no quiere decir que hay que evitarlos, si no comprender cuando usarlos.
- Los `REMs` son una forma de establecer el tamaño de la fuente basándose en el tamaño de la fuente del elemento HTML raíz.  
- `em` es relativo al tamaño de fuente de su padre directo o más cercano.
    - Cuando se tienen estilos anidados se hace difícil rastrear los ems.   
    - Esto es lo que solucionan los REM: el tamaño siempre se refiere a la raíz.


 ### 💻 [Ejercicios](./ejercicios/README.md)
