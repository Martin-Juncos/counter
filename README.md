### Descripción

El proyecto "Counter" es una aplicación sencilla que permite a los usuarios incrementar y decrementar un contador. Está desarrollado utilizando JavaScript y sirve como un excelente ejemplo para entender la manipulación del DOM y los eventos en JavaScript.

### Funcionalidades

- Incrementar el contador.
- Decrementar el contador.
- Restablecer el contador a cero.

### Puesta en marcha

#### Requisitos previos

- Navegador web moderno.

#### Instalación

1. Clona el repositorio en tu máquina local:

   ```bash
   git clone https://github.com/Martin-Juncos/counter.git
   ```

2. Navega al directorio del proyecto:

   ```bash
   cd counter
   ```

3. Abre el archivo `index.html` en tu navegador web preferido.

### Uso

- **Incrementar el contador**: Haz clic en el botón "Increment".
- **Decrementar el contador**: Haz clic en el botón "Decrement".
- **Restablecer el contador**: Haz clic en el botón "Reset".

### Lógica del Código

La aplicación se compone de tres archivos principales: `index.html`, `styles.css` y `script.js`.

#### script.js

Este archivo maneja la lógica del contador. Se definen los eventos para los botones de incrementar, decrementar y restablecer.

```javascript
document.addEventListener("DOMContentLoaded", () => {
  let counter = 0; // Definimos la variable counter para almacenar el valor del contador.
  const counterDisplay = document.getElementById("counter"); // Obtenemos el elemento HTML donde se mostrará el contador.

  // Añadimos un event listener para el botón de incrementar.
  document.getElementById("increment").addEventListener("click", () => {
    counter++; // Incrementamos el valor del contador.
    updateCounter(); // Actualizamos la visualización del contador.
  });

  // Añadimos un event listener para el botón de decrementar.
  document.getElementById("decrement").addEventListener("click", () => {
    counter--; // Decrementamos el valor del contador.
    updateCounter(); // Actualizamos la visualización del contador.
  });

  // Añadimos un event listener para el botón de restablecer.
  document.getElementById("reset").addEventListener("click", () => {
    counter = 0; // Restablecemos el valor del contador a cero.
    updateCounter(); // Actualizamos la visualización del contador.
  });

  // Función para actualizar la visualización del contador.
  function updateCounter() {
    counterDisplay.textContent = counter; // Mostramos el valor actualizado del contador en el elemento HTML.
  }
});
```

### Cómo Probarlo

1.  Abre el archivo `index.html` en tu navegador.
2.  Haz clic en los botones "Increment", "Decrement" y "Reset" para ver cómo cambia el valor del contador.
3.  Observa cómo el valor del contador se actualiza en tiempo real al interactuar con los botones.

                    ©ProfMartin
