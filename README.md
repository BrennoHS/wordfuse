# 💣 WordFuse

Dicionário de sílabas em tempo real para **Bomb Party**, **Word Bomb** e **Word Party**.

Digite uma sílaba e encontre instantaneamente palavras compostas e raras — feito para impressionar (ou detonar) seus amigos no jogo.

## Idiomas suportados
- 🇧🇷 Português
- 🇺🇸 English
- 🇪🇸 Español
- 🇫🇷 Français
- 🇮🇹 Italiano
- 🇯🇵 日本語

## Como rodar

É um único arquivo HTML autocontido — sem build, sem dependências além das fontes do Google Fonts.

```bash
# Só abrir no navegador
open index.html
```

Ou publique com **GitHub Pages**:
1. Vá em `Settings > Pages` no seu repositório.
2. Em "Source", selecione a branch `main` e a pasta `/root`.
3. Salve — o site fica disponível em `https://SEU-USUARIO.github.io/NOME-DO-REPO/`.

## SEO e indexação no Google

O repositório já vem pronto para indexação, sem precisar de domínio próprio:

- `sitemap.xml` e `robots.txt` na raiz, apontando para `https://brennohs.github.io/wordfuse/`.
- Meta tags de SEO (description, keywords, Open Graph, canonical, hreflang) já no `index.html`.

Depois de publicar no GitHub Pages:

1. Acesse [Google Search Console](https://search.google.com/search-console) e adicione a propriedade `https://brennohs.github.io/wordfuse/`.
2. Verifique a propriedade (o Search Console oferece um método de verificação por meta tag HTML — cole a tag que ele fornecer dentro do `<head>` do `index.html`).
3. Em "Sitemaps", envie `sitemap.xml`.
4. Use "Inspeção de URL" para pedir indexação manual da página inicial (acelera o processo).
5. Indexação costuma levar de alguns dias a poucas semanas depois disso.

Domínio próprio **não é necessário** — o `github.io` funciona normalmente para indexação. Um domínio custom (via `CNAME`) só ajuda com branding/memorização, não é requisito técnico para o Google indexar.

## Estrutura
- `index.html` — página completa (HTML + CSS + JS + dicionários embutidos).
- `sitemap.xml` — mapa do site para o Google.
- `robots.txt` — permissões de rastreamento.


## Como adicionar palavras

O dicionário de cada idioma está no objeto `DICTIONARIES` dentro da tag `<script>` do `index.html`. Basta adicionar strings novas ao array do idioma desejado (ou pares `[palavra, romaji]` no caso do japonês).

## Licença

Sinta-se livre para usar, modificar e distribuir.
