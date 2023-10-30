# Enlaces
***
## Índice
- [Etiqueta `a`](#etiqueta-a)
- [Imágenes y Vectores](#imágenes-y-vectores)
- [Enlaces internos](#enlaces-internos)
- [Protocolos especiales](#protocolos-especiales)
***
## Etiqueta `a`
Un enlace es un elemento que nos permite interactuar con diversor archivos en que conforman nuestro sitio

Para esto utilizamos la etiqueta `a`

```html
<a href="ruta">Texto</a>
```

El atributo `href` permite ir hacia otra instancia, en este atributo podemos poner:
    - ruta hacia otro docmento html
```html
<a href="login.html">Ingresar</a>
```
    - enlaces externos
```html
<a href="https://google.com">google.com</a>
```

En caso de enlaces externos es recomendable utilizar el atributo `target` esto para abrir el sitio del enlace en otra pestaña.

```html
<a href="https://google.com" target="_black">google.com</a>
```

De igual forma en enlaces externos se recomienda el uso del atributo `rel` con el valor de `nofollow` para indicarle al navegador que el sitio que se dirige no forma parte del sitio web.

```html
<a href="https://google.com" target="_black" rel="nofollow">google.com</a>
```

## Imágenes y Vectores
También podemos utilizar la etiqueta `a` para colocar imágenes o vectores.

```html
<a href="https://google.com" target="_blank"><img src="img/img.svg"></a>
```

## Enlaces internos
Estos son útiles cuando queremos hacer índices dentro de nuestro sitio, en este caso es importante el uso del caracter `#` en el atributo `href`

```html
<ul>
    <li><a href="index.html#cap1"></a></li>
    <li><a href="index.html#cap2"></a></li>
    <li><a href="index.html#cap3"></a></li>
</ul>
```

El caracter `#` se suele marcar como una sección dentro de nuestro sitio, por ejemplo, en el primer enlace interno podemos leer la propiedad `href` de la siguiente forma:

**sección *cap1* del sitio *index.html***

Además si queremos utilizar enlaces internos es importante identificar cada sección a la cual queremos enlazar, para esto utilizamos el atributo `id` en cada inicio de sección

```html
<h2 id="cap1">Capítulo 1</h2>
<h2 id="cap2">Capítulo 2</h2>
<h2 id="cap3">Capítulo 3</h2>
```

## Protocolos especiales
Estos protocolos sirver para una mejor interacción con el cliente, se necesita una configuración previa el usuario o dueño del sitio.

- Correo Electrónico
```html
<a href="correo@gmail.com">Enlace a correo electrónico</a>
```

- Teléfono
```html
<a href="tel:5212345678">Enlace a teléfono</a>
```

- Whatsapp
```html
<a href="https://api.whatsapp.com/send?phone=521234567890&&text=Hola">Enlace hacia WhatsApp</a>>
```

