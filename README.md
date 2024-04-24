# learn-css
Repositorio para aprende CSS desde cero

CSS (Cascade StyleSheets) significa *hoja de estilos en cascada* y es el lenguaje usado para colocar formato de estilos en los elementos de HTML.

No solo sirve para web, también se puede usar para colocar los estilos de otros medios como:

- Impresión
- Diseños gráficos
- Etc.

## ¿Por qué CSS?

- HTML nunca se diseño para colocar estilos en las webs.
- La tendencia de etiquetas para estilos (`font`, `center`, ...) se abandonó.
- Se usa CSS para colocar los estilos de las webs:

![alt text](image.png)

Ejemplo de sintaxis CSS aplicado a un `<p>`:

```css
  p {
    color: red;
    text-align: center;
  }
```

Prioridad de Cascada

- Selectores más específicos tienen prioridad y 
- Selectores que aparecen "después" (más abajo en el `.css`) ante igualdad de condiciones tienen prioridad:

```css
  p {
    color: red;
  }
  /* Este tiene prioridad para los de la clase "clase": */
  p.clase {
    color:green;
  }
```

```css
  h1 { color: tomato; }
  ... varias líneas después ...
  /* Este mismo selector sobreescribe al anterior: */
  h1 { color: red; }
```

Además: 

- `Inline` tiene máxima prioridad
- `External` e `internal` > estilos por defecto del navegador

---

Contenido basado en el itinerario de CSS de W3Schools: https://www.w3schools.com/css/default.asp