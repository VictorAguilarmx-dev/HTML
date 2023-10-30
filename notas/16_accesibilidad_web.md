# Accesibilidad web
***

***
Esto puede ser útil para personas con discapacidad

por ejemplo
```html
<h3 role="title">Las estaciones del año</h3>
    <ul role="list">
        <li tabindex="1" role="listitem">Primavera</li>
        <li tabindex="2" role="listitem">Verao</li>
        <li tabindex="3" role="listitem">Otoño</li>
        <li tabindex="4" role="listitem">Invierno</li>
    </ul>

    <a role="link" aria-label="En este enlace encontrarás más información sobre las estaciones del año" href="#" target="blank">Más información...</a>
```