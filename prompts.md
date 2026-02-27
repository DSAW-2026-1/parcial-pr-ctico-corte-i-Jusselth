Prompt 1 (Estructura Semántica y Contenedores):
"Actúa como un desarrollador frontend senior. Necesito crear la estructura HTML básica para un componente de interfaz. Genera un contenedor principal con la clase canvas y, dentro de él, cuatro contenedores hijos, cada uno con la clase corner-group. Cada corner-group debe contener dos elementos: un div con la clase shape square y otro con la clase shape circle. Asegúrate de usar etiquetas semánticas (como main para el contenedor) y una estructura limpia que respete el flujo del documento. Cada grupo de esquina debe tener una clase única adicional para el posicionamiento (ej: top-left, top-right, etc.)."

Prompt 2 (Estilos Base, Colores y Modelo de Caja):
"Define los estilos base en un archivo style.css. Aplica un reset global con box-sizing: border-box. El contenedor principal (canvas) debe medir 400px de ancho por 300px de alto, con un fondo azul oscuro (#0a1a8e) y debe estar centrado vertical y horizontalmente en el viewport usando Flexbox en el body.
Define los estilos para las formas:

Los square deben ser cian (#61dafb) y de un tamaño fijo (ej: 50px).

Los circle deben ser rosados (#d65db1), del mismo tamaño y con border-radius: 50% para asegurar la forma circular.
Utiliza variables CSS para los colores para mejorar la especificidad y el mantenimiento."

Prompt 3 (Layout Avanzado, Posicionamiento y Refinamiento):
"El diseño final de la imagen requiere un posicionamiento preciso de los cuatro grupos y un efecto de espejo interno.

Aplica display: flex al contenedor .canvas con flex-wrap: wrap y justify-content: space-between para empujar los grupos a las esquinas izquierda y derecha.

Usa align-content: space-between para empujar los grupos a las esquinas superior e inferior.

Asegura que haya un padding interno en el contenedor (ej: 1.5rem) para que los elementos no toquen los bordes.

Lógica de Espejo: Para lograr el patrón exacto de la imagen original, los grupos de la esquina superior derecha (.top-right) e inferior izquierda (.bottom-left) deben invertir el orden de sus elementos hijos (círculo primero, luego cuadrado). Usa flex-direction: row-reverse en estos grupos específicos.

Asegura que los grupos inferiores se alineen verticalmente al final de su espacio (align-self: flex-end) para que se asienten en el fondo."