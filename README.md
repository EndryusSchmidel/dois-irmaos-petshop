# Template de landing page — Pet Shop

Página única (`index.html`) usada como ponto de partida para landing pages de pet shops.
Feita para ser publicada em qualquer hospedagem estática (Netlify, GitHub Pages, Vercel) ou embutida
como HTML num site (ex.: elemento "Embed HTML" do Wix).

## Como reaproveitar para uma nova loja

1. Copie a pasta `landing/` inteira para o novo projeto (ou duplique dentro deste repo).
2. Troque a logo em `assets/logo.png`.
3. Em `index.html`, atualize:
   - `<title>` e a meta `description`.
   - Nome da loja (`.logo-texto`, cabeçalho e rodapé).
   - Texto do hero, seção "Sobre" e lista de produtos.
   - Número de WhatsApp nos links `wa.me/55...` e `tel:+55...`.
   - Endereço, CEP e o link do Google Maps (`href` do `.mapa` / `.mapa-card`).
   - Tabela de horários (`#horarios`) — os dias já se destacam sozinhos via JavaScript.
4. As cores ficam nas variáveis CSS no topo do `<style>` (`--roxo`, `--amarelo`, etc.) —
   troque pela paleta da nova marca.

## Notas

- O horário "Aberto agora / Fechado agora" é calculado no fuso de Brasília (`America/Sao_Paulo`),
  então funciona certo mesmo se o visitante estiver em outro fuso.
- O mapa usa um `<iframe>` do Google Maps (não funciona em pré-visualizações tipo Claude Artifacts —
  nesses casos, trocar por um cartão com link para o Maps, como foi feito na prévia enviada ao cliente).
