# Curso básico HTML + CSS

Curso dedicado aos princípios básicos de duas linguagens fundamentais do desenvolvimento web: HTML e CSS.


### Ferramentas necessárias:
- [Chrome](https://www.google.pt/intl/pt-PT/chrome/)
- [Visual Studio Code](https://code.visualstudio.com/)

[![](https://img.youtube.com/vi/-YHtjIY6kUQ/maxresdefault.jpg)](https://www.youtube.com/watch?v=-YHtjIY6kUQ)

### Conteúdos
- [Introdução ao HTML](#introdução-ao-html)
- [Sintaxe do HTML](#sintaxe-do-html)
- [Estrutura de um documento](#estrutura-de-um-documento)
- [Primeira página](#primeira-pagina)
- [Tags essenciais](#tags-essencias)
- [Introdução ao CSS](#introducao-ao-css)
- [Sintaxe do CSS](#sintaxe-do-css)
- [Adicionar o CSS](#adicionar-o-css)
- [Selectores Classe e ID](#selectores-classe-e-id)
- [Principais Propriedades](#principais-propriedades)
- [Unidades](#unidades)
- [Media Queries](#media-queries)
- [Layouts](#layouts)
- [Bibliografia](#bibliografia)

## Introdução ao HTML

[![](https://img.youtube.com/vi/LHLtiLr6oTM/maxresdefault.jpg)](https://www.youtube.com/watch?v=LHLtiLr6oTM)


HTML (Hyper Text Markup Language) é uma linguagem de hipertexto e de marcação que descreve a estrutura de uma página web. 

- Por ser uma linguagem de hipertexto aceita links que permitem o acesso directo a outras páginas.
- Por ser uma linguagem de marcação aceita `<tags>` que permitem que os browsers consigam ler de forma correcta a estrutura de um documento.

O HTML é a linguagem base do desenvolvimento web, sendo que todas as outras como o CSS, Javascript ou PHP gravitam à sua volta.

O HTML não é considerado uma linguagem de programação pois não é capaz de instruir o computador para performar operações.

Um ficheiro HTML é identificado pela extensão `.html`.

## Sintaxe do HTML

[![](https://img.youtube.com/vi/Nc1l1oZEnqs/maxresdefault.jpg)](https://www.youtube.com/watch?v=Nc1l1oZEnqs)

### Tags

Um documento HTML é estruturado por tags, que são os elementos que indicam como a página deve ser renderizada pelo browser. 
As tags encontram-se dentro de um sinal de menor (<) e de maior (>) e, na sua maioria, têm uma marcação de início e outra de fim. Em alguns casos, apenas tem uma marcação que assinala o ínicio e o fim.

É a partir das tags que os browsers conseguem renderizar ou interpretar as páginas de forma correcta.

````
<nomeTag>Conteúdo</nomeTag>
<nomeTag />
````
Referências de todas as tags:
https://www.w3schools.com/TAGS/default.ASP

### Atributos

Algumas tags aceitam atributos que permitem adicionar propriedades.

````
<nomeTag atributo=”valor”>Conteúdo</nomeTag>
````

### Árvore de elementos

Uma página HTML é uma estrutura que se organiza em árvore sendo que as tags podem ter pais e filhos.

````
<tagPai>
    <tagFilho>
    </tagFilho>
</tagPai>
````

## Estrutura de um documento

[![](https://img.youtube.com/vi/uuiGQcAko0A/maxresdefault.jpg)](https://www.youtube.com/watch?v=uuiGQcAko0A)

Um documento HTML começa com o que chamamos de estrutura base. Esta estrutura é compostas por:
- Definição do documento (Doctype)
- Head 
- Body

````
<!DOCTYPE html><!-- definição do documento -->
 
<html>
   <head>
       <!-- No head (cabeça) estão as informações que não são para ser vistas pelo utilizador -->
   </head>
 
   <body>
       <!-- No body (corpo) estão as informações que são para ser vistas pelo utilizador -->
   </body>
</html>
````

### Definição do documento (Doctype)
Este elemento serve para informar o browser de que se trata de um documento com código HTML. É um elemento obrigatório e deve sempre estar na primeira linha. No passado era um código longo mas na versão 5 do HTML foi simplificado para `<!DOCTYPE html>`

### Head
No `<head>` estão as informações que não são para ser vistas pelo utilizador. Nele estão os metadados, links para outros arquivos e scripts. 

### Body
No `<body>`  encontram-se as informações para serem lidas pelo utilizador, que pode ser em formato de texto, imagem, vídeo, áudio ou códigos embutidos.


## Primeira página

[![](https://img.youtube.com/vi/1miYn5m-X7g/maxresdefault.jpg)](https://www.youtube.com/watch?v=1miYn5m-X7g)

````
<!DOCTYPE html>
 
<html>
   <head>
       <title>A  minha primeira página</title> <!-- título do documento -->
       <meta charset="utf-8"> <!-- codificação da língua -->
   </head>
 
   <body>
       Olá mundo!
   </body>
</html>
````

## Tags essenciais

[![](https://img.youtube.com/vi/zDCyWakgpIE/maxresdefault.jpg)](https://www.youtube.com/watch?v=zDCyWakgpIE)

### Títulos e subtítulos

Os títulos e subtítulos são identificados pelas tags `<h1>` até à `<h6>`. `<h1>` o mais importante e `<h6>` menos importante.

````
<h1>Título 1</h1>
<h2>Título 2</h2>
<h3>Título 3</h3>
<h4>Título 4</h4>
<h5>Título 5</h5>
<h6>Título 6</h6>
````

### Parágrafos
Os parágrafos são identificados pela tag `<p>`.

````
<p>Isto é um parágrafo.</p>
```` 

### Lista não ordenada
Uma lista não ordenada é identificada pela tag `<ul>` e cada item pela tag `<li>`. 
Numa lista não ordenada cada item é antecedido por um símbolo bullet.

````
<ul>
    <li>Item 1</li>
    <li>Item 2</li>
    <li>Item 3</li>
</ul>
````

### Lista ordenada
Uma lista ordenada é identificada pela tag `<ol>` e cada item pela tag `<li>`. 
Numa lista ordenada cada item é numerado por ordem.

````
<ol>
    <li>Item 1</li>
    <li>Item 2</li>
    <li>Item 3</li>
</ol>
````

### Links
O links são criados utilizando a tag `<a>` que recebe o atributo `href=''` que contém o URL.

````
<a href='<!-- URL -->'>Texto que aparece</a>
````

### Imagens

[![](https://img.youtube.com/vi/Uhei8I5o6Uk/maxresdefault.jpg)](https://www.youtube.com/watch?v=Uhei8I5o6Uk)

As imagens são definidas pela tag `<img>` que recebe o atributo `src=''` que contém o URL da imagem ou o caminho relativo, caso a imagem esteja no nosso servidor.

````
<img width='500' src='<!-- URL da Imagem -->'>
<img width='500' src='<!-- caminho relativo -->'>
````

### Blocos

[![](https://img.youtube.com/vi/FUccstmdnpc/maxresdefault.jpg)](https://www.youtube.com/watch?v=FUccstmdnpc)

Os blocos são elementos que começam sempre numa nova linha e ocupam toda a largura possível.

````
<header>Header</header>
<div>Block</div>
<footer>Footer</footer>
````


# CSS

## Introdução e sintaxe do CSS

[![](https://img.youtube.com/vi/ZpYlFbsl1eY/maxresdefault.jpg)](https://www.youtube.com/watch?v=ZpYlFbsl1eY)

CSS (Cascading Style Sheets) é uma extensão do HTML que permite manipular os estilos de um documento ao dizer como elementos devem aparecer no browser.

Deste modo, o CSS define o design e permite que o website seja responsivo (que se adapte aos diferentes tamanhos de ecrã).

Uma regra em CSS é definida por um selector e por um bloco de declarações. Cada declaração é composta por uma propriedade e por um valor atribuído.

````
selector {
    propriedade1: valor1;
    propriedade2: valor2;
}
````

## Adicionar o CSS
[![](https://img.youtube.com/vi/WjnKhY715SA/maxresdefault.jpg)](https://www.youtube.com/watch?v=WjnKhY715SA)
[![](https://img.youtube.com/vi/QgxQrVbvLZ0/maxresdefault.jpg)](https://www.youtube.com/watch?v=QgxQrVbvLZ0)
Podemos adicionar o CSS de três formas diferentes:
- inline
- interno
- externo (preferencial)

### Inline
Directamente numa tag HTML através do atributo `style=""`.

Este método não é aconselhável pois, por uma questão de organização, devemos separar o código HTML do CSS.

````
<p style="color: blue">Texto azul</p>
````

### Interno
Através da tag `<style>` colocada no `<head>`, que permite que seja utilizada a sintaxe CSS dentro de um documento HTML.

````
<html>
  <head>
    <style>
      p {
        color: blue;
      }
    </style>
  </head>
  <body>
    <p>Texto azul</p>
  </body>
</html>
````

### Externo
Através de um ficheiro externo com a extensão `.css`, que permite separar o código CSS do documento HTML. 

O fichero CSS deve ser colocado na pasta do website e chamado pelo HTML através da tag `<link>` colocada no `<head>`. A tag `<link>` recebe o atributo `href=""`que recebe o caminho relativo do ficheiro CSS.

Exemplo se o ficheiro CSS (style.css) estiver na mesma pasta que o ficheiro HTML:

````
<head>
    <link rel="stylesheet" href="style.css">
<head>
````


## Selectores Classe e ID
Além das referências das tags podemos identificar os elementos de uma página pela sua "classe" ou "id".

### Classes
O selector "classe" seleciona todos os elementos HTML que têm o atributo `class=` com o valor referido antecido por um `.`. As classes identificam um grupo de elementos e um elemento pode ter mais do que uma classe.

`````
.azul {
  background: blue;
}
`````
`````
<div class="azul">
  Elemento com a class "azul"
</div>
<div class="azul">
  Elemento com a class "azul"
</div>
<div class="azul">
  Elemento com a class "azul"
</div>
`````

### IDs
O selector "id" é semelhante ao selector "classe" mas deve ser utilizado para seleccionar um elemento único que têm o atributo `id=` com o valor referido antecido por um `#`. Cada elemento apenas pode ter um "id". Normalmente os "ids" são utilizados para identificar a estrutura de uma página.

`````
<div id="cabecalho">
    Cabeçalho
</div>
<div id="noticias">
    Notícias
</div>
<div id="destaques">
    Destaques
</div>
<div id="agenda">
    Agenda
</div>
<div id="rodape">
    Rodapé
</div>
`````

## Principais Propriedades

### Box-model
- `width` define a largura da caixa;
- `height` define a altura da caixa;
- `margin` define o espaço à volta da caixa;
- `padding` define o espaço entre o limite da caixa e o seu conteúdo;
- `border` define a borda da caixa;

### Formatacão de texto
- `font-family` altera a fonte;
- `font-size` define a altura da fonte;
- `font-weight` define o peso da fonte;
- `line-height` define a altura da linha de texto;
- `text-align` – define o alinhamento do texto (left, right, center);
- `text-decoration` – adiciona elementos decorativos ao texto;
- `text-transform` – define a capitalização do texto;
- `letter-spacing` – espaço entre os caracteres.

### Posições
A propriedade posição define o modo como um elemento é posicionado.

- `position: static;` posição relativa ao flow da página (posição por defeito);
- `position: relative;` posição relativa à sua normal posição;
- `position: absolute;`  posição relativa ao elemento pai;
- `position: fixed;`  posição relativa à viewport;
- `position: sticky;` posição relativa à posição do scroll;


## Unidades

### Absolutas

As unidades absolutas têm sempre o mesmo tamanho independemente do tamanho da janela ou do elemento pai. São utilizadas quando os projectos não precisam de ser responsíveis, isto é, que não se adaptem a diferentes tamanhos de ecrã.

#### Principais unidades absolutas
Unidades Absolutas | Nome | Descrição 
--- | --- | ---
px | Pixeis | 1px = 1/96th of 1in
pt | Points | 1pt = 1/72th of 1in

### Relativas
As unidades relativas têm tamanhos escaláveis consoante o tamanho da janela ou do elemento pai. Apesar de serem um pouco mais difíceis de ser controladas, estas unidades são muito úteis para projectos que tenham de funcionar em diferentes formatados de ecrã.

#### Principais unidades relativas
Unidades Relativas | Descrição 
--- | ---
% | Percentagem relativa ao valor da propriedade no elemento pai
em | Unidade relativa ao tamanho da fonte do elemento
rem | Unidade relativa ao tamanho da fonte da root (html)
vw | Unidade relativa à largura da viewport. 1vw = 1/100 da largura da viewport
vh | Unidade relativa à altura da viewport. 1vh = 1/100 da altura da viewport
vmax | Unidade relativa à dimensão máxima da viewport. 1vmax = 1/100 da dimensão máxima da viewport
vmin | Unidade relativa à dimensão minima da viewport. 1vmin = 1/100 da dimensão minima da viewport

## Media Queries
As media queries servem para definir diferentes regras consoante o tipo de media ao captarem as capacidade do dispositivo. 
Assim podem identificar os seguintes valores:
- largura e altura da viewport;
- largura e altura do device;
- a orientação (horizontal ou vertical);
- a resolução.

### Sintaxe das Media Queries
````
media not|only mediatype and (expressions) {
  CSS-Code;
}
````

Valor | Descrição
--- | ---
all | Todos os tipos de media
screen | Para computadores, tablets, telemóveis, etc..
print | Para impressoras
speech | Para leitores de ecrãs

### CSS para diferentes tamanhos de ecrãs
`````
// ecrãs até 320px
@media screen and (max-width: 320px) {
 h1 {
  font-size: 20px;
 }
}
// ecrãs até 980px
@media screen and (min-width: 980px) {
 h1 {
   font-size: 15px;
 }
}
`````
## Layouts
O desenho de um layout é definido por uma grelha ou um grupo de grelhas que servem de guias para o posicionamento dos diversos elementos numa página.

### Elementos HTML de Layout
- `<header>`
- `<nav>`
- `<main>` 
- `<aside>` 
- `<section>`
- `<article>`
- `<footer>`

### Técnicas de Layout
- Propriedade de Float (desactualizada)
- Flexbox
- CSS Grid
- Frameworks 

## Flexbox
O flexbox é um modelo de layout unidimensional com a capacidade de organizar espacialmente e alinhar elementos.


### Flex Container: Propriedades
- `display: flex;`


- `flex-direction` 
- `flex-wrap`  
- `flex-flow`  


- `justify-content`
- `align-items`
- `align-content`

### Flex Item: Propriedades
- `order`                      
- `flex-grow`
- `flex-basis`
- `flex`
- `align-self`

### Mais informações
- [https://css-tricks.com/snippets/css/a-guide-to-flexbox/]
- [https://origamid.com/projetos/flexbox-guia-completo/]

## CSS Grid 
> "The use of the grid as an ordering system is the expression of a certain mental attitude inasmuch as it shows  that the designer conceives his work in terms that are constructive and oriented to the future"
> – Jusef Muller-Brockmann

O CSS Grid é um modelo de layout bidemencional, através do qual se pode manipular as colunas e as linhas em simultâneo.

### Mais informações
- [https://css-tricks.com/snippets/css/complete-guide-grid/]
- [https://www.origamid.com/projetos/css-grid-layout-guia-completo/]

## Frameworks
Um frameworks é um conjunto de regras abstractas que permitem a sua utilização fácil sem que seja necessário reescreve-las sempre que se queira utilizar.

- [Skeleton](http://getskeleton.com/)
- [Flexboxgrid](http://flexboxgrid.com/)
- [Foundation](https://get.foundation/)
- [Bootstrap](https://getbootstrap.com/)


## Bibliografia
- [https://www.w3schools.com/html/]
- [https://www.w3schools.com/css/]




