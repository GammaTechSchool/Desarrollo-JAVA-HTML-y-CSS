

## Ejemplo de HTML - Cuerpo

```html
<body>
  <h1>Ejemplos de Transformaciones CSS</h1>
  <div class="container">
    <div class="box translate">Translate</div>
    <div class="box rotate">Rotate</div>
    <div class="box scale">Scale</div>
    <div class="box skew">Skew</div>
    <div class="box combo">Combo</div>
  </div>
</body>
```

## Ejemplo de CSS - Animaciones


```html
body {
  font-family: Arial, sans-serif;
  margin: 0;
  padding: 0;
  background-color: #f1f1f1;
  justify-content: center;
  align-items: center;
  min-width: 100vw;
  min-height: 100vh;
  display: flex;
  flex-direction: column;
}

/* Estilos generales para las cajas */
.container {
  display: flex;
  flex-wrap: wrap;
  gap: 20px;
  padding: 20px;
}
.box {
  width: 150px;
  height: 150px;
  background-color: #3498db;
  color: #fff;
  font-size: 1.2em;
  display: flex;
  align-items: center;
  justify-content: center;
  transition: transform 0.5s ease;
}

/* Ejemplo de translate: mueve la caja 50px a la derecha y 20px hacia abajo */
.translate:hover {
  transform: translate(50px, 20px);
}

/* Ejemplo de rotate: rota la caja 45 grados */
.rotate:hover {
  transform: rotate(45deg);
}

/* Ejemplo de scale: escala la caja 1.5 veces su tamaño original */
.scale:hover {
  transform: scale(1.5);
}

/* Ejemplo de skew: inclina la caja 20 grados horizontal y 10 grados vertical */
.skew:hover {
  transform: skew(20deg, 10deg);
}

/* Ejemplo combinando varias transformaciones */
.combo:hover {
  transform: translate(20px, 20px) rotate(30deg) scale(1.2) skew(10deg, 5deg);
}
```

Ejemplo 1: Transición en un botón
En este ejemplo, al hacer hover sobre el botón, se cambia el color de fondo y se aplica un escalado. Se usan varias propiedades de transición en una sola línea.

```html
 <button id="buttonShop">Comprar</button>

 #buttonShop {
      background-color: #3498db;
      color: white;
      padding: 10px 20px;
      border: none;
      cursor: pointer;
      /* La transición se aplica a background-color y transform */
      transition: background-color 0.5s ease, transform 0.5s ease-in-out;
    }

    #buttonShop:hover {
      background-color: #e74c3c;
      transform: scale(1.1);
    }

```
Explicación:

transition: Se define que el cambio de background-color dura 0.5s con suavidad ease y el cambio de transform (en este caso, el escalado) dura 0.5s con ease-in-out.
:hover: Al pasar el ratón sobre el botón, se activa la transición.


Ejemplo 2: Transición con retraso
En este ejemplo se muestra cómo retrasar el inicio de la transición. La caja cambia su ancho de 100px a 300px con una duración de 2 segundos y un retraso de 1 segundo.

```html
 <div class="retraso"></div>

 .retraso {
      width: 100px;
      height: 100px;
      background: red;
      transition: width 2s ease-out 1s;
    }

    .retraso:hover {
      width: 300px;
    }
```
Explicación:

transition: width 2s ease-out 1s;
Propiedad: width
Duración: 2 segundos
Suavidad: ease-out (la animación desacelera al final)
Retraso: 1 segundo
Al hacer hover, la caja incrementa su ancho, pero el cambio comienza 1 segundo después del hover.



Ejemplo 3:Uso de propiedades individuales de transición

Este ejemplo demuestra cómo definir de forma separada cada parte de la transición para dos propiedades: width y background-color.

```html
 <div class="individuales"></div>

 .individuales {
      width: 150px;
      height: 150px;
      background-color: #8e44ad;
      /* Se aplican transiciones diferentes para cada propiedad */
      transition-property: width, background-color;
      transition-duration: 1s, 0.5s;
      transition-timing-function: ease-in-out, linear;
      transition-delay: 0s, 0.5s;
    }

    .individuales:hover {
      width: 300px;
      background-color: #e67e22;
    }
```

Explicación:

transition-property: Especifica que las transiciones se aplican a width y background-color.
transition-duration: La transición de width dura 1s y la de background-color 0.5s.
transition-timing-function: La transición de width usa ease-in-out y la de background-color es linear.
transition-delay: La transición de width inicia inmediatamente, mientras que la de background-color se retrasa 0.5s.
