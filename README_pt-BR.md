## Aviso de crédito ##

Este projeto é uma ramificação (fork). Dê uma olhada no [repositório principal](https://github.com/senchalabs/cssbeautify).


# CSS Beautify #

CSS Beautify é uma implementação em JavaScript do reindentador e reformatador para estilos escritos em [CSS](http://www.w3.org/Style/CSS/).

Dado o seguinte estilo:

```css
menu{color:red} navigation{background-color:#333}
```

CSS Beautify irá produzir:

```css
menu {
    color: red
}

navigation {
    background-color: #333
}
```

Experimente-o online em [cssbeautify.com](http://cssbeautify.com). Para uso em
linha de comando, instale o pacote para Node.js [cssbeautify](https://npmjs.org/package/cssbeautify).

Para mais exemplos, veja também a [suíte de testes](http://cssbeautify.com/test/).




## Usando a função cssbeautify() ##

Como o CSS Beautify é escrito em JavaScript puro, ele pode ser executado em qualquer lugar onde o JavaScript possa ser executado.

A API é muito simples:

```javascript
var resultado = cssbeautify(estilo, opcoes);
```

**opcoes** é um objeto opcional para ajustar a formatação. As opções conhecidas até agora são:

  *  <code>indent</code> (indentação) é uma string usada para a indentação da declaração (o padrão é 4 espaços)
  *  <code>openbrace</code> (chave de abertura) define onde são colocadas as chaves de aberturas, que pode ser *end-of-line* (fim de linha, padrão) ou *separate-line* (linha separada).
  *  <code>autosemicolon</code> (ponto-e-vírgula automático) sempre insere um ponto-e-vírgula depois da última regra (o padrão é *false*).

Chamada de exemplo:

```javascript
var beautified = cssbeautify('menu{opacity:.7}', {
    indent: '  ',
    openbrace: 'separate-line',
    autosemicolon: true
});
```

## Contribuições ##

Contribuições são bem-vindas! Por favor, leia o [Guia de Contribuições](https://github.com/AmirMehrabi/cssstyler/blob/master/CONTRIBUTING.md) para mais informações.

## Licença ##

Copyright (C) 2012 Sencha Inc.
Copyright (C) 2011 Sencha Inc.

A permissão é concedida, gratuitamente, a qualquer pessoa que obtenha uma cópia
deste software e arquivos de documentação associados (o "Software"), para lidar com
no Software sem restrição, incluindo sem limitação os direitos
usar, copiar, modificar, fundir, publicar, distribuir, sublicenciar e/ou vender
cópias do Software, e para permitir que as pessoas a quem o Software se destina
fornecidos para o efeito, sob reserva das seguintes condições:

O aviso de direitos autorais acima e este aviso de permissão devem ser incluídos em
todas as cópias ou partes substanciais do Software.

O SOFTWARE É FORNECIDO "TAL COMO ESTÁ", SEM GARANTIA DE QUALQUER TIPO, EXPRESSA OU
IMPLÍCITO, INCLUINDO, MAS NÃO LIMITADO ÀS GARANTIAS DE COMERCIABILIDADE,
ADEQUAÇÃO A UM FIM ESPECÍFICO E NÃO INFRAÇÃO. EM CASO ALGUM PODERÁ A
OS AUTORES OU DETENTORES DE DIREITOS DE AUTOR SÃO RESPONSÁVEIS POR QUALQUER RECLAMAÇÃO, DANOS OU OUTROS
RESPONSABILIDADE, SEJA NUMA AÇÃO POR CONTRATO, ATO ILÍCITO OU DE OUTRA FORMA, RESULTANTE DE,
FORA DE OU EM CONEXÃO COM O SOFTWARE OU O USO OU OUTRAS TRANSAÇÕES EM
O SOFTWARE.