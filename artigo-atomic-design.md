
## Atomic Design
#####Resumo:
Atualmente  os desenvolvedores possuem uma necessidade que o mercado os exigem, de fazer sistemas web e sites que sejam responsivos. Cada vez mais as pessoas usam diferentes dispositivos e é obrigação do webdesigner fazer sistemas que estejam acessíveis de qualquer um desses dispositivos. 
Porém veio com isso projetos que exigem mais tempo para serem concluídos, pois o webdesigner precisar ter o cuidado de projetar o sistemas para diferentes resoluções a Atomic Designer vem para otimizar esse processo e facilitar a vida destes profissionais.
#####1) O que é?
Metodologia criada para abranger todo um processo de desenvolvimento de sistema para web ou site, facilitando a visualização do projeto por todos os membros, desde o cliente. Baseia-se na ideia de que não se desenvolve apenas páginas para a web, mas uma espécie organismo (sistema) formado por átomos, moléculas e organismo.  Sim, a ideia é mesma que a explicada nas aulas de química, aonde átomo dever ser compreendido como o menor componente do sistema, moléculas é um conjunto de átomos, e o organismo é tudo isso junto e organizado.
#####2) Como funciona
No principio tudo começa pelo menor componente o  átomo.<br />
#####Átomo<br />
São os menores componentes do sistema, aqueles que não podem ser dividos e que se juntam para formar uma molécula. Pensando em linguagem de marcação os átomos são as menores tags disponíveis, aquelas que não necessitam de um contexto para existir, como inputs, botões, parágrafos, títulos...
A partir do conjunto dessas tags soltas formam-se blocos maiores, as moléculas.<br />
#####Moléculas
Consiste no agrupamento dos átomos. Que existem soltos, porém sendo apenas átomos não possuem nenhum proposito, já quando agrupado terão uma finalidade, como por exemplo os campos de input, label e um botão, isolados não fazem nada, mas juntos formam um formulário.
#####Organismos<br />
E por fim temos um conjunto de moléculas que formam os organismos. Podemos pensar em organismos como sendo as seções dentro de um pagina web, como por exemplo, o rodapé e o cabeçalho. O rodapé pode ser visto como um organismo, formado por moléculas que é um conjunto de átomos (imagem, links, parágrafos...).
Depois de der o organismos formados os sistema já começa a ganhar forma.<br />
#####Template<br />
É formado pelo conjunto dos organismos, e nessa etapa já teremos a diagramação dos elementos do nosso sistema.  Aqui é possível desenvolver um wireframe  e ter a visão final de como o site.<br />
#####Páginas<br />
Essa é a etapa final do atomic designer e é onde a paginas web é lapida. Recebe cores e formatos e interação com o usuário.<br />
#####3) Para que usar
Pode-se criar um mini framework, facilitando o reuso de estilização de tags dentro de um sistema, melhorando o processo de desenvolvimento.
#####4) Onde usar?
O conceito de Atomic Designer pode ser aplicado em qualquer área de desenvolvimento de software, porém foi pensado para sistemas web e sites.
#####5) Exemplos:
######Átomo
```html
<input type="text" value="Exemplo de átomo" />
<h1>Exemplo de átomo</h1>
<p>>Exemplo de átomo</p>
```
######Molécula
```html
  <nav>
        <ul>
            <li><a href="">Exemplo de molécula</a></li>
            <li><a href="">Exemplo de molécula</a></li>
            <li><a href="">Exemplo de molécula</a></li>
        </ul>
  </nav>
  ```
######Organismos
  ```html
  <header>
    <img src="logo.png">
    <nav>
        <ul>
            <li><a href="">Exemplo de molécula</a></li>
            <li><a href="">Exemplo de molécula</a></li>
            <li><a href="">Exemplo de molécula</a></li>
        </ul>
    </nav>
    <form>
      <input type="text" value="Exemplo de átomo" />
      <button value="Buscar"></button>
    </form>
</header>
```
######Template
<img src="http://bradfrost.com/wp-content/uploads/2013/06/template1.jpg">

######Página:
<img src="http://bradfrost.com/wp-content/uploads/2013/06/page1.jpg">



#####6) Referências
http://tableless.com.br/o-que-e-design-atomic/<br />
http://bradfrost.com/blog/post/atomic-web-design/<br />
http://www.frontendbrasil.com.br/tutoriais/atomic-design-como-funciona/

