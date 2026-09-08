# 👟 SyntaxWear — E-commerce de Sneakers & Streetwear

<div align="center">

![HTML5](https://img.shields.io/badge/HTML5-E34F26?style=for-the-badge&logo=html5&logoColor=white)
![CSS3](https://img.shields.io/badge/CSS3-1572B6?style=for-the-badge&logo=css3&logoColor=white)
![Design Responsivo](https://img.shields.io/badge/Design-Responsivo-success?style=for-the-badge)
![Status](https://img.shields.io/badge/Status-Concluído-blue?style=for-the-badge)

</div>

> **SyntaxWear** é uma landing page moderna de e-commerce voltada para a venda de tênis e sneakers com atitude urbana e futurista. O projeto foi concebido e desenvolvido com foco em boas práticas de HTML5 semântico, arquitetura modular de CSS3, design responsivo e acessibilidade.

---

## 📑 Sumário

- [Visão Geral](#-visão-geral)
- [Funcionalidades](#-funcionalidades)
- [Tecnologias e Práticas Utilizadas](#-tecnologias-e-práticas-utilizadas)
- [Estrutura do Projeto](#-estrutura-do-projeto)
- [Destaques de Implementação](#-destaques-de-implementação)
- [Responsividade](#-responsividade)
- [Como Executar o Projeto](#-como-executar-o-projeto)
- [Próximos Passos e Melhorias Futuras](#-próximos-passos-e-melhorias-futuras)
- [Autor](#-autor)

---

## 🎯 Visão Geral

O **SyntaxWear** apresenta uma experiência visual imersiva para o usuário, destacando lançamentos da linha de tênis (*Krypton One*) e categorias temáticas de calçados urbanos.

O site foi estruturado para proporcionar navegação fluida tanto em computadores desktop quanto em smartphones e tablets, utilizando soluções puras de CSS sem a necessidade imediata de bibliotecas externas pesadas.

---

## ✨ Funcionalidades

- **Cabeçalho Fixo e Flutuante (Header Flutuante):**
  - Barra de navegação centralizada com cantos arredondados e sombra elegante.
  - Links para categorias principais: *Masculino*, *Feminino* e *Outlet*.
  - Acesso rápido com ícones vetoriais: *Nossas Lojas*, *Sobre*, *Minha Conta*, *Ajuda* e *Carrinho de Compras*.
  - Menu responsivo estilo "hambúrguer" funcional em dispositivos móveis via técnica CSS Checkbox Hack.

- **Hero Banner Interativo:**
  - Imagem de capa em alta definição com suporte a imagem otimizada para mobile.
  - Chamada de impacto (*"Transforme qualquer passo em presença"*).
  - Botões de ação rápida (*CTA*): *"Ver modelos"* e *"Comprar"*.

- **Seção de Categorias Temáticas:**
  - Cards visuais com sobreposição escura (*overlay*) para melhor contraste e leitura:
    - 👟 **Casual**
    - 🏃 **Esporte**
    - ✨ **Moderno**
    - 🚀 **Futurista**

- **Vitrine de Produtos em Mosaico (Product Grid):**
  - Mosaico assimétrico moderno utilizando **CSS Grid (`grid-template-areas`)**.
  - Card de destaque principal com ações segmentadas (*Feminino* / *Masculino*).
  - Exibição de modelos conceituais e variações de cores e estilos de sneakers.

- **Rodapé Completo (Footer):**
  - Formulário de assinatura de newsletter para captura de e-mails.
  - Links para as principais redes sociais com ícones SVG (Instagram, WhatsApp, TikTok, Facebook).
  - Mapa de links de navegação categorizado em colunas organizadas.
  - Linha divisória e nota de direitos autorais (*Copyright*).

---

## 🛠 Tecnologias e Práticas Utilizadas

- **[HTML5](https://developer.mozilla.org/pt-BR/docs/Web/HTML):** Marcação semântica (`header`, `nav`, `main`, `section`, `footer`, `form`, `figure`, etc.) promovendo SEO e acessibilidade.
- **[CSS3](https://developer.mozilla.org/pt-BR/docs/Web/CSS):**
  - **CSS Reset:** Baseado no moderno reset de Andy Bell, garantindo consistência entre navegadores.
  - **CSS Custom Properties (Variáveis CSS):** Centralização de tipografia (`--font-principal`).
  - **Google Fonts:** Tipografia moderna utilizando a família tipográfica [Ubuntu](https://fonts.google.com/specimen/Ubuntu).
  - **Flexbox:** Distribuição inteligente de elementos no cabeçalho, hero e rodapé.
  - **CSS Grid:** Construção da vitrine assimétrica e flexível de produtos.
  - **Efeitos e Transições:** Transições suaves em pseudo-classes `:hover` para botões e ícones.
  - **Media Queries:** Adaptação completa de layouts para diferentes larguras de tela.
- **Ícones em SVG:** Ícones leves, nítidos e escaláveis sem perda de qualidade.

---

## 📂 Estrutura do Projeto

A organização de pastas e arquivos segue uma arquitetura modular e de fácil manutenção:

```plaintext
ecommerce-syntaxwear/
│
├── index.html                     # Estrutura principal do documento HTML
├── README.md                      # Documentação do projeto
│
├── css/                           # Folhas de estilo do projeto
│   ├── reset.css                  # Normalização e reset global de estilos
│   ├── variables.css              # Definição de variáveis CSS e importação de fontes
│   ├── base.css                   # Estilos globais (body, main, botões, classes utilitárias)
│   │
│   └── components/                # Estilos componentizados por seção
│       ├── header.css             # Estilo do cabeçalho e menu de navegação
│       ├── hero.css               # Estilo do banner principal e chamadas
│       ├── product-category.css   # Estilo dos cards de categorias
│       ├── product-grid.css       # Estilo do mosaico de produtos com CSS Grid
│       └── footer.css             # Estilo do rodapé, newsletter e redes sociais
│
├── images/                        # Ativos visuais e imagens estáticas
│   ├── banners/                   # Imagens dos banners de destaque
│   │   ├── hero.jpg               # Imagem do banner para desktop
│   │   └── hero-mobile.jpg        # Imagem do banner otimizada para mobile
│   │
│   ├── icons/                     # Ícones vetoriais em formato SVG
│   │   ├── bag.svg                # Ícone de sacola/carrinho de compras
│   │   ├── facebook.svg           # Ícone do Facebook
│   │   ├── hamburguer.svg         # Ícone do menu mobile
│   │   ├── help.svg               # Ícone de ajuda/suporte
│   │   ├── instagram.svg          # Ícone do Instagram
│   │   ├── tiktok.svg             # Ícone do TikTok
│   │   ├── user.svg               # Ícone de perfil/usuário
│   │   └── whatsapp.svg           # Ícone do WhatsApp
│   │
│   ├── logo/                      # Identidade visual da marca
│   │   └── logo.svg               # Logotipo oficial SyntaxWear
│   │
│   └── products/                  # Fotografias dos produtos e modelos
│       ├── card_imagem.jpg        # Imagem do card de destaque
│       ├── casual.jpg             # Imagem da categoria Casual
│       ├── esporte.jpg            # Imagem da categoria Esporte
│       ├── moderno.jpg            # Imagem da categoria Moderno
│       ├── futurista.jpg          # Imagem da categoria Futurista
│       ├── modelo-feminino.jpg    # Ensaio fotográfico conceito
│       ├── futurista-grid.jpg     # Foto do produto no grid
│       ├── moderno-grid.jpg       # Foto do produto no grid
│       ├── preto-branco-grid.jpg  # Foto do produto no grid
│       └── roxo-verde-grid.jpg    # Foto do produto no grid
│
└── js/                            # Diretório reservado para scripts JavaScript
```

---

## 🎨 Destaques de Implementação

### 1. Menu Mobile com CSS Puro (Checkbox Hack)
O menu responsivo no cabeçalho utiliza a técnica de controle de estado por meio de um elemento `<input type="checkbox">` e a pseudo-classe `:checked`:
```css
.menu-toggle:checked ~ .nav-container {
    right: 0;
}
```
Isso permite abrir e recolher o menu lateral em telas menores sem a dependência obrigatória de JavaScript inicial.

### 2. Vitrine Assimétrica com `grid-template-areas`
A vitrine de produtos organiza diferentes proporções de imagem de forma intuitiva e visualmente rica:
```css
.grid-section {
    display: grid;
    grid-template-columns: repeat(4, 1fr);
    grid-template-rows: repeat(3, 300px);
    grid-template-areas:
        "highlight highlight sneaker-purple sneaker-purple"
        "highlight highlight model sneaker-color "
        "sneaker-white sneaker-white model sneaker-silver ";
    gap: 30px;
}
```

---

## 📱 Responsividade

O layout foi planejado para se adaptar com elegância a diferentes resoluções:

| Breakpoint | Adaptações Aplicadas |
| :--- | :--- |
| **Desktop (> 1280px)** | Menu horizontal completo, cabeçalho flutuante centralizado, grid de produtos em 4 colunas. |
| **Tablet / Telas Médias (≤ 1280px e ≤ 1000px)** | Exibição do botão hambúrguer, menu em drawer lateral, rodapé reorganizado em colunas verticais. |
| **Mobile (≤ 768px e ≤ 500px)** | Banner com imagem vertical dedicada (`hero-mobile.jpg`), vitrine reestruturada para 2 colunas com áreas empilhadas, cards de categorias ocupando 100% da largura. |

---

## 🚀 Como Executar o Projeto

Como o projeto é composto por tecnologias fundamentais da web (HTML5 e CSS3), não é necessário instalar dependências ou gerenciadores de pacotes para visualizá-lo:

1. **Clone o repositório:**
   ```bash
   git clone https://github.com/RSGames2019/ecommerce-syntaxwear.git
   ```

2. **Acesse a pasta do projeto:**
   ```bash
   cd ecommerce-syntaxwear
   ```

3. **Abra o arquivo `index.html`:**
   - Dê um duplo clique no arquivo `index.html` para abri-lo no seu navegador padrão; **OU**
   - No VS Code, utilize a extensão **[Live Server](https://marketplace.visualstudio.com/items?itemName=ritwickdey.LiveServer)** clicando com o botão direito em `index.html` e escolhendo *"Open with Live Server"*.

---

## 💡 Próximos Passos e Melhorias Futuras

- [ ] Implementar interatividade com JavaScript para o formulário de Newsletter (validação e feedback visual).
- [ ] Adicionar funcionalidade de carrinho de compras com contagem de itens em tempo real.
- [ ] Criar páginas individuais de produtos e fluxo de checkout.
- [ ] Implementar carrossel/slider de novidades na seção Hero.
- [ ] Adicionar modo escuro (*Dark Mode*).

---

## 👨‍💻 Autor

Desenvolvido por **Rogério Silva**.

- **GitHub:** [@RSGames2019](https://github.com/RSGames2019)
- **Repositório do Projeto:** [ecommerce-syntaxwear](https://github.com/RSGames2019/ecommerce-syntaxwear)

---

<div align="center">
  <sub>Desenvolvido com foco no aprendizado prático de desenvolvimento web.</sub>
</div>
