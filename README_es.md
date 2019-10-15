## Descargo de responsabilidad de crédito ##

Este proyecto es un tenedor. Echa un vistazo al [Repo principal](https://github.com/senchalabs/cssbeautify) .


# CSS Beautify #

CSS Beautify es una implementación de JavaScript de reindenter y reformatter para estilos escritos en [CSS](http://www.w3.org/Style/CSS/).

Dado el siguiente estilo:

```css
menu{color:red} navigation{background-color:#333}
```

CSS Beautify producirá:

```css
menu {
    color: red
}

navigation {
    background-color: #333
}
```

Pruébelo en línea en [cssbeautify.com](http://cssbeautify.com). Para el uso de la línea de comandos, instale el paquete Node.js [cssbeautify](https://npmjs.org/package/cssbeautify).

Para más ejemplos, vea también su [conjunto de pruebas](http://cssbeautify.com/test/).




## Usando la función cssbeautify() ##

Como CSS Beautify está escrito en puro JavaScript, puede ejecutarse en cualquier lugar que JavaScript pueda ejecutar.

El API es muy sencillo:

```javascript
var resultado = cssbeautify(estilo, opciones);
```

**opciones** es un objecto opcional para ajustar el formato. Opcionas conodicas hasta ahora son:

  *  <code>indent</code> (indentación) es una cadena utilizada para la indentación de la declaración (el valor predeterminado es 4 espacios)
  *  <code>openbrace</code> (llave de apertura) define la ubicación de la llave abierta, ya sea * fin de línea * (predeterminado) o * línea separada *.
  *  <code>autosemicolon</code> (punto y coma automático) siempre inserta un punto y coma después del último conjunto de reglas (el valor predeterminado es * false *)

Llamada de ejemplo:

```javascript
var beautified = cssbeautify('menu{opacity:.7}', {
    indent: '  ',
    openbrace: 'separate-line',
    autosemicolon: true
});
```

## Contribuyendo ##

¡Las contribuciones son bienvenidas! Por favor lea la [Guía de Contribución](https://github.com/AmirMehrabi/cssstyler/blob/master/CONTRIBUTING.md) for more info.

## Licencia ##

Copyright (C) 2012 Sencha Inc.
Copyright (C) 2011 Sencha Inc.

Por la presente se otorga permiso, sin cargo, a cualquier persona que obtenga una copia
de este software y los archivos de documentación asociados (el "Software"), para tratar
en el Software sin restricción, incluidos, entre otros, los derechos
para usar, copiar, modificar, fusionar, publicar, distribuir, sublicenciar y / o vender
copias del Software y para permitir a las personas a quienes pertenece el Software
amueblado para hacerlo, sujeto a las siguientes condiciones:

El aviso de copyright anterior y este aviso de permiso se incluirán en
todas las copias o partes sustanciales del Software.

EL SOFTWARE SE PROPORCIONA "TAL CUAL", SIN GARANTÍA DE NINGÚN TIPO, EXPRESA O
IMPLÍCITO, INCLUYENDO PERO NO LIMITADO A LAS GARANTÍAS DE COMERCIABILIDAD,
APTITUD PARA UN PROPÓSITO PARTICULAR Y NO INFRACCIÓN. EN NINGÚN CASO EL
LOS AUTORES O LOS TITULARES DE LOS DERECHOS DE AUTOR SERÁN RESPONSABLES POR CUALQUIER RECLAMACIÓN, DAÑO U OTRO
RESPONSABILIDAD, EN CASO DE ACCIÓN DE CONTRATO, TORTURA O DE OTRA MANERA, DERIVADA DE,
FUERA DE O EN CONEXIÓN CON EL SOFTWARE O EL USO U OTRAS OFERTAS EN
EL SOFTWARE.
