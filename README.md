# Estudo e criações referentes a **HTML** e **CSS**

##  Motivo do repositório?
O repositório tem o intuito de documentar meus estudos sobre o que eu aprendi sobre HTML e CSS, sem nenhuma intenção para fins financeiros.

---
<h2 align="center" ><b>HTML</b></h2>
### Tags

- `<html>`É a raiz do documento, avisa para o dom que o arquivo vai ser um arquivo html;
- `<head>`É a representação dos metadados onde se pode incluir links ;
- `<body>` É a representação do corpo do html onde irão conter os dados principais;

```html
<html lang="pt-br">
    <head>
        <meta charset="utf-8">
        <title> HTML</title>
        <meta name="description" content="HTML, CSS, JavaScript">
        <meta name="author" content="Gui Seek">
        <link rel="stylesheet" href="style.css">
    </head>
    <body>
        Informação da paǵina
    </body>
</html>
```

- `<title>` É a tag que define o titulo do documento onde é apresentado no titulo do navegador ou na guia da página;
```html
    <head>
	<title>Nome do siste</title>
    </head>
```

- `<base>` Define a URL base para a URL da página relativa;
```html
    <base href="https://www.exemplo.com/">
    <base target="_blank">
    <base target="_top" href="https://exemplo.com/">
```

- `<link>` É mais utilizada para linkar arquivos externos, tende a ser utilizada geralmente para linkar arquivos CSS;
```html
    <head>
    <meta charset="UTF-8">
	  <title>Mentoria com Luciane</title>
     <link rel="stylesheet" type="text/css" href="styles.css">             
    </head>
```
- `<meta>`Define os metadados que não podem ser  definidas usando outro elemento HTML;
```html
    <head>
    <meta charset="UTF-8">
```

- `<style>` É utilizada para escrever CSS dentro de um documento HTML;
```html
    <style>
      body {
         font-family: Poppins;
         font-size: 20px;
         background-color: #FFF;
      }
    </style>
```

- `<script>` Define um script interno e também pode ser um link para um script externo e sua linguagem é JavaScript;
```html
    <script type="text/javascript" src="js/arquivo.js"></script>
    <script>
     alert("Olá, amigos!");
    </script>
```

- `<noscript>` Define um conteúdo alternativo a ser exibido, acontece quando o navegador não suporta o scripts ou se o script está desativado no navegador.
```html
    <noscript>
    <a href="http://www.github/erickcelestino/">Link Externo</a>    
    </noscript>
    <p>Informações</p>
```
- `<template>` É um container para manter algum conteúdo HTML oculto do usuário no momento que a página é carregada. O conteúdo dentro de template pode ser renderizado posteriormente com JavaScript;
```html
 <button onclick="showContent()">Fazer dados aparecer</button>

<template>
  <h2>Imagem aleatória</h2>
  <img src="imagem_aleatoria.jpg">
</template>

<script>
function showContent() {
  var temp = document.getElementsByTagName("template")[0];
  var clon = temp.content.cloneNode(true);
  document.body.appendChild(clon);
}
</script> 
```

- `<section>`Define uma seção em um documento HTML;
```html
    <section>
        <div>
            <p>Seção criada com sucesso</p>
        </div>
    </section>
```

- `<nav>` Define uma seção que contém apenas links para navegação;
```html
    <nav>
        <ul>
            <li><a href="https://w3c.org">W3C</a></li>
            <li><a href="https://whatwg.org">Meetups</a></li>
            <li><a href="https://github.com">GitHub</a></li>
            <li><a href="https://twitter.com">Twitter</a></li>
        </ul>
    </nav>
```

- `<article>` Define que pode existir de forma idenpendente do resto do conteúdo. Está tag poderia ser um post de um blog, fórum, um artigo de revista ou jornal;
```html
    <article>
    <p>Texto 1</p>
    <p>Texto 2</p>
    </article>
```

- `<aside>` Define um conteúdo reservado do resto do conteùdo da página. Caso for removida, o conteudo ainda continua fazendo sentido, em si seria algo complementar;
```html
    <section>
      <h3> Artigo ilustrativo</h3>
           <img src="imagens.png" width="350" alt="Imagem ilustrativa">
           <figcaption hidden>Imagem ilustrativa</figcaption>
       </a>
       <aside>
           <p>Texto desenvolvendo a ideia sobre o conteúdo</p>
       </aside>
   </section>

```

- `<hgroup>` Agrupa um conjunto de elementos de `<h1>` a `<h6>` quano um titulo tem vários niveis;
```html
    <body>
        <header>
            <hgroup>
                <h1>Programação</h1>
                <h2>Porque programar?</h2>
            </hgroup>
        </header>
    </body>
```

- `<header>` Define o cabeçalho de uma página ou seção. Muitas vezes contém um logo, titulo do site um menu de navegação do conteúdo;
```html
    <header class="cabecalho">
        <figure class="cabecalho__logo">
            <img src="https://www.imagem.com/" width="84" alt="Logo da pagina">
            <figcaption hidden>Logo da pagina</figcaption>
        </figure>
        <hgroup>
            <h1>Descrição</h1>
            <h2>Corpo da requisição</h2>
        </hgroup>
    </header>

```

---

## Referencias

- <a href="https://guiseek.notion.site/Elementos-do-HTML-na-pr-tica-1f83decf102a4edcbdee81eafefc2175">Elementos do HTML na prática</a>
- <a href="https://www.w3schools.com">W3schools</a>
