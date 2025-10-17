# ☕ Bruma Cafeteria
Site institucional moderno e responsivo para a aquivo, uma agência de arquitetura e design focada em projetos comerciais e residenciais sustentáveis.

[![HTML5](https://img.shields.io/badge/HTML5-E34F26?style=for-the-badge&logo=html5&logoColor=white)](https://developer.mozilla.org/pt-BR/docs/Web/HTML)
[![CSS3](https://img.shields.io/badge/CSS3-1572B6?style=for-the-badge&logo=css3&logoColor=white)](https://developer.mozilla.org/pt-BR/docs/Web/CSS)
[![Responsive](https://img.shields.io/badge/Responsive-FF6B6B?style=for-the-badge&logo=mediaquery&logoColor=white)](https://developer.mozilla.org/pt-BR/docs/Web/CSS/Media_Queries)

## 📋 Sobre o Projeto
O site Bruma Cafeteria foi desenvolvido utilizando HTML5 e CSS3 com o objetivo de apresentar uma cafeteria fictícia, destacando seus produtos, filosofia e formas de contato.  
O projeto prioriza um design moderno, responsivo e intuitivo, proporcionando uma navegação agradável e fluida.

## Checklist (colar no README e marcar)

- [x]  3 páginas mínimas (Home/Sobre/Contato) + links funcionando.
- [x]  header, nav, main, footer usados com propósito.
- [X]  Hero na página principal
- [x]  Tabela simples presente.
- [x]  Paleta no :root (variáveis CSS).
- [x]  Google Fonts.
- [x]  Imagens otimizadas com alt descritivo.
- [x]  README com papéis, paleta, fontes e decisões.
- [x]  Site no ar.
- [x]  Vídeo de demonstração.
---


arquivo/
├── index.html          # Página inicial com hero section
├── sobre.html          # Sobre a empresa e serviços
├── servicos.html       # Detalhes completos dos serviços
├── contato.html        # Formulário de contato e mapa
├── assets/
│   ├── css/
│   │   └── styles.css  # CSS completo e organizado
│   └── img/
│       └── ARQUITETURA.jpg  # Imagem de background otimizada
└── README.md           # Documentação completa


---

## 🌐 Páginas do Site

### 🏠 Home (index.html)
- Exibe um banner principal (hero) com o slogan “Sinta a Bruma do seu drink”.
- Apresenta a seção “Nossos destaques”, com os principais produtos:
  - Expresso  
  - Drink Gelado  
  - Especial da Casa  
- Contém o menu de navegação e o rodapé com direitos autorais.

---

### 🍵 Sobre (sobre.html)
- Descreve a proposta e o conceito da Bruma Cafeteria.  
- Lista as principais bebidas oferecidas.  
- Inclui uma tabela de preços com nome, tamanho e valor de cada bebida.

---

### 📍 Contato (contato.html)
- Apresenta o endereço e meios de contato da cafeteria.  
- Exibe um mapa interativo do Google Maps mostrando a localização (Marco Zero – Recife).  

---

## 🎨 Estilo e Layout (CSS3)
O estilo do site é definido no arquivo css/style.css, com:
- Design responsivo (ajustável a diferentes telas);  
- Tipografia moderna e harmônica;  
- Cores neutras e elegantes, alinhadas ao tema de cafeteria;  
- Classes reutilizáveis, como .header, .footer, .container, .card, .botao, etc.

O código começa definindo variáveis CSS dentro de :root para gerenciar cores e famílias de fontes, o que facilita a manutenção e a consistência visual:

--cor-principal: #F7F4EA (Um bege ou branco suave, usado como fundo de alguns blocos e cor de texto em destaque).

--cor-destaque: #763932 (Um marrom escuro ou bordô, usado como fundo principal e cor de texto de destaque/links).

--cor-secundaria: #E1B382 (Um bege mais quente, não muito utilizado no código visível).

--cor-texto: #2C2C2C (Um cinza escuro, usado como cor de texto padrão).

--fonte-titulo: 'Pangolin', serif (Uma fonte mais lúdica, usada para títulos).

--fonte-texto: 'Open Sans', sans-serif (Uma fonte limpa e moderna, usada para o corpo do texto).

A folha de estilo também importa a fonte 'Pangolin' do Google Fonts e aplica um reset básico (*) para remover margens e preenchimentos padrão e usar o box-sizing: border-box.

O body recebe a cor de fundo --cor-destaque (marrom escuro), a cor de texto --cor-texto (cinza escuro) e a fonte --fonte-texto.

## 💻 Seções Principais de Layout
Header (.header e .nav)
O cabeçalho tem fundo --cor-principal (branco/bege), margens externas e cantos arredondados (border-radius: 30px), destacando-o do fundo da página.

O container (.container) centraliza o conteúdo em até 1200px.

A navegação (.nav) utiliza Flexbox para alinhar a logo e o menu, distribuindo o espaço (justify-content: space-between).

A navegação (.nav-menu) utiliza Flexbox para exibir os links horizontalmente, com a cor de destaque (--cor-destaque). O efeito hover aplica um sublinhado.

Hero (.hero)
A seção principal (hero) usa position: relative para permitir que o texto seja posicionado de forma absoluta sobre uma imagem (que teria a classe .hero-img).

O texto do hero (.hero-texto) é centralizado no meio da imagem (top: 50%, left: 30% com transform: translate) e utiliza a cor --cor-principal (branco/bege) para se destacar.

Os títulos usam a fonte --fonte-titulo (Pangolin).

O botão (.botao) é estilizado com borda e cor de texto --cor-principal e inverte as cores no hover.

Destaques/Cards (.destaques, .cards, .card)
Esta seção centralizada exibe a cor de fundo background-color: white nos cartões.

O título da seção (.titulo-secao) usa a fonte de título e a cor --cor-principal.

Os cards (.cards) utilizam Flexbox para exibir os itens lado a lado, permitindo quebras de linha (flex-wrap: wrap).

Cada card (.card) possui cantos arredondados, sombra e um efeito sutil de elevação no hover (transform: translateY(-5px)).

Rodapé (.footer)
O rodapé utiliza a cor de fundo --cor-destaque (marrom escuro) e cor de texto --cor-principal (branco/bege), garantindo contraste.

## 📄 Estilos Específicos e Responsividade
Estilos de Seções Genéricas
Todas as tags <section> são fortemente estilizadas com borda --cor-principal, cantos arredondados (30px), preenchimento e margem, criando grandes blocos delimitados.

Títulos h1 e h2 dentro de section usam a cor white e a fonte --fonte-titulo.

Parágrafos (p) dentro de section usam a cor --cor-principal.

Seções de Contato e Endereço
Classes .contato e .endereco definem blocos com largura fixa (500px e 610px, respectivamente) e display: inline-block, sugerindo que serão exibidos lado a lado na mesma linha.

Menu de Bebidas (.bebidas e .itemBebida)
A seção .bebidas tem fundo --cor-principal e borda/cantos arredondados, criando um grande bloco de menu.

Os itens de bebida (.itemBebida) usam a fonte de título e cor --cor-destaque, com borda.

No hover, o item inverte as cores, usando --cor-destaque como fundo e --cor-principal como texto.

Tabela (table, tr, td, th)
As tabelas são estilizadas de forma semelhante à seção .bebidas, com fundo --cor-principal.

Linhas (tr) e células (td) usam a cor --cor-destaque e a fonte de título.

As células (td) possuem um efeito hover que inverte cores, semelhante ao menu de bebidas.

Responsividade (@media)
Para telas com largura de 768px ou menos, os cards (.cards) são empilhados verticalmente (flex-direction: column).

O tamanho do título principal do hero (.hero-texto h1) é reduzido.

---

## 🧭 Navegação
O menu principal é fixo no topo e está presente em todas as páginas:

html
<ul class="nav-menu">
  <li><a href="index.html">Home</a></li>
  <li><a href="contato.html">Contato</a></li>
  <li><a href="sobre.html">Sobre</a></li>
</ul>
Essa estrutura garante consistência visual e facilidade de navegação.

⚙ Boas Práticas Adotadas
Uso de tags semânticas HTML5 (header, main, section, footer);

Imagens com atributo alt para acessibilidade;

Separação entre conteúdo e estilo (HTML × CSS);

Estrutura clara, limpa e bem organizada;

Responsividade por meio da meta tag viewport.

🎥 Demonstração do Projeto
Confira a demonstração em vídeo do projeto Bruma Cafeteria:

👉 Assista ao vídeo de demonstração

https://youtu.be/GMH5YwC9VnY?si=Fl8y7C1VQiD_Blep

🚀 Melhorias Futuras
Implementar formulário de contato funcional;

Adicionar animações sutis em CSS;

Criar modo escuro (dark mode);

Otimizar imagens para melhorar o desempenho.

🏁 Conclusão
O projeto Bruma Cafeteria representa visualmente uma marca fictícia de cafeteria, com foco em elegância, experiência do usuário e identidade visual marcante.
Desenvolvido com HTML5 e CSS3, o site cumpre seu papel de apresentar os produtos e essência da marca de forma clara e atraente.

## 👨‍💻 Autores 
Lauan Gonçalves – Estrutura e Acessibilidade** (HTML, semântica)
Thiago Cardozo – Layout e Componentes** (Flex, cards, botões)
Emily Raquel – Estilo e Documentação** (Paleta, tipografia, README, otimização de imagens).
📅 Desenvolvido em 2025
💻 Projeto acadêmico com fins de estudo e portfólio
