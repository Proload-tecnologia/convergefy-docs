# convergefy-docs

Site publicado da **Central de Ajuda do Convergefy**: **https://docs.convergefy.com.br**

> **Não edite o site aqui.** Este repositório só hospeda o site já gerado. Os guias são escritos no repositório
> principal do Convergefy, na pasta `docs/`, e publicados aqui automaticamente.

## Para quem procura ajuda

- Guias: https://docs.convergefy.com.br
- Versão em texto, para agentes de IA:
  - [`llms.txt`](https://docs.convergefy.com.br/llms.txt): índice de todos os guias;
  - [`llms-full.txt`](https://docs.convergefy.com.br/llms-full.txt): todos os guias num arquivo só;
  - cada guia em markdown, no endereço `https://docs.convergefy.com.br/kb/<guia>.md`.

## Branches

| Branch | O que tem | Quem altera |
|---|---|---|
| `main` | Só este README. | Pessoas. A automação nunca toca nesta branch. |
| `gh-pages` | O site gerado (HTML, JS, `kb/*.md`, `llms.txt`), servido pelo GitHub Pages. | Só a automação. Cada publicação substitui a branch inteira por um único commit. |

## Como o site é publicado

1. Um push na `main` do repositório principal que altere `docs/` dispara o workflow `docs-pages-deploy`.
2. O workflow gera o site e cria um commit `deploy: convergefy@<sha>`, sem nenhum commit anterior. O `<sha>` identifica o
   commit de origem no repositório principal.
3. O commit inclui dois arquivos de configuração:
   - `CNAME`: na publicação por branch, é desse arquivo que o GitHub Pages lê o domínio próprio;
   - `.nojekyll`: desliga o Jekyll, para que os `.md` sejam servidos como estão, sem virar HTML.
4. O workflow faz push forçado na `gh-pages`, e o Pages republica o site.

A `gh-pages` não guarda histórico de propósito. Os arquivos gerados mudam de nome a cada build, então guardar histórico
só faria o repositório crescer a cada publicação. A história que importa é a dos guias, no repositório principal.

## Corrigir ou desfazer uma publicação

Corrija ou reverta no repositório principal. O próximo push na `main` publica a versão corrigida.

Não faça commit na `gh-pages`: ele é apagado na publicação seguinte.

## Configuração

- **Settings → Pages:** "Deploy from a branch", com `gh-pages` e `/ (root)`. Custom domain `docs.convergefy.com.br`,
  com "Enforce HTTPS".
- **DNS:** `CNAME docs → proload-tecnologia.github.io`, em **DNS only** (sem proxy). Com proxy, o GitHub
  não consegue emitir o certificado HTTPS.
- **Settings → Deploy keys:** uma chave com escrita, usada pelo workflow para publicar. A chave privada fica no secret
  `DOCS_PAGES_DEPLOY_KEY` do repositório principal. Para trocar a chave:
  1. gere um par novo;
  2. substitua a chave pública aqui e o secret lá;
  3. apague a chave antiga.
