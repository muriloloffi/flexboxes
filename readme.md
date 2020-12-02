# Curso Flexboxes

Propriedade que veio com CSS3 para trabalhar com layouts responsivos na web com mais facilidade.

## Propriedades do Flexbox

Para trabalhar com flexboxes, aplicar ```display: flex;``` a partir das configurações CSS no elemento em si ou no elemento pai dos elementos desejados.

### Flex-direction

Determina o eixo principal a ser trabalhado, recebe quatro valores:

- **row**: eixo principal em linha; Atributo definido por padrão;
- **row-reverse**: eixo principal em linha, mas partindo da margem direita.
- **column**: eixo principal em coluna;
- **column-reverse**: eixo principal em coluna partindo da margem inferior.

#### Eixo cruzado

Quando o eixo principal está definido em linha, o eixo cruzado é o eixo vertical e vice-versa. É importante atentar-se a este datalhe na hora de justificar e alinhar os itens "Flex", pois as propriedades de alinhamento trabalham com eixos específicos.

### Flex-wrap

```flex-wrap: wrap;``` Permite que um container do tipo flexbox quebre em múltiplas linhas. Neste caso, cada linha se comporta como um contâiner distinto e a distribuição de espaço irá acontecer ao longo daquela linha.

Pode receber os valores:

- **nowrap**
- **wrap**
- **wrap-reverse**
- **initial**
- **inherit**

### Flex-flow

Permite combinar as propriedades `flex-direction` e `flex-wrap` em uma única. Exemplo de uso: ```flex-flow: row-reverse wrap;```

### Alinhamento

As propriedades de alinhamento trabalham com eixos predefinidos. Estes eixos são permutados conforme as direções de renderização escolhidas, "row" e "column".

#### Justify-content

Alinha os conteúdos no eixo principal. Este eixo será horizontal para linha e vertical para coluna. Valores possíveis:

- **flex-start**
- **flex-end**
- **center**
- **space-between**
- **space-around**
- **space-evenly**

#### Align-items

Alinha os conteúdos no eixo cruzado, ou seja, vertical para direção em linha e horizontal para coluna. Valores possíveis:

- **flex-start** - valor padrão.
- **flex-end**
- **center**
- **space-between**
- **space-around**
- **stretch**
- **space-evenly**

Desta forma, se um item está definido como linha/"row", a propriedade `align-items` irá modificar o eixo vertical, enquanto um item definido em coluna/"column" é modificado no eixo horizontal pela mesma propriedade.

### Flex: uso do espaço disponível

Com a propriedade `flex`, é possível definir como um ítem ocupa o espaço disponível. Esta propriedade é uma abreviação das propriedade `flex-grow`, `flex-shrink` e `flex-basis`. A propriedade flex pode ser declarada com um, dois ou três valores.

- **Sintaxe de um valor:** Deve ser um número que será interpretado como `flex: <número> 1 0;`; Isto quer dizer que `flex-grow` terá um valor customizado e que `flex-shrink` e `flex-basis` terão valores padrão 1 e 0, respectivamente.

- **Sintaxe de dois valores:** O primeiro valor será interpretado como `flex-grow` e deve ser um número. O segundo valor poder ser tanto um número quanto uma largura, que serão interpretados como `flex-shrink` ou `flex-basis`, respectivamente.

- **Sintaxe de três valores:** Os valores devem seguir a ordem "número, número e um valor de largura", que serão interpretados como `flex-grow`, `flex-shrink` e `flex-basis`.

O mais usual é a sintaxe de dois valores ou um valor, para definição das propriedades `flex-grow` e `flex-shrink` ou apenas `flex-grow`.
