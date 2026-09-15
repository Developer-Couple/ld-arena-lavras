# Handoff — Arena Lavras

Branch: `client/arena-beach-lavras` (worktree criado a partir de `main` do
template `beach-tennis-landing-page`).

## Cliente

- Nome: Arena Lavras
- Endereço: Rua Lucas Costa, 60, Portal da Mata, Lavras - MG
- Instagram: `@arena_lavras` (fonte das fotos)
- Celular/WhatsApp: (35) 99891-5177

## Já feito

- Nome do clube substituído em todo o `index.html`
  (`[Nome do Clube]` / `[NOME DO CLUBE]`).
- Endereço preenchido no card de localização e no embed do Google Maps
  (`SEU_ENDERECO_AQUI` → endereço URL-encoded), incluindo `[CIDADE-UF]`.
- Instagram preenchido (`SEU_INSTAGRAM` → `arena_lavras`).
- WhatsApp/telefone preenchidos (`SEUNUMERODEWHATSAPP` → `5535998915177`,
  `(00) 00000-0000` → `(35) 99891-5177`).
- Horário de atendimento preenchido no bloco de contato: Seg a Sáb 7h–12h e
  15h–22h, Dom 8h–12h.
- Hero: fundo do gradiente placeholder trocado por
  `uploads/img/fallback-mobile-hero.jpg` (imagem, usada em tablet/desktop e
  como fallback antes do vídeo carregar) + `uploads/video/video-mobile-hero.mp4`
  (`<video>` com `heroVideoRef`, autoplay/mudo/loop, só visível em
  `max-width:860px` via classe `.btc-hero-video`).
- Logo (`uploads/img/logo.png`) aplicada nos 4 lugares (nav, hero, card de
  localização, footer), substituindo o SVG placeholder.
- Foto de localização (`uploads/img/localizacao.jpg`) aplicada via
  `src` no `<image-slot id="location-photo">`.
- Design system recalibrado pra IDV da logo: `--color-accent` (laranja)
  e `--color-accent-2` (era azul-petróleo, virou verde) e suas escalas de
  tint/shade, no bloco `--color-*` logo após `</helmet>`. Reflete em CTA,
  bullets de modalidades, hover de cards e gradiente de fundo do hero.
- `pnpm run responsive-check` rodado — sem overflow horizontal em
  mobile/tablet/desktop.

## Pendente (faltam dados do cliente)

1. **Facebook** — busque `SEU_FACEBOOK` (ou remover o link se o cliente não
   tiver).
2. **Fotos** — `<image-slot>` de sobre, serviços, equipe e depoimentos
   seguem vazios; puxar do Instagram `@arena_lavras` e preencher.
3. Conferir números da seção "em números" (`statsTargets` no `<script>`
   final) e textos de serviços/depoimentos — hoje genéricos.

Assim que tiver Facebook/fotos/logo do cliente, aplicar as mesmas
substituições feitas para nome/endereço/Instagram/WhatsApp e rodar
`pnpm run responsive-check` de novo antes de enviar pro cliente.
