# 📚 Estudos de HTML e CSS — DevClub

Repositório com os meus estudos de **HTML5** e os primeiros passos em **CSS**, feitos durante as aulas do **DevClub**.

Cada arquivo trata de um tema: tem o código de exemplo e, logo abaixo, comentários (`<!-- -->`) explicando o conceito com as minhas próprias anotações. A ideia é servir de material de consulta rápida.

> 👤 **Autor:** Renan — estudante de Engenharia de Software e desenvolvimento web, com o objetivo de se tornar desenvolvedor **Full Stack**.
> 🔗 [LinkedIn](https://www.linkedin.com/in/renandev07/)

---

## 🗂️ Estrutura do projeto

```
AULAS DEV CLUB/
├── html/                        # Estudos de HTML (um tema por arquivo)
│   ├── estrutura.html
│   ├── tag.html
│   ├── tags-texto.html
│   ├── links.html
│   ├── listas.html
│   ├── imagens.html
│   ├── video.html
│   ├── iframe.html
│   ├── tabelas.html
│   ├── elementos estruturais.html
│   ├── forms.html
│   ├── input.html
│   ├── seo.html
│   └── desafio.html             # Desafio: página "Quem sou eu"
├── css/                         # Primeiros passos com CSS
│   ├── index.html
│   └── style.css
├── img/                         # Imagens usadas nos exemplos
└── README.md
```

---

## 🧭 Ordem sugerida de estudo

| # | Arquivo | Tema | O que é abordado |
|---|---------|------|------------------|
| 1 | [estrutura.html](html/estrutura.html) | Estrutura do documento | `<!DOCTYPE>`, `<html>`, `<head>`, `<body>`, `<meta charset>`, `<meta viewport>`, `<title>` |
| 2 | [tag.html](html/tag.html) | Anatomia de uma tag | Abertura, fechamento, conteúdo, pareamento e tags sem fechamento (`<img>`, `<input>`) |
| 3 | [tags-texto.html](html/tags-texto.html) | Tags de texto | Títulos `<h1>`–`<h6>`, `<p>`, `<br>`, `<b>`, `<strong>`, `<i>`, `<u>`, `<s>`, `<sub>`, `<sup>` |
| 4 | [links.html](html/links.html) | Links | `<a href>`, `target="_blank"`, `mailto:`, `tel:` e âncoras internas (`#id`) |
| 5 | [listas.html](html/listas.html) | Listas | `<ul>`, `<ol>` (tipos `1`, `A`, `a`, `I`, `i`), `<li>`, listas aninhadas e de definição (`<dl>`, `<dt>`, `<dd>`) |
| 6 | [imagens.html](html/imagens.html) | Imagens | `<img>`, `src`, `alt`, `width`/`height`, `title`, `loading="lazy"`, `<figure>` e `<figcaption>` |
| 7 | [video.html](html/video.html) | Vídeo | `<video>`, `controls`, `autoplay`, `muted`, `loop`, `poster`, `<source>` (mp4/webm) e legendas com `<track>` |
| 8 | [iframe.html](html/iframe.html) | Iframe | Incorporar YouTube, Google Maps e outras páginas; atributos `src`, `width`, `height`, `title`, `allowfullscreen` |
| 9 | [tabelas.html](html/tabelas.html) | Tabelas | `<table>`, `<tr>`, `<td>`, `<th>`, `<thead>`, `<tbody>`, `<tfoot>`, `<caption>`, `colspan`, `rowspan`, `scope`, exemplos práticos e desafio |
| 10 | [elementos estruturais.html](html/elementos%20estruturais.html) | Layout e semântica | `<div>`, `<span>`, `<header>`, `<nav>`, `<main>`, `<section>`, `<article>`, `<aside>`, `<footer>` |
| 11 | [forms.html](html/forms.html) | Formulários | `<form>`, atributos `action` e `method` (`GET` x `POST`) |
| 12 | [input.html](html/input.html) | Campos de entrada | `<input>`, `<label>` e tipos (`text`, `password`, `email`, `number`, `date`, `checkbox`, `radio`, `file`, `hidden`, `submit`); atributos `name`, `value`, `placeholder`, `required`, `disabled`, `readonly` |
| 13 | [seo.html](html/seo.html) | SEO | O que é *Search Engine Optimization* e por que ele importa |
| 14 | [desafio.html](html/desafio.html) | 🏆 Desafio | Página pessoal "Quem sou eu" juntando títulos, parágrafos, link, lista e imagem |
| 15 | [css/index.html](css/index.html) | 🎨 Introdução ao CSS | Ligar uma folha de estilo externa com `<link rel="stylesheet">` |

---

## 📝 Resumo dos principais conceitos

### Estrutura básica de uma página
```html
<!DOCTYPE html>
<html lang="pt-br">
<head>
    <meta charset="UTF-8">
    <meta name="viewport" content="width=device-width, initial-scale=1.0">
    <title>Minha página</title>
</head>
<body>
    <h1>Olá, mundo!</h1>
</body>
</html>
```

### Tags com e sem fechamento
- **Com fechamento:** `<p>texto</p>`, `<button>clique</button>`
- **Sem fechamento (vazias):** `<img>`, `<input>`, `<br>`, `<meta>`, `<link>`

### Links
```html
<a href="https://www.google.com" target="_blank">Abre em nova aba</a>
<a href="mailto:email@exemplo.com">Enviar e-mail</a>
<a href="tel:+5511999999999">Ligar</a>
<a href="#fim">Ir para o fim da página</a>
```

### Tabela bem estruturada
```html
<table>
    <caption>Notas</caption>
    <thead>
        <tr><th scope="col">Aluno</th><th scope="col">Nota</th></tr>
    </thead>
    <tbody>
        <tr><td>Renan</td><td>10</td></tr>
    </tbody>
    <tfoot>
        <tr><td colspan="2">Média: 10</td></tr>
    </tfoot>
</table>
```
> ⚠️ Tabela serve para **dados**, não para montar layout de página.

### Layout semântico
```html
<header> <nav>...</nav> </header>
<main>
    <section>
        <article>...</article>
    </section>
    <aside>...</aside>
</main>
<footer>...</footer>
```
- `<div>` → bloco genérico (ocupa a linha inteira)
- `<span>` → elemento em linha (agrupa pedaços de texto)

### Formulário
```html
<form action="/enviar" method="POST">
    <label for="username">Usuário:</label>
    <input type="text" id="username" name="username" required placeholder="Digite seu username">
    <input type="submit" value="Enviar">
</form>
```
- `GET` → dados vão na URL (buscas, filtros)
- `POST` → dados vão no corpo da requisição (login, cadastro)

---

## ▶️ Como visualizar

Não precisa instalar nada:

1. Baixe ou clone esta pasta.
2. Abra qualquer arquivo `.html` no navegador (duplo clique).
3. Para estudar, abra o mesmo arquivo no editor (ex.: **VS Code**) e leia os comentários.

💡 Dica: a extensão **Live Server** do VS Code atualiza a página sozinha a cada alteração salva.

---

## 🚀 Próximos passos

- [x] Fundamentos de HTML5
- [ ] CSS: seletores, cores, box model, Flexbox e Grid
- [ ] Responsividade (media queries)
- [ ] JavaScript
- [ ] Back-end e banco de dados → **Full Stack**

---

## 🛠️ Tecnologias

![HTML5](https://img.shields.io/badge/HTML5-E34F26?style=for-the-badge&logo=html5&logoColor=white)
![CSS3](https://img.shields.io/badge/CSS3-1572B6?style=for-the-badge&logo=css3&logoColor=white)
![VS Code](https://img.shields.io/badge/VS%20Code-007ACC?style=for-the-badge&logo=visualstudiocode&logoColor=white)

---

Feito com 💙 durante as aulas do **DevClub**.
