# Estrutura do portfólio

```text
portfolio_organizado/
├── index.html
├── projetos.html
├── curriculo.pdf
├── css/
│   └── style.css
├── js/
│   └── components.js
└── projetos/
    └── modelo-projeto.html
```

## Header e footer

O arquivo `js/components.js` cria o header e o footer padrão.

Em páginas na raiz:

```html
<body data-page="index" data-root=".">
```

Em páginas dentro da pasta `projetos`:

```html
<body data-page="projetos" data-root="..">
```

Todas as páginas devem conter:

```html
<div data-component="header"></div>
...
<div data-component="footer"></div>
```

E carregar o JavaScript no final:

```html
<script src="js/components.js"></script>
```

Dentro da pasta `projetos`, use:

```html
<script src="../js/components.js"></script>
```

Altere no arquivo `js/components.js`:

- `SEU-USUARIO`
- `SEU-EMAIL`
- link do LinkedIn
