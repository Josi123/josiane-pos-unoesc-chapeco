#### Unoesc Chapecó
#### Pós-graduação em Desenvolvimento Web, Cloud e dispositivos móveis - WebMob
#### Disciplina: HTML5+CSS3
#### Professor: Jean Carlo Nascimento
#### Acadêmica: Josiane Meneghetti
### Artigo de revisão de CSS3
##### Funcionalidade:  opacity
##### O que é?
Permite dar opacidade em elementos HTML
##### Onde usar:
Qualquer elemento.
##### Como usar:
```css
seletor {
opcity:([level]);
}
```
##### Exemplo de uso

```css
seletor { 
  opacity:0.8;
}

```
##### Funcionalidade: transition
##### O que é?
Mostra uma transição de um estado para outro quando o usuário passa o mouse sobre o elemento.
##### Onde usar:
Qualquer elemento que tenha tamanho definido ou posição.
##### Como usar:
```css
seletor {
transition [propriedade] | [tempo(s)]
}
```
##### Exemplo de uso

```css
seletor { 
    width: 100px; 
    height: 100px; 
    background: #000; 
    transition: margin-left 2s; 
}

```
##### Funcionalidade: linear-gradient 
##### O que é?
O linear-gradinte é uma propriedade do background que permite criar listras de cores e repertir-lás por todo o fundo da página, sem precisar usar imagens.
##### Onde usar:
Em tags que podem receber o atributo background.
##### Como usar:
```css
seletor {background: repeating-linear-gradient(
[ <deg> | <graus> ] [ <rgb> | <000,000,000> ] [ <rgb> | <000,000,000> <height>] [ <rgb> | <000,000,000> <height>]  [ <rgb> | <000,000,000> <height>] ?);
}
```
##### Exemplo de uso

```css
seletor {
background: repeating-linear-gradient(
30eg,
#0000FF,
#0000FF 10px,
#FFFF7A 10px,
#FFFF7A 20px
);

```
##### Funcionalidade: box-shadow
##### O que é?
Propriedade que permite adicionar sombras em um elemento, primeiramente define-se a posição da sombra em relação ao elemento pai, isso é feito nos dois
primeiros valores, primeiro valor referente a top e bottom, e segundo valor left e right. O terceiro valor permite controlar se a sombra vai ser esfumaçada ou rígida.
Após definir essas propriedades é preciso sertar a cor da sombra.
##### Onde usar:
Pode ser usada em elementos HTML que possuem uma margem em relação ao tamanho da tela, também é possível usar esse efeito de sombras em textos, usando text-shadow.
##### Como usar:
```css
seletor {box-shadow: (
[ <height> | <px> ],[ <height> | <px> ], <height> | <px> ], [ <rgb> | <000,000,000> ] ?);
}
```
##### Exemplo de uso

```css
seletor {
box-shadow:  10px 10px 10px #3D3DFF;
};

```
##### Funcionalidade: multiplos backgrounds
##### O que é?
Permiter definir multiplas imagens de fundo para um elemento.
##### Onde usar:
Pode ser usada em elementos HTML que podem receber a propriedade.
##### Como usar:
```css
seletor {  background-image: (
[ <background1> ,[ <background1> ], <...> ] ?);
}
```
##### Exemplo de uso

