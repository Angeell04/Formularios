# Documentación del Configurador de Vehículo

Enlace a la aplicación web: [cozy-starburst-e33aba.netlify.app](https://cozy-starburst-e33aba.netlify.app)

## Elementos Visibles de la Interfaz

La aplicación muestra una tarjeta central dividida en los siguientes apartados:

### 1. Desplegables de Configuración
* **Motorización**: Selector entre Gasolina (7.500 €) y Diésel (9.200 €).
* **Cilindrada / Potencia**: Selector entre 1200 cc (+900 €), 1900 cc (+2.100 €) y 2300 cc (+2.600 €).
* **Tipo de Pintura**: Selector entre acabado Normal (+750 €), Mate (+1.400 €) y Metalizada (+1.580 €).
* **Color**: Selector entre Negro, Blanco, Rojo, Azul, Verde y Gris, con un texto informativo que avisa de las restricciones de pintura.

### 2. Equipamiento y Extras Opcionales
Casillas de verificación para añadir componentes:
* **Alerón deportivo** (+190 €)
* **Radio-CD con MP3** (+230 €)
* **Altavoces gama alta** (+530 €)
* **GPS incorporado** (+520 €)

### 3. Botones de Control
* **Guardar Configuración**: Botón para procesar la selección y calcular el precio.
* **Restablecer**: Botón para limpiar todos los campos del formulario.

## Respuestas Visibles de la Aplicación

### Resultado Correcto
Si la configuración es válida, se genera un mensaje de texto visible en la parte inferior del formulario con el coste total:
* "Tienes que pagar: [precio final en euros]"

### Avisos y Restricciones
Si la combinación seleccionada es incompatible, se muestra una ventana emergente de aviso (alert) detallando las restricciones incumplidas:
* No se puede fabricar un motor diésel con 2300 cc.
* La pintura normal no está disponible en color azul, verde ni gris.
* El alerón deportivo solo se puede seleccionar con pintura metalizada.
* Los altavoces de gama alta solo se pueden seleccionar si se ha marcado previamente la opción de Radio-CD.
