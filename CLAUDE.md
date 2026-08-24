# Instruções do projeto

## Preview local (`http://localhost:8934`)

Este projeto é um site estático de arquivo único (`index.html`). Pra visualizar localmente, o servidor é configurado em `.claude/launch.json` (na pasta raiz da sessão do Claude Code, não neste repo) usando um script Node simples (`static-server.js` em scratchpad) servindo esta pasta na porta 8934.

**Regra importante: não derrubar o servidor de preview (`preview_stop`) depois de usá-lo para verificação própria.** O usuário costuma querer conferir as mudanças no navegador dele logo em seguida, então:

- Depois de verificar uma mudança no preview, **deixe o servidor rodando**.
- Só derrube o servidor se o usuário pedir explicitamente, ou no fim da sessão.
- Se o servidor cair por qualquer motivo (reinício de sessão, etc.) e o usuário disser que não consegue acessar `localhost:8934`, recrie o `.claude/launch.json` e rode `preview_start` de novo sem perguntar — é uma ação de baixo risco e o usuário já pediu isso várias vezes.

## Fluxo de git deste projeto

- Cada mudança de conteúdo/design vira uma branch nova (`git checkout -b nome-da-mudanca`), nunca commit direto na `main`.
- Peça aprovação do usuário antes de commitar quando ele estiver revisando uma mudança grande (ex.: "não commit nada ainda antes de eu aprovar").
- Depois do commit, pergunte se o usuário quer subir (`git push`), abrir PR (`gh pr create`) e mesclar — normalmente ele pede as três coisas em sequência.
- Depois do merge, confirme o rebuild do GitHub Pages (`gh api repos/WanderTerra/lp-adriana-alvarenga/pages/builds/latest`) antes de avisar que está no ar, e sincronize a `main` local (`git checkout main && git pull`).
- **Bash tem um bug conhecido nesta pasta** (falha ao criar/gravar arquivos, provavelmente por causa da sincronização do OneDrive) — use PowerShell para qualquer `git add/commit/push/checkout` ou criação de arquivo dentro deste repositório.

## Pendências do site

Ver [DUVIDAS-CLIENTE.md](DUVIDAS-CLIENTE.md) para a lista de decisões/dados ainda pendentes com a Dra. Adriana.
