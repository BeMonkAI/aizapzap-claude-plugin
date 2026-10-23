# AIZapZap no Claude Code

Plugin para configurar e administrar sua conta [AIZapZap](https://aizapzap.com.br) conversando com o Claude: perfil, horários, cardápio ou catálogo, agentes de IA, equipe e serviços. Também traz uma configuração guiada, passo a passo, e responde dúvidas sobre o produto.

## O que você precisa

- Uma conta no AIZapZap com um estabelecimento criado (https://aizapzap.com.br).
- O Claude Code instalado. Veja como instalar em https://docs.claude.com/en/docs/claude-code/setup.

## Instalação (uma vez só)

1. Abra o Claude Code no terminal:

   ```
   claude
   ```

2. Adicione o catálogo de plugins do AIZapZap:

   ```
   /plugin marketplace add BeMonkAI/aizapzap-claude-plugin
   ```

3. Instale o plugin:

   ```
   /plugin install aizapzap@aizapzap
   ```

4. Reinicie o Claude Code (feche e abra de novo) para o plugin carregar.

## Primeiro acesso: login na sua conta

1. No Claude Code, digite `/mcp`, escolha **aizapzap** e depois **Authenticate**.
2. O navegador abre o AIZapZap. Entre com o seu e-mail e senha de sempre (ou com o Google).
3. Aparece a tela "Permitir acesso à sua conta AIZapZap?" mostrando quem pede o acesso, a sua conta e os seus estabelecimentos. Confira e clique em **Permitir**.
4. Pronto: volte para o Claude Code. O acesso fica salvo e é renovado sozinho.

## Como usar

- Para configurar a conta do zero ou ver o que falta:

  ```
  /aizapzap:configurar
  ```

  O Claude mostra um checklist e vai com você um passo por vez. Dá para parar e continuar outro dia, ele sempre recomeça de onde a conta está.

- Para ajustar algo, é só pedir. Exemplos:
  - "Muda meu horário de sábado para 9h às 14h."
  - "Adiciona no cardápio: pizza margherita, R$ 45."
  - "Deixa a IA mais formal e com respostas mais curtas."
  - "Liga o agente de agendamento."

- Para tirar dúvidas, também é só perguntar. Exemplos:
  - "Como funciona a fidelidade?"
  - "Por que a IA não respondeu a cliente Maria ontem?"
  - "Onde eu conecto o Instagram?"

## Mais de um estabelecimento

Se a sua conta tem vários estabelecimentos, o Claude pergunta qual você quer mexer. Para trocar, diga o nome do outro ("agora no da Vila Mariana").

## O que o Claude não faz

Por segurança, estas ações continuam só no painel do AIZapZap:

- cobrança, plano e créditos;
- conectar ou desconectar o WhatsApp e o Instagram;
- convidar ou remover pessoas da conta;
- apagar qualquer dado;
- mandar mensagens ou campanhas para os seus clientes;
- trocar o tipo de negócio do estabelecimento.

Reservas, agendamentos e pedidos podem ser consultados pelo Claude, mas criar ou alterar é no painel.

Antes de cada alteração, o Claude Code pede a sua permissão. Toda alteração feita por aqui fica registrada na sua conta.

## Desinstalar e revogar o acesso

1. No Claude Code: `/mcp`, escolha **aizapzap** e **Clear authentication**.
2. Remova o plugin:

   ```
   /plugin uninstall aizapzap@aizapzap
   ```

## Suporte

Dúvidas ou problemas: use a tela de Suporte no painel, em https://aizapzap.com.br/dashboard/support.
