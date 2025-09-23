<!-- Leitura -->  
tags que precisam ser implementadas e entender seus papéis dentro do código.
https://www.alura.com.br/artigos/o-que-e-html-suas-tags-parte-1-estrutura-basica

https://www.alura.com.br/artigos/extensoes-vs-code-descubra-as-mais-usadas  outras extensões no artigo

https://www.alura.com.br/artigos/nomes-de-classes-no-css o Block Element Modifier (BEM).

https://www.alura.com.br/artigos/qual-diferenca-entre-id-e-class uso de classes e conhecer outro atributo semelhante chamado id

https://www.alura.com.br/artigos/criando-layouts-com-css-grid-layout o uso de Grid.

https://medium.com/collabcode/pare-de-chutar-e-aprenda-como-funciona-o-display-inline-block-4e6cba2f19d4 forma de display: o inline-block.

<!-- New-Item imagens\.gitkeep -ItemType File --> 
O Git não rastreia pastas vazias. Se imagens/ estiver vazia, você pode criar um arquivo especial para forçar o rastreamento. Esse .gitkeep é uma convenção usada para manter pastas vazias no repositório.


<!-- Background-image:  -->
Não foi colocada dentro da tag <img> porque ela é considerada decorativa e não essencial para o entendimento do conteúdo da página. Imagens decorativas, como a de fundo, são melhor implementadas via CSS, pois não afetam a semântica do HTML. Isso garante que, caso a imagem não carregue, a experiência do usuário não seja prejudicada. 

<!-- Button e Ancora <a> -->
 <button> é o mais apropriado e semanticamente 
    Executa uma ação, como apagar os dados de um formulárioo u disparar um script.
    Garante que a funcionalidade seja clara para o usuário e acessível para tecnologias assistivas. 
    Possui comportamentos padrão de acessibilidade.
 
 <a> Melhorar a indexação: 
    Links feitos com <a> são rastreados e seguidos pelos robôs do Google.
    Aumentar a relevância: se o texto da âncora for bem escolhido, ele pode ajudar a posicionar melhor a página de destino.
    Use **text-align** quando quiser centralizar texto ou imagens dentro de um bloco.


<!--  Text-align e Align-Items -->

**TEXT-ALIGN**:
Aplica-se a elementos inline ou inline-block dentro de um elemento de bloco. É usada principalmente para alinhamento horizontal de texto e elementos inline. Funciona em elementos como <span>, <img>, <a> quando estão dentro de uma <div> ou outro bloco.
Exemplo:
css
.container {
  text-align: center;
}
Isso vai centralizar o texto e imagens dentro da .container, desde que sejam elementos inline ou inline-block.

**ALIGN-ITEMS**:
É uma propriedade usada dentro de layouts flexíveis, ou seja, quando o display: flex está ativo. Controla o alinhamento vertical dos itens dentro do container flex. Só funciona se o elemento pai tiver display: flex.
Exemplo:
css
.container {
  display: flex;
  align-items: center;
}
Isso vai alinhar os elementos filhos verticalmente ao centro do container.
Use **align-items** quando estiver trabalhando com layout flexível e quiser controlar o alinhamento dos itens verticalmente.

<!-- display: inline-block -->
É um valor de display que combina o melhor dos dois mundos:
Como **INLINE**: o elemento fica na mesma linha que outros elementos, se houver espaço.
Como **BLOCK**: o elemento aceita propriedades de tamanho, como width, height, margin, padding.

📊 Comparação com outros valores de display:
Valor	Quebra de linha?	Aceita width/height?	Pode ficar lado a lado?
block	✅ Sim	✅ Sim	❌ Não
inline	❌ Não	❌ Não	✅ Sim
inline-block	❌ Não	✅ Sim	✅ Sim

Exemplo:
  .botao {
  display: inline-block;
  padding: 10px 20px;
  background-color: blue;
  color: white;
  border-radius: 5px;
}
Esse botão vai ocupar apenas o espaço necessário, pode ter padding e bordas, e ainda pode ficar lado a lado com outros elementos.