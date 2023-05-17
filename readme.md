# Flex CSS

Responsividade para todo o CSS, não apenas para a grid.

Esqueça media query.

### Defina seus prefixos e tamanhos

```Javascript

const sizes1 = [
    { prefix: 's-', minSize: 0 },
    { prefix: 'm-', minSize: 500 },
    { prefix: 'l-', minSize: 1000 }
];

const sizes2 = [
    { prefix: 'xs-', minSize: 0 },
    { prefix: 's-', minSize: 433 },
    { prefix: 'm-', minSize: 733 },
    { prefix: 'l-', minSize: 1000 },
    { prefix: 'xl-', minSize: 1333 }
];

```

### Controle a aplicação de suas classes CSS por prefixos

```CSS

.xs-panel {width: 100%}
.m-panel {width: 50%}
.l-panel {width: 33%}

.xs-span {
    text-align: left;
    color: black;
}
.m-span {
    text-align: center;
    color: blue;
}

```

### Como usar

```Javascript

// Simplesmente chame esta função no final do seu index.html
processFlexCSS(sizes);

```
