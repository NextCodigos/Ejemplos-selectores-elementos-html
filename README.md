# Demostración: Selectores y creación dinámica de botones

Este proyecto contiene una página HTML de ejemplo que demuestra diferentes métodos para seleccionar elementos del DOM y crear botones dinámicamente usando JavaScript.

Archivo principal
- `Dom.html`: ejemplo interactivo que muestra y compara varios métodos de selección del DOM y formas de añadir botones (appendChild, innerHTML, insertAdjacentHTML, getElementById, querySelector, querySelectorAll, getElementsByClassName, getElementsByTagName, getElementsByName).

Descripción breve
- Propósito: mostrar buenas y malas prácticas para manipular el DOM y los efectos sobre los eventos y el rendimiento.
- Público objetivo: estudiantes y desarrolladores que quieran entender selectores y técnicas de inserción de elementos.

Cómo usar
- Abrir `Dom.html` directamente en un navegador moderno (Chrome, Firefox, Edge). Para una experiencia más parecida a producción, servir el directorio con un servidor HTTP simple:

```bash
# desde la carpeta DOM
python3 -m http.server 8000
# luego abrir http://localhost:8000/Dom.html
```

Qué se demuestra
- Selección: `getElementById`, `querySelector`, `querySelectorAll`, `getElementsByClassName`, `getElementsByTagName`, `getElementsByName`.
- Inserción de elementos: `appendChild` (recomendado), `innerHTML +=` (no recomendado), `insertAdjacentHTML` (buena alternativa).
- Efectos colaterales: pérdida de listeners con `innerHTML +=`, colecciones "vivas" con `getElementsByClassName`, y consideraciones de rendimiento.

Estructura del archivo
- HTML con estilos y varios bloques de demostración.
- Scripts inline que contienen funciones de prueba para cada método y botones para generar/limpiar ejemplos.

Recomendación
- Para añadir elementos dinámicos y mantener eventos, usar `createElement` + `appendChild` o `insertAdjacentHTML` según el caso.

Contribuciones
- Puedes modificar `Dom.html` directamente y probar cambios en el navegador.

Licencia
- Uso libre para aprendizaje y experimentación.
