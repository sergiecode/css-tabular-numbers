![tabular nums](https://raw.githubusercontent.com/sergiecode/css-tabular-numbers/master/tabular-numbers.jpg)

# Tutorial de CSS: Tabular Nums

Este tutorial te guiará a través del uso de la propiedad CSS `font-variant-numeric` con el valor `tabular-nums` para mostrar números en formato de tablas. Verás cómo aplicar esta propiedad a un conjunto de números en un párrafo y lograr que se muestren de manera alineada y legible.

## HTML

El código HTML que utilizaremos en este tutorial es el siguiente:
```
<body class="container">
    <div class="container2">
        <div class="tabular-nums">
            <p>$312.000.659</p>
            <p>$124.010.010</p>
            <p>$251.111.111</p>
        </div>
    </div>
</body>
```

Aquí tenemos un elemento `div` con la clase `"container2"` que contiene otro elemento `div` con la clase `"tabular-nums"`. Dentro de este último div, hay tres elementos `p` que contienen números de ejemplo con un formato de dinero.

## CSS

Agregaremos estilos CSS para lograr el efecto deseado:
```
.container {
    margin: 5px;
    padding: 5px;
    font-family: cursive;
}

.container2 {
    padding: 7px;
    width: 130px;
    height: 130px;
    text-align: end;
    border: 1px black solid;
}

.tabular-nums {
    font-variant-numeric: tabular-nums;
}
```

Aquí hemos definido algunas reglas CSS:

-   En la clase `.container`, establecemos márgenes, relleno y una fuente cursiva para el cuerpo del documento.
    
-   En la clase `.container2`, establecemos un relleno, un ancho y un alto fijos, alineamos el texto a la derecha (`text-align: end`) y agregamos un borde negro sólido de 1 píxel.
    
-   En la clase `.tabular-nums`, utilizamos la propiedad `font-variant-numeric` con el valor `tabular-nums` para aplicar el formato de números tabulares a los elementos de texto dentro de este contenedor. Esto garantizará que los números se muestren alineados correctamente y sean más fáciles de leer.