```css
seletor {
    background-image: url(fundo1.jpg), url(fundo2.jpg);
    background-position: top left,top right;
    background-repeat: no-repeat, no-repeat;
};

```
##### Funcionalidade: animation
##### O que é?
Permite que seja setado um ponto inicial e um ponto final, assim como um angulo para um elemento HTML, fazendo com que execute uma determinada animação
durante o tempo e a velociades setados. Para conseguir que o efeito seja realizado com sucesso é preciso usar a regra de @-webkit-keyframes.
É preciso definir as caracteristicas do elemento, como tamanho, cor e formato, e depois as propriedades do animation, na -webkit-animation-name é setado o nome da 
regra do keyframe, na -webkit-animation-duration o tempo de duração da animação, na -webkit-animation-timing-function a forma como a
animação vai acontecer, na-webkit-animation-iteration-count por quanto tempo ela vai acontecer e em -webkit-animation-direction sua direção.
##### Onde usar:
Qualquer elemento que possua uma altura e uma largura definidas.
##### Como usar:
```css
seletor {
[ <width> | <px> ],[ <height> | <px> ], <height> | <px> ], [ <background> | <000,000,000> ], [<-webkit-animation-name> | <nome>]
[<-webkit-animation-duration> | <s>], [<-webkit-animation-timing-function> | <efeito>], [<-webkit-animation-iteration-count> | <infinite>],
[<-webkit-animation-direction> | <direction>];s
}
```
##### Exemplo de uso

```css
@-webkit-keyframes rodaroda {
		from {
			-webkit-transform:rotate(90deg);
		}
		to {
			-webkit-transform:rotate(0deg);
		}
}
seletor {
	width:50px;
	height:50px;
	background: #000;
 
	-webkit-animation-name: rodaroda;
	-webkit-animation-duration: 0.5s;
	-webkit-animation-timing-function: linear;
	-webkit-animation-iteration-count: 100;
	-webkit-animation-direction: left;
}
```
##### Funcionalidade: rotate
##### O que é?
Rotaciona um elemento HTML em angulos 2D ou 3D, porém pouquissímos navegadores suportam o 3D. 
##### Onde usar:
Pode ser usado para carregar um elemento com um angulo diferente, ou mudar o angulo deste elemento após o click ou hover.
##### Como usar:
```css
seletor {   transform: (
[ <rotate> | <angulo> ]?);
}
```
##### Exemplo de uso

```css
seletor {
 transform: rotate(30deg);  
};

```
#####Funcionalidade:  @font-face
#####O que é? <br />
Permite usar família de fontes fora do padrão do sistema 
#####Onde usar: <br />
Tags de fontes. 
#####Como usar: 
```css
@font-face{  
font-family: “nome da fonte”; 
src= url(‘caminho-da-fonte.otf’); 
 
}  
#####Exemplo de uso 
@font-face { 
font-family: helveticaneue; 
src: url(‘HelveticaNeueLTStd-UltLt.otf’); 
} 
```
 
```
##### Funcionalidade: text-overflow
##### O que é?
Permite recortar o texto maior do que o tamanho do box e acrescenta reticências(...) no final da frase, mostrando que o texto continua.
##### Onde usar:
Qualquer texto.
##### Como usar:
```css
seletor {  text-overflow (
[ <ellipsis> ]?);
}
```
##### Exemplo de uso
```css
seletor { 
    white-space: nowrap;  
    width: 120px;  
    overflow: hidden; 
    text-overflow: ellipsis;  
    border: 1px solid #000000; 
}  

``````
##### Funcionalidade: media queries
##### O que é?
Permite que sejam carregadas diferentes estilizações conforme a resolução do dispositivo usado. 
##### Onde usar:
Qualquer elemento de um site.
##### Como usar:
```css
seletor {  @media (min-width: px) and (max-width: px) { ... }?);
}
```
##### Exemplo de uso
```css
@media (max-width: 767px) { 
  selector ul{ 
  display: block
  } 
}

```
##### Funcionalidade: calc() 
##### O que é?
Permite que o valor determinado para um propriedade seja o resultado de um calculo.
##### Onde usar:
Elementos que tenham tamanho ou valor definido.
##### Como usar:
```css
seletor { propriedade: calc(expressão matemática); } 
}
```
##### Exemplo de uso
```css
 seletor { 
        height: calc(100%- 10px); 
    }

```
### Referencia:
http://tableless.com.br/tag/css3/
http://www.w3schools.com/css/css3_animations.asp
http://www.w3schools.com/css/css3_transitions.asp
http://www.maujor.com/tutorial/guia-completo-seletores-css3.php
