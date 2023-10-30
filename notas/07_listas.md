# Listas
***
## Índice
- [Listas ordenadas](#listas-ordenadas)
- [Listas no ordenadas](#listas-no-ordenadas)
- [Listas de definición](#listas-de-definición)
***
## Listas ordenadas
Para escribir una lista ordenada necesitamos de dos etiquetas
    - La etiqueta `ol` que especifica una lista ordenada
    - La etiqueta `li` la cual especifica un miembro de la lista.


```html
<ol>
    <li>Primavera</li>
    <li>Verano</li>
    <li>Otoño</li>
    <li>Invierno</li>
</ol>
```

La etiqueta `ol` tiene algunos atributos interesantes

- Si queremos iniciar la lista en un número en específico escribimos el atributo `start`

```html
<ol start="3">
    <li>Primavera</li>
    <li>Verano</li>
    <li>Otoño</li>
    <li>Invierno</li>
</ol>
```

- Si queremos tener una lista en el orden inverso agregamos el atributo `reversed`

```html
<ol reversed>
    <li>Primavera</li>
    <li>Verano</li>
    <li>Otoño</li>
    <li>Invierno</li>
</ol>
```

- Modificar la enumeración de la lista agregamos el atributo `type`

```html
<ol type="A">
    <li>Primavera</li>
    <li>Verano</li>
    <li>Otoño</li>
    <li>Invierno</li>
</ol>
```

este atributo puede recibir los siguientes valores
    - "a" --> letras minúsculas.
    - "A" --> letras mayúsculas.
    - "i" --> números romanos en minúsculas.
    - "I" --> números romanos en mayúsculas.
    - "1" --> números arábigos (valor default).

## Listas no ordenadas
Para agregar una lista no ordenada en nuestro sitio utilizamos la etiqueta `ul`

```html
<ul>
    <li>Terminar de estudiar</li>
    <li>Ir al gimnasio</li>
    <li>Lavar ropa</li>
    <li>Ir a comprar café</li>
</ul>
```

Al igual que en las listar ordenadas tenemos atributos que le podemos agregar una lista no ordenada.

- Para modificar la viñeta utilizamos el atributo `type`

```html
<ul type="circle">
    <li>Terminar de estudiar</li>
    <li>Ir al gimnasio</li>
    <li>Lavar ropa</li>
    <li>Ir a comprar café</li>
</ul>
```

tenemos tres tipos de viñetas disponibles
    - circle
    - square
    - disc

## Listas de definición
No se utilizan habitualmente, pero las podemos utilizar en glosarios o índices alfabéticos.

En este tipo de listas necesitamos 3 etiquetas diferentes
    - `dl` --> señala el tipo de lista, en este caso de definición.
    - `dt` --> señala el término que queremos definir
    - `dd` --> señala la definición del termino que queremos definir

```html
<dl>
    <dt>HTML</dt>
    <dd>Es un lenguaje de marcado que define el contenido de la web.</dd>
    <dt>CSS</dt>
    <dd>Es un lenguaje de definición que da estilos al código HTML.</dd>
    <dt>JavaScript</dt>
    <dd>Es el lenguaje de la web.</dd>
</dl>
```