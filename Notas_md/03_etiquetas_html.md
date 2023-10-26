# Etiquetas HTML
***
- [Etiquetas `h1`-`h6`](#etiquetas-h1---h6)
- [`p`](#eqtiqueta-p)
- [Etiquetas de formato de texto](#etiquetas-de-formato-de-texto)
    - [`b`](#b)
    - [`i`](#i)
    - [`u`](#u)
    - [`sup`](#sup)
    - [`sub`](#sub)
    - [`mark`](#mark)
- [Etiquetas semánticas](#etiquetas-semánticas)
    - [`strong`](#strong)
    - [`em`](#em)
    - [`blackquote`](#blackquote)
- [Etiquetas de salto](#etiquetas-de-salto)
    - [`br`](#br)
    - [`hr`](#hr)
- [Etiquetas de formateo](#etiquetas-de-formateo)
    - [`pre`](#pre)
    - [`code`](#code)
- [Etiquetas semánticas estructurales](#etiquetas-semánticas-estructurales)
    - [`span`](#span)
    - [`div`]
    - [`header`](#header)
    - [`main`](#main)
    - [`footer`](#footer)
    - ['nav`](#nav)
    - [`article`](#article)
    - [`aside`](#aside)
    - [`section`](#section)
    - [`address`](#address)
- [Etiquetas de bloque vs Etiquetas de línea](#etiquetas-de-bloque-vs-etiquetas-de-línea)
***
## Etiquetas `h1` - `h6`
Estas etiquetas permiten titularizar nuestro contenido

```html
<h1>Encabezado nivel 1</h1>
<h2>Encabezado nivel 2</h2>
<h3>Encabezado nivel 3</h3>
<h4>Encabezado nivel 4</h4>
<h5>Encabezado nivel 5</h5>
<h6>Encabezado nivel 6</h6>
```

Tenemos unas reglas en el uso de este tipo de etiquetas.
- La etiqueta `h1` sólo se utiliza una vez en el sitio web.
- Debe de haber un orden en el uso de las etiquetas h, es decir, no se puede usar una etiqueta `h6` antes de una etiqueta `h4`.

## Eqtiqueta `p`
La etiqueta `p` se utiliza para insertar texto formateado en forma de párrafo

```html
<p>Esto es un párrafo en el cual utilizamos la etiqueta <p> de html.</p>
```

## Etiquetas de formato de texto
Estas etiquetas modifican la presentación del texto dentro de una etiqueta `p`

### `b`
La etiqueta `b` se utliza para poner en negrita una palabra o una parte de un párrafo

```html
<p>Esto es un ejemplo de una <b>palabra</b> en negrita</p>
```

### `i`
La etiqueta `i` se utliza para colocar secciones de un párrafo en letra itálica.

```html
<p>Esto es un ejemplo del uso de <i>la etiqueta </i> i para colocar el texto con una <i>letra itálica</i>.</>
```

### `u`
La etiqueta `u` se utiliza para subrallar texto en un párrafo.

```html
<p>Esto es un ejemplo de una <u>palabra</u> subrrayada con la etiqueta `u`</p>
```

### `sup`
La etiqueta `sup` sirve para colorar supraíndices, esto es util para fórmulas matemáticas.

```html
<p>La ecuación de la relatividad de Einstein es e=mc<sup>2</sup></p>
```

### `sub`
La etiqueta `sub` sirve para colocar subíndices, esto es útil para fórmulas matemáticas

```html
<p>La fórmula química del agua es: H<sub>2</sub>O<p>
```

### `mark`
La etiqueta `mark` sirve para subrayar texto como si fuera con marcatextos.

```html
<p>Este es un ejemplo del uso de la etiqueta `mark` para <mark>subrayar texto</mark></p>
```

## Etiquetas semánticas
Estas etiquetas sirven para modificar la semántica en la que se presenta un texto dentro de una etiqueta `p`

### `strong`
La etiquta `strong` la utlizamos para dar importancia a un texto.

```html
<p><strong>Este texto es importante</strong></p>
```

### `em`
La etiqueta `em` se utiliza para dar enfasis a un texto.

```html
<p><em>Este texto hace énfasis</em></p>.
```

### `blackquote`
Esta etiqueta permite hacer referencias, por ejemplo, citas bibliográficas, frases, etc...

```html
<p>
    <blockquote>Yo solo sé, que no se nada</blockquote>
    <cite>Sócrates</cite>
</p>
```

## Etiquetas de salto

### `br`
Esta etiqueta sirve para hacer saltos de línea en un párrafo

```html
<p>Esta parte del párrafo es antes del salto de línea <br> y esta parte del párrafo es despúes de señalar el salto de línea</p>
```

No hay limitantes en cuestión cuantas etiquetas `br` se pueden utilizar consecutivamente.

### `hr`
Esta etiqueta es para dividir contenido de forma semántica, se representa como una línea horizontal que divide el contenido.

```html
<h2>Encabezado h2</h2>
<p>Contenido de la sección antes de la etiqueta `hr`</p>
<hr>
<h2>Encabezado h2</h2>
<p>Contenido de la sección después de la etiqueta `hr`</p>
```

## Etiquetas de formateo

### `pre`
Sirve para señalar al navegador que respete el formato en el que escribes en el editor de código

```html
<p>
    <pre>
        - Elemento 1
            - Elemento 1.1
            - Elemento 1.2
        - Elemento 2
        - Elemento 3
    </pre>
</p>
```

### `code`
Esta etiqueta permite escribir código de un lenguaje de programación

```html
<p>
    <code>
        valores = [1, 2, 3, 4]
        for i in valores:
            print(valores)
    </code>
</p>
```

Por como es la sintaxis de html para crear código html como contenido debemos modificar el código para que respete la aparición de etiquetas, por ejemplo

```html
<p>
    <pre>
        <code>
            <body></body>
            &lt;body&gt;&lt;/body&gt;
        </code>
    </pre>
</p>
```

## Etiquetas semánticas estructurales
Estas etiquetas nos permiten maquetar un sitio web así como para seccionar el contenido del sitio.

### `span`
Esta es una etiqueta contenedora en línea que no tiene semántica, sirve para seccionar los elementos en una misma línea de contenido

```html
<span></span>
```

### `div`
Es una etiqueta contenedora en bloque que no tiene semántica, sirve para seccionar los elementos de un sitio web.

```html
<div></div>
```

### `header`
Representa la cabecera de un sitio web o de una sección

```html
<header></header>
```

### `main`
Define la sección principal del documento, solo puede existir una etiqueta `main` por documento.

```html
<main></main>
```

### `footer`
Representa el pié de página de un sitio web o de una sección.

```html
<footer></footer>
```

### `nav`
Representa una navegación, en esta etiqueta se coloca el menú de navegación del sitio.

```html
<nav></nav>
```

### `article`
Representa una sección de autocontenido (que por sí sola se explica.), por ejemplo en un blog de noticias el lugar donde va una noticia se colocaría en una etiqueta `article`

```html
<article></article>
```

### `aside`
Representa contenido complementario o secundario, por ejemplo, en un sitio de noticias podemos crear una parte de noticias similares o noticias sugeridas, o poner publicidad en esta etiqueta.

```html
<aside></aside>
```

### `section`
Representa una sección de contenido genérico.

```html
<section></section>
```

### `address`
Representa una información de contacto.

```html
<address></address>
```

## Etiquetas de bloque vs Etiquetas de línea
Una etiqueta de bloque es aquella que genera saltos de línea con sus etiquetas hermanas. Podemos ver a las etiquetas de bloque como aquellas que utilizan todo el espacio disponible del viewport

Algunas etiquetas de bloque son las siguientes:
    - `h1` - `h6`
    - `p`
    - Etiquetas semánticas estructurales excluyendo `span`

Una etiqueta de línea es aquella que sólo ocupa el espacio necesario que tiene su contenido, no generan saltos de línea por arriba o por debajo de ella

Algunas etiquetas de línea son las siguientes:
    - `span`
    - Etiquetas de formato de texto
    - Etiquetas semánticas de 
    - enlases
    - imágenes
    - videos