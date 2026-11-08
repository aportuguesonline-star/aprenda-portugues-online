# LP Aprenda Português Online

Página única (`index.html`) com imagens em `img/`. Não precisa de build.

## Publicar (Netlify + GitHub)
1. Suba **o conteúdo desta pasta** para o repositório (o `index.html` fica na raiz do repo).
2. No Netlify: *Add new site → Import from Git*, escolha o repositório. Não há comando de build; a pasta publicada é a raiz (`netlify.toml` já diz isso).

## Endereço do site
O endereço já está preenchido (`aprendaportuguesonline.netlify.app`). Se um dia usar domínio próprio, troque-o nas 5 linhas do `<head>` do `index.html`.

## Configurar (bloco `window.APO` no `<head>` do index.html)
- `ga4`: ID do Google Analytics 4 (`G-XXXXXXX`).
- `metaPixel`: ID do Pixel da Meta.
- `ofertaFim`: último dia da oferta (`AAAA-MM-DD`). A página escreve "até DD/MM" na faixa e no cupom e, depois da data, esconde faixa, cupom, post-it de −10%, preços com desconto e a pergunta do FAQ sobre o desconto.

Todo clique em WhatsApp, e-mail ou Instagram gera o evento `clique_contato` (dataLayer), `generate_lead` (GA4) e `Contact` (Pixel), com o local da página e o plano.

## Preços
Estão no HTML, nas fichas de plano: `data-de` (preço cheio) e `data-conta` (preço com desconto), e no FAQ.
