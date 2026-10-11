# M&G Teck — site estático

O site pronto fica na raiz do repositório: `index.html`, `styles.css`, `app.js`, `config.js`, páginas legais e `assets/`.

Não é necessário instalar dependências nem executar build para publicar esta versão.

## Vercel

- Root Directory: raiz do repositório (deixar em branco).
- Framework Preset: Other.
- Build Command: vazio; ativar Override e deixar o campo vazio caso exista um comando antigo.
- Output Directory: `.`.
- Install Command: vazio, conforme `vercel.json`.

## Netlify

- Base directory: raiz (em branco ou `.`).
- Package directory: em branco.
- Build command: vazio.
- Publish directory: `.`.

As configurações estão em `vercel.json` e `netlify.toml`. Após alterar configurações antigas no painel, publicar novamente a branch `main`.

## Arquivos preservados

A pasta `smartsolutions/` mantém o código-fonte original em `public/`, os scripts em `scripts/`, o `package.json` e sua documentação. O conteúdo de `smartsolutions/dist/` foi movido para a raiz, sem alterações de design ou conteúdo.

O script original de build não apaga nem sobrescreve os arquivos do site na raiz, mas não deve ser usado pelas hospedagens nesta estrutura. Para atualizar o site publicado, editar os arquivos da raiz.
