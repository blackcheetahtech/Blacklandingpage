# Black Cheetah — Landing Page

Site institucional da Black Cheetah. Página única, estática, sem build e sem dependências.

## Estrutura

```
index.html          página completa (HTML + CSS + JS inline)
assets/hero.webp    olho da marca — seção principal
assets/logo.webp    olho da marca — logo do cabeçalho
favicon.ico         ícone da aba
apple-touch-icon.png ícone ao salvar na tela inicial do iPhone
og-image.png        preview do link (WhatsApp, LinkedIn, Facebook)
robots.txt          liberação para indexação
.nojekyll           desliga o Jekyll no GitHub Pages
.htaccess           compressão e cache (só vale em Apache/LiteSpeed, ex.: Hostinger)
```

## Publicar no GitHub Pages

1. **Settings → Pages**
2. **Source:** Deploy from a branch
3. **Branch:** `main` — pasta `/ (root)` → **Save**

Em cerca de um minuto o site fica no ar em `https://<usuario>.github.io/<repositorio>/`.

## Domínio próprio

1. Crie um arquivo `CNAME` na raiz com uma única linha: `blackcheetah.com.br`
2. No painel do seu domínio, aponte:
   - `A` para `185.199.108.153`, `185.199.109.153`, `185.199.110.153`, `185.199.111.153`
   - `CNAME` de `www` para `<usuario>.github.io`
3. **Settings → Pages → Custom domain**, informe o domínio e marque **Enforce HTTPS**

## Depois que o domínio estiver no ar

Em `index.html`, troque a meta tag de preview pelo endereço completo — sem isso o WhatsApp não exibe a imagem do cartão:

```html
<meta property="og:image" content="https://blackcheetah.com.br/og-image.png">
```

## Editar

Abra o `index.html` em qualquer editor. Não existe etapa de build: salvou, commitou, o Pages republica sozinho.

Contato: (43) 98486-4326
