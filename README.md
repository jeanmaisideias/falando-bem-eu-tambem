# Falando Bem, Eu Também — Landing page

Landing page do curso em videoaulas **Falando Bem, Eu Também**, de Vanesca Vanzuita (fonoaudióloga).
Site estático: HTML + CSS + JS puro, sem build e sem dependências. Fonte Montserrat via Google Fonts.

## Estrutura
```
index.html          página completa (10 seções + rodapé)
assets/img/         imagens otimizadas (.webp com fallback .jpg) e logo
```

## Configuração rápida
No fim do `index.html`, bloco `CONFIG`:
- `checkoutUrl` — checkout oficial da Hotmart (oferta `5weua4dl`)
- `checkoutSource` — valor enviado no parâmetro `sck` para identificar vendas desta página
- `youtubeId` — vídeo de apresentação
- `price` — valor usado nos eventos de conversão

As UTMs da visita (`utm_*`, `src`, `xcod`, `sck`) são repassadas automaticamente para o checkout.

## Rastreamento (pendente)
Inserir no `<head>` somente com IDs reais: Google Tag Manager, GA4 e Meta Pixel.
Eventos já prontos: `fbet_cta_click`, `fbet_checkout_click`, `fbet_view_offer`, `fbet_video_play` (dataLayer),
`begin_checkout` / `view_item` (gtag), `InitiateCheckout` / `ViewContent` (fbq). Compra (Purchase) fica com a Hotmart.

## Pendências de conteúdo
- Seção 03: ilustração provisória `assets/img/placeholder-atividade.svg` (substituir por foto autorizada de adulto e criança brincando)
- Seção 07: ilustração provisória `assets/img/placeholder-conexao.svg` (substituir por foto autorizada de família em interação espontânea)
- Seção 10: foto existente `vanesca.webp` / `vanesca.jpg` reaproveitada no fechamento; avaliar nova foto posteriormente
- Política de privacidade e termos de uso
- IDs de GTM, GA4 e Meta Pixel

Os pontos de troca estão marcados no HTML com comentários `ILUSTRAÇÃO PROVISÓRIA` / `FOTO EXISTENTE`. Os SVGs são recursos ilustrativos e não retratam clientes reais.

## Publicação
Funciona em qualquer hospedagem estática (GitHub Pages, Netlify, Cloudflare Pages).
No GitHub Pages: Settings → Pages → Deploy from branch → `main` / root.
