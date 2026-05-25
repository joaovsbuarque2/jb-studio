# JB Studio

Portfólio do JB Studio — estúdio digital focado em desenvolvimento de apps e sites modernos.

## Stack

- **Hugo** — gerador de site estático
- **Tailbliss** — tema Hugo com Tailwind CSS + Alpine.js
- **GitHub Pages** — hospedagem e deploy via GitHub Actions

## Desenvolvimento

```bash
# Instalar dependências do tema
cd themes/tailbliss && npm install

# Build do CSS
npx vite build --config themes/tailbliss/vite.config.mjs

# Servidor local
hugo server -D
```

## Deploy

O deploy é automático via GitHub Actions ao fazer push na branch `main`. O workflow:

1. Instala dependências e faz build do CSS
2. Executa `hugo --gc --minify`
3. Faz upload do artefato para GitHub Pages

## Estrutura

```
├── content/        # Páginas em Markdown
├── layouts/        # Templates HTML
├── assets/         # Imagens e assets
├── static/         # Arquivos estáticos (CSS compilado, etc.)
└── hugo.yaml       # Configuração principal do site
```
