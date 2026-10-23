# AIZapZap no Claude Code

Plugin para configurar e administrar sua conta [AIZapZap](https://aizapzap.com.br) conversando com o Claude: perfil, horários, cardápio ou catálogo, agentes de IA, equipe e serviços. Também traz uma configuração guiada, passo a passo, e responde dúvidas sobre o produto.

## O que você precisa

- Uma conta no AIZapZap com um estabelecimento criado (https://aizapzap.com.br).
- Um destes: o app do Claude no computador (recomendado), o chat do Claude (claude.ai, app ou celular) como conector, o VS Code com a extensão Claude Code, ou o Claude Code no terminal (também é o caminho na JetBrains).

O passo a passo também está no painel do AIZapZap, em Integrações, no cartão "Administre sua conta com o Claude", com botão de copiar cada comando.

## No app do Claude (recomendado)

1. Instale o app do Claude no computador (https://claude.com/download), abra a aba **Code** e comece uma sessão local. Pode escolher qualquer pasta.
2. No campo de mensagem, cole e envie:

   ```
   /plugin marketplace add BeMonkAI/aizapzap-claude-plugin
   ```

3. Depois cole e envie:

   ```
   /plugin install aizapzap@aizapzap
   ```

   O plugin passa a aparecer em **+ › Plugins**, onde dá para ligar, desligar ou remover.
4. Faça o login na sua conta: envie `/mcp`, escolha **aizapzap** e entre. O navegador abre o AIZapZap: entre com o seu e-mail e senha de sempre (ou com o Google) e clique em **Permitir**.
5. Comece com `/aizapzap:configurar`.

## No VS Code

1. Instale a extensão **Claude Code** no VS Code e abra o painel do Claude.
2. No campo de mensagem, digite `/plugins`. Abre a tela de plugins.
3. Na aba **Marketplaces**, adicione `BeMonkAI/aizapzap-claude-plugin`.
4. Na aba **Plugins**, procure **aizapzap**, clique em **Install** e escolha **Install for you**. Não precisa reiniciar.
5. Faça o login: digite `/mcp`, escolha **aizapzap** e **Manage OAuth authentication**, entre na conta e clique em **Permitir**. Se o login não concluir pelo painel, abra o terminal integrado do VS Code e siga o passo 4 da seção do terminal abaixo; o login vale para os dois.
6. Comece com `/aizapzap:configurar`.

## No terminal ou na JetBrains

Na JetBrains (IntelliJ, PyCharm, WebStorm...), o plugin do Claude Code roda o Claude Code no terminal da IDE, então os passos são estes. Instale o Claude Code antes (https://docs.claude.com/en/docs/claude-code/setup).

1. Abra o Claude Code:

   ```
   claude
   ```

2. Adicione o catálogo de plugins do AIZapZap:

   ```
   /plugin marketplace add BeMonkAI/aizapzap-claude-plugin
   ```

3. Instale o plugin e reinicie o Claude Code (feche e abra de novo):

   ```
   /plugin install aizapzap@aizapzap
   ```

4. Login: digite `/mcp`, escolha **aizapzap** e depois **Authenticate**. No navegador, entre na conta e clique em **Permitir**.
5. Comece com `/aizapzap:configurar`.

Instalou num lugar, vale nos outros: o plugin instalado para você (escopo de usuário) aparece no app do Claude, no VS Code e no terminal do mesmo computador.

## No claude.ai ou no app do Claude, como conector (sem instalar plugin)

Para usar numa conversa normal do Claude, no navegador ou no app, sem a aba Code. Assim você tem as ferramentas do AIZapZap, mas não os comandos `/aizapzap:configurar` e o guia de ajuda do plugin: é só pedir em português.

1. Abra **Configurações › Conectores** (https://claude.ai/settings/connectors) e clique em **Adicionar conector personalizado**.
2. Dê o nome **AIZapZap**, cole este endereço e clique em **Adicionar**:

   ```
   https://tlcpebxdioeyzrjdtyes.supabase.co/functions/v1/mcp
   ```

3. No painel do AIZapZap, vá em **Integrações**, no cartão "Administre sua conta com o Claude", aba **Conector (claude.ai)**, e clique em **Enviar código para meu e-mail**. O código vale por 10 minutos e só pode ser usado uma vez.
4. Volte ao Claude e clique em **Conectar**. No navegador, entre na sua conta AIZapZap e, na tela que mostra **Claude (app/claude.ai)**, digite o código do e-mail e clique em **Permitir**. Só aprove se foi você que clicou em Conectar agora.
5. Numa conversa nova, ligue o AIZapZap no botão de ferramentas e peça: "Configure minha conta AIZapZap passo a passo".

Por que o código: sem ele, alguém poderia começar uma conexão na conta Claude dele e te mandar o link para você aprovar. Com o código, só funciona se foi você que pediu no seu painel. **Nunca passe esse código para ninguém.** Em contas Team ou Enterprise do Claude, quem adiciona o conector é o administrador da organização.

## A tela "Permitir acesso"

Ao fazer o login, aparece a tela "Permitir acesso à sua conta AIZapZap?". Ela mostra quem pede o acesso, a sua conta, os seus estabelecimentos e para onde o acesso volta: o seu próprio computador (`localhost`), no Claude Code, ou o Claude (`claude.ai`), no conector, que também pede o código enviado ao seu e-mail. Qualquer outro destino é recusado. Se essa tela aparecer sem você ter pedido, não clique em Permitir: um link mandado por outra pessoa entregaria o acesso à conta Claude dela.

O acesso fica salvo e é renovado sozinho.

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

1. No Claude Code (app, VS Code ou terminal): `/mcp`, escolha **aizapzap** e **Clear authentication**. No conector do claude.ai: **Configurações › Conectores**, abra o AIZapZap e remova.
2. Remova o plugin:

   ```
   /plugin uninstall aizapzap@aizapzap
   ```

## Suporte

Dúvidas ou problemas: use a tela de Suporte no painel, em https://aizapzap.com.br/dashboard/support.
