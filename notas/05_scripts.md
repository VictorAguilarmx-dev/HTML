# Scripts en HTML
En HTML tenemos dos formas diferentes de escribir código JavaScript en nuestro documento

## Etiqueta `script`
Gracias a la etiqueta `script` podemos escribir código JS dentro del docuemento.

Se recomienda colocar esta etiqueta al final de la etiqueta body

```html
<body>
    <h1>Ejemplo del uso de la etiqueta `script`</h1>
    <div>La etiqueta `script` se coloca al final de la etiqueta `body`</div>
    <script>console.log("hola estamos aprendiendo html")</script>
</body>
```

## Archivo .js
Se crea una carpeta llamada `assets` y en ella crearemos todos los archivos necesarios de scripts JS con el siguiente formato:
```
nombre_archivo.js
```
para ver reflejado los estilos en nuestro archivo de estilos utilizamos la etiqueta `script` con el atributo `src` dentro del `body`
```html
<head>
    <script src='./assets/nombre_archivo.js></script>
</head>
```