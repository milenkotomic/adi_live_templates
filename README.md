# Instalacion en PhpStorm

1. Abrir PhpStorm Preferences (o Settings) | Tools | Settings Repository
2. Agregar a Read-only Source la URL del repositorio <https://github.com/milenkotomic/adi_live_templates/>
3. Reiniciar PhpStorm

Para más info: <https://www.jetbrains.com/help/phpstorm/using-live-templates.html>

# Live Templates para PHP 
## ninc
Crea una nueva clase con los metodos get y upd con la estructura habitual

## nweb
Código base de un archivo web con la inclusion del config y el llamado a KERNEL::render

# Inyección de funciones de HTML lib 
## ajaxcompletar

## calendario

## checkbox

## file

## inctem
```HTML
<!-- include( template( '../template/$END$.html' ) ); -->
```

## numero
Input text con class numero

## rut
Input text con class rut

## select

## tabs

## text
Input text sin clase

## textarea

# Live Templates para HTML
## buscador

## da
```HTML
<a class="file pdf" href="" target="">Nombre Archivo</a><em>Tamaño</em>
```

## ftable
Formulario estilo tabla con dos columnas, nombre del campo y campo

## h1

## h2

## nsortable
Tabla para desplagar elementos, inlcuye sortable, search y sticky.
Por defecto, utiliza la variable `$iterable` como el arreglo a recorrer, `$id` como llave del objeto y `$object` como el objeto.

## persona
Inlcuye la foto, nombre y rut de una persona.
Por defecto, utiliza la variable `$persona`.

## req
Agrega `class="req"`

## sep
Agrega una fila de tabla con clase `separador` y `colspan=0`

## tabla
Lo mismo que `nsortable`

## tn
Agrega una cabezera de tabla con clase `number`

## trf
Agrega una fila a una tabla formulario.
```HTML
<tr>
    <th class="string">^^</th>
    <td>{HTML::text( '', $valor , $placeholder ) }</td>
</tr>
```

## trq
Igual que `trf` incluyendo el `class="req"` al `tr`

## ts
Agrega una cabezera de tabla con clase `string`

## ttr
Agrega una fila de tabla con `th` y `td`

# Live Templates para PHP

## les
```PHP
$link->escapeSimple( );
```

## odk
Dado el nombre de un campo de la base de datos, entrega el string que forma parte de `on duplicate key update`. Por ejemplo: 
`PERS_ID` se transforma en `PERS_ID = values( PERS_ID )`
