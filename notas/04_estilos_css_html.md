# Estilos de CSS en HTML
Tenemos tres formas de dar estilos a nuestra página desde un documento html

## Propiedad `style`
Esta propiedad se coloca después del nombre de la etiqueta que queremos usar, por ejemplo:

```html
<div style="blackground-color = green"></div>
```
## Etiqueta `style`
En esta etiqueta la escribiremos dentro de la etiqueta `head` de nuestro documento y en ella pondremos todos los estilos de nuestro sitio.

```html
<head>
    <style>
        h2{
            color:orangered;
        }
    </style>
</head>
```

## Archivo css
Se crea una carpeta llamada `styles` y en ella crearemos todos los archivos necesarios de estilos con el siguiente formato:
```
nombre_archivo.css
```
para ver reflejado los estilos en nuestro archivo de estilos utilizamos la etiqueta `link` dentro del `head`
```html
<head>
    <link rel='stylesheet', href='./styles/nombre_archivo.css'>
</head>
```