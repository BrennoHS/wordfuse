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

## Estrutura
- `index.html` — página completa (HTML + CSS + JS + dicionários embutidos).

## Como adicionar palavras

O dicionário de cada idioma está no objeto `DICTIONARIES` dentro da tag `<script>` do `index.html`. Basta adicionar strings novas ao array do idioma desejado (ou pares `[palavra, romaji]` no caso do japonês).

## Licença

Sinta-se livre para usar, modificar e distribuir.
