# Pet&Style — Loja Virtual Pet 🐾

Página inicial responsiva da loja virtual fictícia **Pet&Style**, desenvolvida com **HTML5** e **Tailwind CSS via CDN** seguindo a abordagem **utility-first** e **mobile-first** (`sm:`, `md:`, `lg:`).

## Estrutura do Repositório

```text
petstyle-loja-virtual/
├── index.html                  # Página principal estilizada com classes utilitárias do Tailwind CSS
├── README.md                   # Documentação do projeto
└── imagens/                    # Ilustrações vetoriais locais da loja e dos produtos
    ├── logo.svg
    ├── hero-pet.svg
    ├── produto-cama.svg
    ├── produto-coleira.svg
    ├── produto-moletom.svg
    └── produto-comedouro.svg
```

## Seções Desenvolvidas

1. **Header (`<header>`)**:
   - Logotipo fictício **Pet&Style** e menu de navegação estruturados com **Flexbox** (`flex`, `items-center`, `justify-between`, `gap-6`, `lg:gap-8`).
   - Navegação responsiva com menu retrátil para dispositivos móveis (`md:hidden`) e barra horizontal a partir de telas médias (`hidden md:flex`).
2. **Hero (`#inicio`)**:
   - Layout mobile-first (`flex flex-col lg:flex-row items-center justify-between gap-10 lg:gap-12`) com chamada principal, botões de ação empilhados no celular e lado a lado em `sm:flex-row`, indicadores de autoridade e imagem de destaque (`imagens/hero-pet.svg`).
3. **Produtos (`#produtos`)**:
   - Seção com **4 cards de produtos** utilizando **CSS Grid** responsivo (`grid grid-cols-1 sm:grid-cols-2 md:grid-cols-2 lg:grid-cols-4 gap-6 lg:gap-8`).
   - Cards construídos com Flexbox interno (`flex flex-col justify-between`), selos de destaque, avaliações, preços e botão interativo de adição à sacola.
4. **Depoimentos (`#depoimentos`)**:
   - Três relatos de clientes fictícios distribuídos em Grid (`grid grid-cols-1 md:grid-cols-2 lg:grid-cols-3 gap-6 lg:gap-8`), com classificação em estrelas e identificação do tutor e seu pet.
5. **Contato (`#contato`)**:
   - Canais diretos de atendimento (**E-mail**, **Telefone/WhatsApp** e **Endereço**) combinados a um **formulário simples** com campos de Nome, E-mail, Telefone, Pet e Mensagem estilizados com utilitários de borda, espaçamento e foco (`focus:border-orange-500`, `focus:ring-2`).

## Breakpoints Mobile-First Aplicados

- **Base (Mobile `< 640px`)**: Layout em coluna única (`grid-cols-1`, `flex-col`), menu hambúrguer compacto e tipografia ajustada (`text-3xl`).
- **`sm:` (`>= 640px`)**: Botões do Hero alinhados em linha (`sm:flex-row`), grade de produtos e diferenciais em 2 colunas (`sm:grid-cols-2`) e campos do formulário divididos em duas colunas.
- **`md:` (`>= 768px`)**: Exibição do menu de navegação horizontal (`md:flex`), cabeçalhos expandidos (`md:text-5xl`) e grade de depoimentos em 2 colunas (`md:grid-cols-2`).
- **`lg:` (`>= 1024px`)**: Hero dividido em duas colunas (`lg:flex-row`), grade de produtos em 4 colunas (`lg:grid-cols-4`), grade de depoimentos em 3 colunas (`lg:grid-cols-3`) e seção de contato em 12 colunas (`lg:grid-cols-12`).
