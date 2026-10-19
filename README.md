# Lucas Guckert Design de Interiores

Site estático (index.html + img/) publicado no Cloudflare Pages: https://lucasguckert.pages.dev

## Publicação automática

Todo push na branch `main` publica o site no projeto `lucasguckert` do Cloudflare Pages
(workflow em `.github/workflows/deploy.yml`).

Configuração necessária (uma vez), em Settings › Secrets and variables › Actions:

- `CLOUDFLARE_ACCOUNT_ID`: ID da conta Cloudflare onde está o projeto `lucasguckert`
- `CLOUDFLARE_API_TOKEN`: token com permissão **Cloudflare Pages: Edit**

Para alterar o site: editar `index.html` (ou trocar imagens em `img/`), fazer commit e push.
