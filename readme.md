# Curso Flexboxes

Propriedade que veio com CSS3 para trabalhar com layouts responsivos na web com mais facilidade.

## Propriedades do Flexbox

Para trabalhar com flexboxes, usar ```display: flex;``` no elemento em si ou no elemento por fora dos elementos desejados.

### Flex-direction

Determina o eixo principal a ser trabalhado, recebe quatro valores:

- **row**: eixo principal em linha; Atributo definido por padrão;
- **row-reverse**: eixo principal em linha, partindo da margem direita.
- **column**: eixo principal em coluna;
- **column-reverse**: eixo principal em coluna partindo da margem inferior.

#### Eixo cruzado

Quando o eixo principal está definido em linha, o eixo cruzado é o eixo vertical e vice-versa. É importante atentar-se a este datalhe na hora de justificar e alinhar os itens "Flex", pois as propriedades trabalham com eixos distintos.

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

### Justify-content

Alinhas os conteúdos no eixo principal.

### Align-items

Alinha os conteúdos em relação ao eixo cruzado. Valores possíveis:

- **flex-start**
- **flex-end**
- **center**
- **stretch**
- **baseline**

