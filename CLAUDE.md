# aizapzap-claude-plugin

Plugin público do AIZapZap para o Claude Code: skills `configurar` e `ajuda` (guia por tela em `plugins/aizapzap/skills/ajuda/guia/`) e o `.mcp.json` que aponta para o MCP remoto. As ferramentas vivem no repo `BeMonkAI/aizapzap` (`supabase/functions/mcp/registry.ts`) e chegam ao usuário com o deploy de lá, sem mudar nada aqui.

## Regras

- **Nunca pôr `version` em `plugin.json` nem em `marketplace.json`.** Sem ela o Claude Code versiona pelo SHA do commit e todo merge na `main` chega a quem atualiza. Com `version` fixa, o usuário fica no cache até a string mudar (foi o que aconteceu com 0.1.0 entre 23/10 e 26/10/2026).
- O guia descreve o que está em **produção** (`origin/main` do `aizapzap`), não o `development`.
- Mudou tela, rótulo, limite ou plano no painel? Atualizar a página do guia correspondente, a seção `## English` dela e o `guia/index.md` se a tela for nova.
- Cada página segue o mesmo molde: Link, Para quem, Para que serve, Como usar, Dúvidas comuns, Pelo Claude, English.
- Sem travessão nos textos do guia.
