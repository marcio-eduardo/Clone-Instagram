# Clone-Instagram
Trabalho de conclusão do curso de CSS da DIO

### Estudado no curso os seguintes itens:

## Flexbox em CSS

### Objetivo do curso

Apresentar os fundamentos e aplicações da propriedade flexbox na criação de layouts responsivos, sem a necessidade da definição de valores fixos.

- Introdução ao flexbox;
- fundamentos do flexbox;
- projeto integrador;

### Flex Container

É a tag que envolve os itens. Será nela que iremos aplicar a propriedade "display: flex". Transforma todos os seus filhos em flex itens.

**Propriedades relacionadas**

- display
- flex-direction
- flex-wrap
- flex-flow
- justify-content
- align-items
- align-content

### Flex Item

São os elementos filhos diretos do Flex Container. Também podem se tornar Flex Container

**Propriedades relacionadas:**

- flex-grow
- flex-basis
- flex-shrink
- flex
- order
- align-self

### Display: flex;

Torna a tag um elemento do tipo Flex Container**, assim, automaticamente todos os seus filhos diretos desta tag, tornam-se em **Flex Items**.



### Flex-direction

É a propriedade que estabelece o eixo principal do container, definindo assim a direção que os flex items são colocados no flex container.

### Os eixos

- **row (padrão)**: à direção do texto, esquerda para direita;
- **row-reverse**: sentido oposto à direção do texto;
- **column:** ordenação de cima para baixo, em coluna;
- **column-reverse:** ordenação inversa, de baixo para cima;



### Flex-wrap

É a propriedade que define se os itens devem ou não quebrar a linha.

Por padrão, eles não quebram linhas, isso faz com que os flex items sejam compactados além do limite do conteúdo.

- nowrap: é o padrão. Não permite a quebra de linha.
- wrap: permite a quebra de linha assim que um dos flez items não puder mais se compactado.
- wrap-reverse: permite qiebra de linha assim que um dos flex items não puder mais ser compactado, porém na direção contrária da linha, acima.

### Flex-flow

É um atalho para as  propriedades **fle-direction** e **flex-wrap**, porém seu uso não é tão comum, visto que, quando mudamos o flex-direction para column, mantemos o padrão do flex-wrap que é nowrap.

### Justify Content

Essa propriedade vai se encarregar de alinhar os itens dentro do conatainer de acordo com a direção pretendida e tratar da distribuição de espaçamento entre eles.

**Obs.:** caso seus itens estejam ocupando 100% de todo o container,ela não se aplica.

**As variações**

- **flex-start:** início do container;
- **flex-end:** final do container.
- **center:** ao centro do container;
- **space-between:** cria um espaçamento igual entre os elementos;
- **space-around:** os espaçamentos do meio são duas vezes maiores que o inicial e final;



### Align-itens

Trata do alinhamento dos flex itens de acordo com o eixo do container.

O alinhamento é diferente para quando os itens estão em colunas ou linhas

Permite o alinhamento central no eixo vertical.

### Topos de alinhamento

- **center**: alinhamento dos itena ao centro;
- **strech**: é o padrão e os flex itens crescem igualmente;
- **flex-start**: alinhamento dos itens no início;
- **flex-end**: alinhamento dos itens no final;
- **baseline**: alinhamento de acordo com a linha base da tipografiados itens;

### Align-content

É a propriedade responsável por tratar o alinhamento das linhas do container em relação ao eixo vertical do container.

**Precisamos que:**

- O container utilize quebra de linhas;
- A altura o container seja maior que a soma das linhas dos itens;

#### Tipos de alinhamento

- **center**: alinhamento dos itena ao centro;
- **strech**: é o padrão e os flex itens crescem igualmente;
- **flex-start**: alinhamento dos itens no início;
- **flex-end**: alinhamento dos itens no final;
- **space-between**: cria um espaçamento igual entre os elementos;
- **space-around**: os espaçamentos do meio são duas vezes maiores que o inicial e final;



## Fundamentos - Flex Items

### Flex-grow

Define a proporcionalidade de crescimentos dos itens, respeitando o tamanho de seus conteúdos internos.

**Obs.:** não irá funcionar caso tenhamos adicionado justify-content ao nosso flex container.

### Flex-basis

É a propriedade que estabelece o tamanho inicial do item antes da distribuição de espaço restante dentro dele, usando como base o conteúdo interno disposto.

**Valores possíveis**

- **auto**: caso o item não tenha tamanho, este será proporcional ao conteúdo do item;
- **px, %, em, ...:** são valores exatos previamente definidos;
- **0 (zero):** terá relação com a definição do flex-grow;

### Flex-shrink

É a propriedade que estabelece a capacidade de redução ou compressão do tamanho de um item.

### Flex

Esta propriedade é um atalho ou abreviação de escrita para as propriedades: grow, shrink e basis

### Align-self

É a propriedade que estabelece o alinhamento de modo individual sobre determinado item.

#### Valores possíveis

- **auto:** valor padrão, irá respeitar a definição de align-items do container;
- **flex-start:**ao início do container;
- **flex-end:** ao final do container;
- **center:** relativo ao centro de acordo com o eixo;
- **stretch:** ocupa todo os espaços relativo;
- **baseline:** utiliza a linha base da tipografia
