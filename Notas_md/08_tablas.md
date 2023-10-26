# Tablas
***
## Índice
- [Tablas básicas](#tablas-básicas)
- [Tablas agrupando renglones](#tablas-agrupando-renglones)
- [Combinar celdas](#combinar-celdas)
- [Alinear celdas](#alinear-celdas)
***
## Tablas básicas
Para crear una tabla utilizamos la etiqueta `table`. Junto con esta etiqueta para crear una tabla básica necesitamos otras 2 etiquetas para llenar la tabla
    - `tr` --> indica el renglón de la tabla.
    - `td` --> indica el dato de la celda de la tabla.

```html
<table>
    <tr>
        <td>Nombre</td>
        <td>País</td>
    </tr>
    <tr>
        <td>Mole</td>
        <td>México</td>
    </tr>
    <tr>
        <td>Hot Dogs</td>
        <td>Estados Unidos</td>
    </tr>
    <tr>
        <td>Café Turco</td>
        <td>Turquía</td>
    </tr>
</table>
```
## Tablas agrupando renglones
Podemos agrupar filas con las siguientes 3 etiquetas
    - `thead` --> Dentro de esta etiqueta colocaremos los encabezados de la tabla, junto con esta etiqueta utilizamos la etiqueta `th` para remplazar la etiqueta `td` en el contenido.
    - `tbody` --> Dentro de esta etiqueta escribiremos el contenido de la tabla.
    - `tfoot` --> El funcionamiento de esta etiqueta es similar a la etiqueta `thead`, sólo que que coloca al final de la tabla, en esta etiqueta utilizamos la etiqueta `td` para añadir el contenido.

```html
<table>
    <thead>
        <tr>
            <th>Nombre</th>
            <th>País</th>
        </tr>
    </thead>
    <tbody>
        <tr>
            <td>Mole</td>
            <td>México</td>
        </tr>
        <tr>
            <td>Hot Dogs</td>
            <td>Estados Unidos</td>
        </tr>
        <tr>
            <td>Café Turco</td>
            <td>Turquía</td>
        </tr>
    </tbody>
    <tfoot>
    </tfoot>
</table>
```
## Combinar celdas
Podemos combinar celdas por columna o por renglón por medio de atributos en nuestra tabla
    - `colspan` --> combina celdas por columna.
    - `colrow` --> combina celdas por renglón.

```html
<table>
    <thead>
        <tr colspan="2">
            Comidas por Internacionales
        <tr>
            <th>Nombre</th>
            <th>País</th>
        </tr>
    </thead>
    <tbody>
        <tr>
            <td>Mole</td>
            <td>México</td>
        </tr>
        <tr>
            <td>Hot Dogs</td>
            <td>Estados Unidos</td>
        </tr>
        <tr>
            <td rowspan="2">Café</td>
            <td>México</td>
        </tr>
        <tr>
            <td>Etiopía</td>
        </tr>
    </tbody>
    <tfoot>
    </tfoot>
</table>
```
## Alinear celdas