# redirect-apex

Redireciona `magofy.com.br` (sem www) para `https://www.magofy.com.br`, mantendo caminho e parâmetros.
Publicado no GitHub Pages (repositório público, só tem esta página; nada sensível).

- `index.html` e `404.html`: mesma página. A `404.html` atende qualquer caminho (ex.: `/caxambu/`).
- `CNAME`: o domínio do Pages.
- DNS (KingHost): `A @` para 185.199.108.153, .109.153, .110.153 e .111.153. O `www` é CNAME para o Cloudflare Pages (site-magofy.pages.dev), não muda.
- Limite: é redirecionamento por página (JS + meta refresh), não 301 de servidor. O Google segue, e o endereço sem www quase não tem tráfego próprio.
- Por que não a KingHost: a raiz do domínio lá cai numa página padrão "Site em construção", fora da pasta /www (protocolos 261115559680 e 261115559708, 15/11/2026).
- Voltar atrás: `A @` para 185.158.133.1 (Lovable).
