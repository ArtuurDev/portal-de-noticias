# Portal de Noticias

https://artuurdev.github.io/portal-de-noticias/

Projeto de uma pagina estatica de portal de noticias sobre tecnologia, construido com HTML e CSS puro.

## Preview

A pagina apresenta:

- cabecalho com menu, logo, busca e navegacao por categorias;
- area de noticias em destaque;
- secao com as noticias mais lidas da semana;
- lista de destaques sobre inteligencia artificial;
- barra lateral com anuncio e noticias complementares.

## Tecnologias

- HTML5
- CSS3
- CSS Grid
- CSS custom properties
- Fonte Archivo via Google Fonts

## Estrutura

```text
.
├── index.html
├── assets/
│   ├── icons/
│   ├── images/
│   ├── Ads.png
│   └── Logo.svg
└── styles/
    ├── index.css
    ├── global.css
    ├── header.css
    ├── sections.css
    └── utility.css
```

## Como executar

Este projeto nao precisa de instalacao de dependencias.

Abra o arquivo `index.html` diretamente no navegador ou use a extensao Live Server do VS Code.

## Arquivos CSS

- `styles/index.css`: importa todos os arquivos de estilo.
- `styles/global.css`: reset, variaveis globais, estilos base e layout principal.
- `styles/header.css`: estilos dos menus superior e secundario.
- `styles/sections.css`: estilos das secoes de noticias, cards e aside.
- `styles/utility.css`: classes utilitarias de grid, gaps e tipografia.

## Observacao sobre layout

O layout principal usa `grid-template-areas` para organizar as secoes:

```text
featured featured
weekly   weekly
ai       aside
```

Para que essa estrutura funcione corretamente, o elemento `main` precisa ter `display: grid`, seja diretamente no CSS ou por meio da classe utilitaria `grid` no HTML.
