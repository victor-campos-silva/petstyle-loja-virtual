# Pet&Style — Loja Virtual Pet 🐾

Página inicial responsiva da loja virtual fictícia **Pet&Style**, desenvolvida com **HTML5** e **Tailwind CSS via CDN** seguindo a abordagem **utility-first** e **mobile-first** (`sm:`, `md:`, `lg:`).

## Estrutura do Repositório

```text
petstyle-loja-virtual/
├── index.html                  # Página principal estilizada com classes utilitárias do Tailwind CSS
├── README.md                   # Documentação do projeto
└── imagens/                    # Fotografias de estúdio e ilustrações locais da loja e dos produtos
    ├── logo.svg
    ├── hero-pet.jpg
    ├── produto-cama.jpg
    ├── produto-coleira.jpg
    ├── produto-moletom.jpg
    └── produto-comedouro.svg
```

## Seções e Funcionalidades Desenvolvidas

1. **Header (`<header>`)**:
   - Logotipo fictício **Pet&Style** e menu de navegação estruturados com **Flexbox** (`flex`, `items-center`, `justify-between`, `gap-6`, `lg:gap-8`).
   - Navegação responsiva com menu retrátil para dispositivos móveis (`md:hidden`) e barra horizontal a partir de telas médias (`hidden md:flex`).
   - **Botão Sacola Funcional (`#btnCarrinho`)**: Abre um painel lateral interativo (*Drawer*) com lista de produtos adicionados, controle de quantidade (`+`/`-`), exclusão de itens, barra de progresso para **Frete Grátis**, cálculo automático de subtotal/total e finalização de pedido.
2. **Hero (`#inicio`)**:
   - Layout mobile-first (`flex flex-col lg:flex-row items-center justify-between gap-10 lg:gap-12`) com chamada principal, botões de ação empilhados no celular e lado a lado em `sm:flex-row`, indicadores de autoridade e fotografia de destaque (`imagens/hero-pet.jpg`) com selos flutuantes responsivos em HTML/Tailwind.
3. **Produtos (`#produtos`)**:
   - Seção com **4 cards de produtos** utilizando **CSS Grid** responsivo (`grid grid-cols-1 sm:grid-cols-2 md:grid-cols-2 lg:grid-cols-4 gap-6 lg:gap-8`) e filtro interativo por categoria.
   - Cards construídos com Flexbox interno (`flex flex-col justify-between`), fotos de estúdio, selos de destaque, avaliações, preços e botão de adição à sacola.
4. **Depoimentos (`#depoimentos`)**:
   - Três relatos de clientes fictícios distribuídos em Grid (`grid grid-cols-1 md:grid-cols-2 lg:grid-cols-3 gap-6 lg:gap-8`), com classificação em estrelas e identificação do tutor e seu pet.
5. **Contato (`#contato`)**:
   - Canais diretos de atendimento (**E-mail**, **Telefone/WhatsApp** e **Endereço**) combinados a um **formulário simples** com campos de Nome, E-mail, Telefone, Pet e Mensagem estilizados com utilitários de borda, espaçamento e foco (`focus:border-orange-500`, `focus:ring-2`).
