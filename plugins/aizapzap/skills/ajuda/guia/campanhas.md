# Campanhas
Link: https://aizapzap.com.br/dashboard/campaigns
Para quem: todos.

## Para que serve
Envia mensagens de campanha para clientes que aceitaram receber novidades. Você cria a mensagem, vê quem vai receber, agenda e acompanha o envio. O canal é o WhatsApp conectado, ou e-mail quando está disponível.

## Como usar
1. Conecte o WhatsApp antes. Sem conexão, a tela pede para ir à página WhatsApp.
2. Em "Nova campanha", dê um nome (só para você) e escreva a mensagem. Use {nome} para o primeiro nome do cliente.
3. Se quiser, adicione 1 link, uma imagem (endereço https ou uma arte de Minha marca) e até 2 botões de link.
4. No WhatsApp, você pode escolher um formulário em "Formulário (opcional)". Cada cliente recebe o próprio link: no fim da mensagem no QR Code, ou no botão "Responder formulário" na conexão oficial. Só aparecem formulários ativos que o cliente responde pelo link ("Link (página com as perguntas)"); com formulário, a mensagem não leva link próprio e cabe só 1 botão. Veja [Formulários](formularios.md).
5. Filtre o público: pediu nos últimos N dias, sem pedir há N dias, mínimo de pedidos, mínimo de pontos. Clique em "Ver público".
6. Escolha "Salvar rascunho" ou "Agendar envio" (vazio significa agora).
7. Acompanhe no "Histórico": enviadas, falharam, puladas, com Pausar, Retomar e Cancelar.

## Dúvidas comuns
- **Quem recebe?** Só quem aceitou novidades e já conversou com você. Quem responde SAIR para de receber na hora.
- **Qual o risco do QR Code?** A conexão por QR Code não é oficial e campanhas por ela podem bloquear seu número. Ela exige aceitar um termo de risco (só o administrador aceita) e tem limite diário baixo que cresce a cada dia.
- **E na API oficial?** A mensagem vira um modelo enviado para aprovação da Meta antes do envio, e a Meta cobra cada mensagem de marketing direto na sua conta do WhatsApp Business.
- **A campanha pausou sozinha.** Motivos mostrados na tela: WhatsApp desconectado, muitas falhas, limite do mês atingido ou termo não aceito.
- **Limite de mensagens?** Há uma cota mensal de mensagens de campanha por plano, com pacote avulso para comprar.
- **E-mail?** Leva link de descadastro, e quem sai para de receber em todos os canais.
- **Apareceu uma campanha que eu não criei, com nome e data.** É uma rotina do CRM que rodou. Cada vez que uma rotina roda, ela vira uma campanha aqui, com o nome da rotina e a data. Se ela pausar, retome ou cancele aqui. Para mudar a rotina, vá em CRM, aba "Rotinas" ([crm.md](crm.md)).

## Pelo Claude
listar_campanhas, criar_campanha (sempre como rascunho; aceita formulario, o id de um formulário ativo respondido pelo link, só no WhatsApp), agendar_campanha, pausar_campanha, retomar_campanha e cancelar_campanha. Termo de risco e compra de pacote: só pelo painel.

## English
Campaigns sends messages to customers who agreed to receive news. You write the message, preview the audience, schedule it and follow results. The unofficial QR Code connection needs a risk term and has a daily limit, while the official API requires Meta template approval. On WhatsApp you can attach an active link form ("Formulário (opcional)"): each customer gets their own link at the end of the text, or in a "Responder formulário" button on the official connection. Claude can create (as draft, with an optional formulario), schedule, pause, resume and cancel campaigns.
