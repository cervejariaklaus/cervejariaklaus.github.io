# Landing page — Cervejaria Klaus (Kapitän Klaus)

Site estático. Suba o conteúdo desta pasta na raiz do domínio.

## Antes de publicar
1. Troque `https://SEU-DOMINIO.com.br` pelo domínio final (https, com ou sem www) em `index.html`:
   - Linux/macOS: `sed -i 's#https://SEU-DOMINIO.com.br#https://DOMINIO-FINAL#g' index.html`
   - Afeta: `canonical`, `og:url`, `og:image`, `twitter:image` e o JSON-LD.
2. Confirme que o (31) 2942-3090 abre conversa no WhatsApp.

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
