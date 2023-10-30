# Meta etiquetas para SEO

- `title` --> Esta nos permite colocar un nombre a nuestro sitio, este aparecerá en el buscador. Se recomienda utilizar entre 55 y 65 caracteres.
```html
<title>Título de nuestro sitio</title>
```
- `description` --> Podemos colocar una breve descripcción sobre nuestro sitio, es util para posicionar nuestro sitio por la forma de como busca sitios el buscador de preferencia. Se recomienda utilizar no más de 165 caracteres.
```html
<meta name="description" content="Descripción de ejemplo para ver el funcionamiento de el atributo description">
```
- `canonical` --> Permite decirle a los motores de busqueda cual es url principal de un conjunto de url con el mismo tema, por ejemplo en una tienda en línea tenemos una página de un producto y otra página con alguna promoción, entonces nuestra url canónica sería la url de nuestra página sin la promo ya que a partir de esta se crea la página con la promo.
```html
<link rel="canonical" href="http://tudominio.com/la-url-canonica">
```

- `icon` --> Permite agregar una imágen en formato png en las pestañas de los navegadores
```html
<link rel="icon" href="img/favicon.png">
```
- `theme-color` --> Permite cambiar el color de la pestaña de nuestro sitio
```html
<meta name="theme-color" content="#ffffff">
```
- `og` --> Permiten una mejor presentación de nuestro sitio en post en redes sociales
```html
<meta property="og:title" content="og:título del sitio">
<meta property="og:description" content="og:descripcción del sitio">
<meta property="og:image" content="https://tudominio.com/img/imagen.png">
<meta property="og:url" content="https://tudominio.com/index.html">
<meta name="twitter:card" content="sumary">
```