# Paola Pax — site pessoal

Site pessoal da Paola Pax (Paola Giavina Bianchi) — moodboard, projetos e
contato comercial. Identidade 100% dela, sem qualquer marca ou menção ao
The Watermouse no conteúdo visível; a hospedagem apenas reaproveita a infra
de domínio já existente.

## Stack

HTML/CSS/JS puro, um único `index.html`, sem build tool. Toggle PT/EN via
atributos `data-pt` / `data-en` + `localStorage`.

## O que já é real

- Nome, handles e links: TikTok [@apaolapax](https://www.tiktok.com/@apaolapax),
  Instagram [@paolabianchi](https://instagram.com/paolabianchi)
- Números do hero (seguidores/curtidas do TikTok) — **atualizar periodicamente**,
  foram capturados em 28/09/2026
- Base em São Paulo, audiência internacional (BR/MX/FR/UK) — vem da bio pública do TikTok

## O que é placeholder (marcar com a Paola antes de publicar)

1. **Fotos reais** — todo bloco com a etiqueta "+ foto" no moodboard (`#moodboard`)
   e o retângulo "foto a adicionar" em `#sobre` precisam virar `<img>` de verdade.
   Nunca embutir em base64 — sempre arquivo referenciado (ex: `fotos/mood-1.jpg`).
2. **Bio** (`#sobre`) — o primeiro parágrafo usa só fatos confirmados; a frase em
   itálico logo abaixo é o aviso de "complete aqui" e deve ser apagada quando o
   texto de verdade entrar.
3. **Projetos** (`#projetos`) — os dois cards tracejados ("+ Próximo projeto" /
   "+ Trabalho anterior") são vagas para trabalhos reais (marcas, parcerias, arte).
4. **E-mail de contato** (`#contato`) — hoje só tem os links de DM. Se ela quiser
   um e-mail dedicado, adicionar e trocar a nota "adicionar endereço aqui".
5. **Idioma** — o toggle já funciona ponta a ponta; só revisar a tradução quando
   o texto real (bio, projetos) for definido.

## Deploy

1. Criar o repo em `thewatermouse/paolapax` (GitHub Pages, branch `main`).
2. Push do conteúdo desta pasta.
3. Settings → Pages → confirmar custom domain `paolapax.thewatermouse.com`
   (o arquivo `CNAME` já está no repo).
4. No Cloudflare (zona `thewatermouse.com`), criar registro `CNAME` —
   `paolapax` → `thewatermouse.github.io` (proxy Cloudflare pode ficar ligado).
5. Aguardar o certificado HTTPS do GitHub Pages (alguns minutos após o DNS propagar).
