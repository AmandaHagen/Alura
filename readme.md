<!-- Leitura -->  
tags que precisam ser implementadas e entender seus papéis dentro do código.
https://www.alura.com.br/artigos/o-que-e-html-suas-tags-parte-1-estrutura-basica

https://www.alura.com.br/artigos/extensoes-vs-code-descubra-as-mais-usadas  outras extensões no artigo

https://www.alura.com.br/artigos/nomes-de-classes-no-css o Block Element Modifier (BEM).

https://www.alura.com.br/artigos/qual-diferenca-entre-id-e-class uso de classes e conhecer outro atributo semelhante chamado id

https://www.alura.com.br/artigos/criando-layouts-com-css-grid-layout o uso de Grid.

https://medium.com/collabcode/pare-de-chutar-e-aprenda-como-funciona-o-display-inline-block-4e6cba2f19d4 forma de display: o inline-block.

https://developer.mozilla.org/pt-BR/docs/Web/CSS/Pseudo-classes ler mais sobre pseudo-classes

https://www.alura.com.br/artigos/heroku-vercel-outras-opcoes-cloud-plataforma mais sobre esse tipo de serviço ou conhecer outros sites

https://beacons.ai/aluraonline Você pode encontrar os nossos perfis 

https://linktr.ee/monicahillman  linktree Instrutora Monica Hillman

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

<!-- Pseudo-classe -->
É uma propriedade que é adicionada ao final dos seletores que especifica o estado que esse elemento está. Ele detecta, por exemplo, se o elemento está com um mouse em cima dele, construindo uma experiência interativa com o usuário. 
**:focus:** é aplicada quando um elemento está em foco, pode ser pelo clique do mouse ou seleção pelo teclado. Um exemplo é quando os campos de escrita em formulários estão selecionados para o usuário escrever.

**:hover:** detecta quando um usuário está com o mouse em cima do elemento, sem necessariamente estar clicando.

**:active:** detecta quando o elemento está ativo, quando há uma interação, por exemplo: o link <a> está sendo clicado.

**:visited:** detecta quando o link <a> já foi visitado, ou seja, se você já clicou anteriormente naquele link.

**:link:** detecta quando é um link <a> que nunca foi clicado antes.

A sintaxe correta de uso de pseudo-classes é essa:
Utilização na prática seria este de trocar a cor do botão para azul quando o mouse estiver em cima dele:
.container__botao:hover {
  background-color: blue;
}

https://amandahagen.github.io/Alura/

pelo vercel

https://alura-4pipd15y4-amandahagens-projects.vercel.app/

Uma maneira super fácil e rápida de fazer essas pequenas alterações é diretamente no GitHub.

Já dentro da pasta do aluraplus, vamos pressionar o . (ponto final) no teclado. Com isso, abrimos o VS Code diretamente no navegador! Nem precisamos abrir localmente nosso computador!