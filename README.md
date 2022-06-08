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

### Flex-wrap
`flex-wrap` é a propriedade que define se os itens devem ou não quebrar a linha. Por padrão, eles não quebram linhas, isso faz com que os flex itens sejam compactados além do limite do conteúdo.

* nowrap: é o padrão, não permite a quebra de linha.
* wrap: permite a quebra de linha assim que um dos flex itens não puder mais ser compactado.
* wrap-reverse: permite a quebra de linha assim que um dos flex itens não puder mais ser compactado, porém na direção contrária da linha, acima.

### Flex-flow
`flex-flow` é um atalho para as propriedades `flex-direction` e `flex-wrap`. Porém seu uso não é tão comum, visto que quando mudamos o flex-direction para column, mantemos o padrão do flex-wrap que é nowrap.

### Justify content
`justify-content` se encarrega de alinhar os itens dentro do container de acordo com a direção pretendida e trata da distribuição de espaçamento entre eles. Caso seus itens estejam ocupando 100% de todo o container, não se aplica.

* flex-start: início do container.
* flex-end: final do container.
* flex-center: centro do container.
* space-between: cria um espaçamento igual entre os elementos.
* space-around: os espaçamentos do meio são duas vezes maiores que o inicial e final.

### Align-itens
`align-itens` trata do alinhamento dos flex itens de acordo com o eixo do container. O alinhamento é diferente para quando os itens estão em colunas ou linhas. Permite o alinhamento central no eixo vertical.

* center: alinha os itens ao centro.
* strecth: padrão, e os flex itens cresçam igualmente.
* flex-start: alinhamento dos itens no início.
* flex-end: alinhamento dos itens no final.
* baseline: alinhamento de acordo com a linha base da tipografia dos itens.

### Align-content
`align-content` é a propriedade responsável por tratar o alinhamento das linhas do container em relação ao eixo vertical do container.
É necessário que:
* o container utilize quebra de linhas.
* a altura do container seja maior que a soma das linhas dos itens.

Tipos de alinhamento:
* center: alinhamento dos itens ao centro.
* stretch: é o padrão e os flex itens crescem igualmente.
* flex-start: alinhamento dos itens no início.
* flex-end: alinhamento dos itens no final.
* space-between: cria um espaçamento igual entre os elementos.
* space-around: os espaçamentos do meio são duas vezes maiores que o inicial e final.

## Fundamentos do Flex Box - Parte 2

### Estrutura básica do flex grow
`flex-grow` é a propriedade que define a proporcionalidade de crescimentos dos itens, respeitando o tamanho de seus conteúdos internos.
Não irá funcionar caso tenhamos adicionado justify-content ao nosso flex container.

### Estrutura básica do flex basis
`flex-basis` é a propriedade que estabelece o tamanho inicial do item antes da distribuição de espaço restante dentro dele, usando como base o conteúdo interno disposto.

Valores possíveis:
* auto: caso o item não tenha tamanho, este será proporcional ao conteúdo do item.
* px, %, em, etc...: são valores exatos previamente definidos
* 0 (zero): terá relação com a definição do flex-grow
