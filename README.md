# Landing page — Cervejaria Klaus (Kapitän Klaus)

Site estático. Suba o conteúdo desta pasta na raiz do domínio.

## Domínio
Configurado para **https://cervejariaklaus.github.io/** (GitHub Pages, raiz do repositório `cervejariaklaus.github.io`).
Se migrar para domínio próprio, troque nas tags `canonical`, `og:url`, `og:image`, `twitter:image` e no JSON-LD de `index.html`:
`sed -i 's#https://cervejariaklaus.github.io#https://NOVO-DOMINIO#g' index.html`

## Antes de divulgar
Confirme que o (31) 2942-3090 abre conversa no WhatsApp.

## Arquivos
- `index.html` — página (CSS e JS embutidos, sem dependências além do Google Fonts)
- `img/` — imagens em WebP · `video/` — hero (desktop e mobile, sem áudio)
- `og-klaus.jpg` (1200×630), `favicon.ico`, `favicon-32.png`, `apple-touch-icon.png`, `icon-192.png`, `icon-512.png`
- `robots.txt`, `404.html` (configure o servidor para usá-la em erros 404)

## Checklist pós-publicação
- [ ] `/robots.txt` abre na URL pública e não bloqueia o site
- [ ] `canonical` e `og:url` apontam para o domínio final
- [ ] `/og-klaus.jpg` abre por URL absoluta; prévia testada no WhatsApp (ou depurador do Facebook/Meta)
- [ ] JSON-LD sem erros no Rich Results Test / Schema Markup Validator
- [ ] Ícone do WhatsApp e botão do formulário abrem a conversa com a mensagem correta
- [ ] Lighthouse mobile (Performance, Acessibilidade, SEO, Boas Práticas) revisado
- [ ] Menu (gaveta) e formulário testados no celular; vídeo da hero toca sem som
