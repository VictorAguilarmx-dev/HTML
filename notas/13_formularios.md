# Formularios
***
## Índice
- [Elementos de Formularios](#elementos-de-formularios)
    -[Input](#input)
    -[Textarea](#textarea)
    -[Listas](#listas)
- [Atributos de Inputs y Formularios](#atributos-de-inputs-y-formularios)
***

Los formularios permiten la interactividad entre el usuario y el sitio web.

Para agregar un formulario utlizamos la etiqueta `form`.
```html
<form>

</form>
```
Esta etiqueta es una etiqueta de bloque.

## Elementos de Formularios

### Input
Este elemento es el más básico dentro de un formulario y es un elemento de línea.

```html
<input type = "tipo">
```
dentro de este elemento tenemos diferentes tipos de input
    - `text` --> texto
```html
<input type = "text">
```

- `checkbox` --> permite seleccionar opciones más de una vez.
```html
<input type = "checkbox">
```
- `radio` --> Permite seleccionar una opcción entre muchas.
```html
<input type = "radio">
```
- `date` --> calendario
```html
<input type = "date">
```
- `color` --> genera un picker de colores.
```html
<input type = "color">
```
- `button` --> botón, en este caso es importante el uso de la propiedad `value` para agregar texto al botón
```html
<input type = "button" value="Botón">
```
- `submit` --> botón que envía los datos del formulario.
```html
<input type = "submit">
```
- `reset` --> botón que limpia los valores que hemos introducido en el formulario.
```html
<input type = "reset">
```
- `file` --> permite que el usuario pueda elegir un archivo para poder subirlo al servidor. Para que el usuario pueda seleccionar multiples archivos se utiliza la propiedad `multiple`
```html
<input type = "file">
<input type = "file" multiple>
```
- `hiden` --> sirven para que que el desarrollador pueda mandar un valor una vez que el usuario envíe datos.
```html
<input type="hiden" name="idioma" value="es">
```
- `email` --> sirve para introducir emails, en dispositivos tactiles modifica el teclado tactil para agregar caracteres especiales de los emails
```html
<input type="email">
```
- `number` --> sirve para ingresar números, aparece un teclado numérico.
```html
<input type="number">
```
- `tel` --> sirve para ingresar números telefónicos, aparece un teclado de celular.
```html
<input type="tel">
```
- `password` --> sirve para agregar contraseñas, al escribir en este tipo de `input` por default el pasword aparece oculto por medio de bulets
```html
<input type="password">
```
- `search` --> sirve para hacer búsquedas 
```html
<input type="search">
```
Por default este elemento tiene el tipo `text`

### Label
La etiqueta `label` sirve para poner un texto a un lado de un `imput`, esto es de gran utilidad para ayudar a identificar los elementos de un formulario.
```html
<label for="">Usuario</label>
```

### Textarea
Es elemento del formulario que permite ingresar texto, es util para que el usuario pueda escribir comentarios.
```html
<textarea cols="30" rows="10"></textarea>
```

### Listas
Podemos agregar listas desplegables a nuestros formularios.
```html
<select name="" id="">
    <option value="">HTML</option>
    <option value="">CSS</option>
    <option value="">JS</option>
    <option value="">PHP</option>
    <option value="">Python</option>
</select>
```
Por default este tipo de elemento solo permite la selección de una opción, pero podemos agregar el atributo multiple para seleccionar mas de una opción.
```html
<select name="" id="" multiple>
    <option value="">HTML</option>
    <option value="">CSS</option>
    <option value="">JS</option>
    <option value="">PHP</option>
    <option value="">Python</option>
</select>
```

## Atributos de Inputs y Formularios
- `id` --> Este atributo define un identificador único el cual no debe de repetirse en todo el documento
```html
<form id="formulario_login">
    <input id="usuario">
</form>
```

- `readonly` --> Sirve para volver un input de solo lectura, es decir el usuario no podrá modificar su contenido.
```html
<input type="text" value="Víctor" readonly>
```

- `desabled` --> Sirve para desabilitar inputs, este atributo es útil para inputs con el atributo `readonly`, además este atributo cambia el estilo del input.
```html
<input type="text" value="Víctor" readonly disabled>
```

- `placeholder` --> Sirve para mandar mensajes por default, por lo general se utiliza para dar instrucciones de uso al usuario del input.
```html
<input type="text" placeholder="Escribe tu nombre">
```

- `action` --> este atributo es exclusivo de la etiqueta `form` el valor de este atributo señala el lugar en donde se envía la información del formulario
```html
<form action="https://victor.com/">

</form>
```

- `name` --> Es para dar nombre a la variable generada al ingresar los datos.
```html
<input type="text" name="usuario">
```

- `method` --> Define con qué método HTTP se envían los datos. Tiene dos posibles valores.
    - `GET` --> valor por defecto
    - `POST` --> Se envía de forma ‘‘oculta’’

```html
<form action="https://victor.com/" mathod="GET"> 
<form action="https://victor.com/" mathod="POST"> 
```
Es recomendable siempre utilizar el método `action` con este método.

Si no se utiliza el método `action` el formulario el formulario se estaría autoprocesando

Usualmente el manejo y envío de formularios se maneja con JS

- `autocomplete` --> permite el autocompletado del formulario. Tiene dos posibles valores
    - `on`
    - `off`
```html
<form autocomplete="on">
<form autocomplete="off">
<input type="text" name="email" autocomplete="off">
```

Este atributo se puede utilizar en la etiqueta `form` o en un `input` independiente.

- `for` --> este atributo aparece con la etiqueta `label` y hace referencia al atributo `id` de la etiqueta `input`, es decir vincula la etiqueta `label` con su respectivo `input`
```html
<label for="usuario">Usuario</label>
<input type="text" name="usuario" id="usuario">
```

- `required` --> Este atributo hace obligatorio el llenado del `input` que tenga este método
```html
<input type="password" required>
```

- `pattern` --> Sirve para colocar un patron de verificación de un `input`, en este método se utilizan expresiones regulares

```html
<input pattern="^[A-Za-z]+$">
```

- `title` --> Este permite agregar un mensaje de validación en el `input`

```html
<input title="El campo solo acepta letras" patter="^[A-Za-z]+$">
```

- `value` --> Este permite dar un valor por defecto al input o botón.

```html
<button value="click on me">
```

- `multiple` --> Permite elegir más de una opción en un `input` tipo lista.

- `selected` --> Da un valor por defecto en un `input` tipo lista


## Ejemplo de Formularios
### Formulario Login
```html
<form action="https://victor.com/" method="POST" autocomplete="off">
    <label for="usuario">Usuario</label>
    <input type="text" name="usuario" id="usuario" placeholder="Escribe tu usuario" patter="^[A-Za-z]+$" title="El campo solo acepta letras" required>
    <br>
    <label for="password">Contraseña</label>
    <input type="password" name="password" id="password" placeholder="Escribe tu password" required>
    <br>
    <input type="submit">
    <br>
    <input type="reset">
</form>
```
## Selects Radios y Checkbox
```html
<form>
    <p>Elige tu idioma</p>
    <select name="idioma" required>
        <option value="">Elige una opción</option>
        <option value="es" selected>Español</option>
        <option value="en">Inglés</option>
        <option value="fr">Frances</option>
        <option value="it">Italiano</option>
        <option value="pt">Portugués</option>
    </select>
    <p>Elige tu lenguaje de programación favorito</p>
    <input type="radio" name="lenguaje" id="radio-js" value="js" required>
    <label for="radio-js">JavaScript</label>
    <input type="radio" name="lenguaje" id="radio-py" value="py" checked>
    <label for="radio-py">Python</label>
    <input type="radio" name="lenguaje" id="radio-php" value="php">
    <label for="radio-php">PHP</label>
    <p>Elige tus intereses</p>
    <label>
        <input type="checkbox" name="intereses-deportes" value="deportes" checked>
        Deportes
    </label>
    <label>
        <input type="checkbox" name="intereses-finanzas" value="finanzas">
        Finanzas
    </label>
    <label>
        <input type="checkbox" name="intereses-salud" value="salud">
        Salud
    </label>
    <label>
        <input type="checkbox" name="intereses-politica" value="politica">
        Política
    </label>
    <label>
        <input type="checkbox" name="intereses-ecologia" value="ecologia" ckecked>
        Ecología
    </label>
    <label>
        <input type="checkbox" name="terminos" required>
        ¿Acepta términos y condiciones?
    </label>
    <input type="submit">
    <input type="reset">
</form>
```
## Formulario de contacto
```html
<form action="https://formsubmit.co/victor.aguilar.dev97@gmail.com" method="post">
    <input type="text" name="nombre" placeholder="Escribe tu nombre" pattern="^[A-Za-ZÑNÁáÉéÍíÓóÚúÜü\s]+$" title="Nombre sólo acepta letras y espacios en blanco" required>
    <br>
    <input type="email" name="correo" placeholder="Escribe tu correo" pattern="^(\w+[/./-]?){1,}@[a-z]+[/.]\w{2,}$" title="Formato de correo inválido" required>
    <br>
    <textarea name="comentarios" cols="30" rows="10" required></textarea>
    <br>
    <input type="submit">
</form>
```

