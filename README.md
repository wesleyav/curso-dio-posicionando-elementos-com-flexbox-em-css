# Posicionando elementos com Flexbox em CSS
Repositório com o material do curso Posicionando elementos com Flexbox em CSS da DIO.


## Introdução ao Flex Box

### Flex Container
`flex container` é a tag que envolve os itens, será nela que iremos aplicar a propriedade "display:flex". Transforma seus itens filhos em flex itens.

Propriedades relacionadas:

* display
* flex-direction
* flex-wrap
* flex-flow
* justify-content
* align-itens
* align-content

### Flex Item
`flex item` são os elementos filhos diretos do Flex Container. E também podem se tornar Flex Container.

Propriedades relacionadas:

* flex-grow
* flex-basis
* flex-shrink
* flex
* order
* align-self

## Fundamentos do Flex Box - Parte 1

### Estrutura básica do display:flex

Sugestão de extensões para uso no Vscode:
* HTML Snippets;
* Live HTML Previewer;

### Display:flex
`Display:flex` torna a tag um elemento do tipo flex container, e assim automaticamente todos os seus filhos diretos desta tag tornam-se em flex items.

### Flex-direction
`flex-direction` é a propriedade que estabelece o eixo principal do container, definindo assim a direção que os flex items são colocados no flex container.

Eixo horizontal
* row (padrão): à direção do texto, esquerda para direita.
* row-reverse: sentido oposto à direção do texto.

Eixo vertical
* column: ordenação de cima para baixo, em coluna única.
* column-reverse: ordenação reversa, de baixo para cima.