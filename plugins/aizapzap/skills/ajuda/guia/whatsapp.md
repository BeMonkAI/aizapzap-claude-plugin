# WhatsApp
Link: https://aizapzap.com.br/dashboard/whatsapp
Para quem: todos.

## Para que serve
Conecta o número de WhatsApp do negócio, define quando a conversa passa para uma pessoa e ajusta o comportamento da IA no WhatsApp. A IA do Instagram usa essas mesmas configurações.

## Como usar
1. Em "Como conectar", escolha "QR Code (recomendado)" ou "API oficial do WhatsApp".
2. No QR Code: inicie a conexão, gere o QR Code e leia com o celular do WhatsApp. O painel verifica a conexão sozinho.
3. Na API oficial: preencha as credenciais da Meta e configure o webhook.
4. Em "Números de Contato", informe o número do negócio e o contato que recebe os avisos de escalonamento (com código do país, ex: +55 11 98888-8888).
5. Defina o "Horário de Atendimento Humano" e as regras de escalonamento.
6. Em "Avançado", ajuste brevidade, pausa após atendimento humano, tempo para encerrar por inatividade e números habilitados. Clique em "Salvar".

## Dúvidas comuns
- **Quando um atendimento é encerrado?** Depois de "Encerrar atendimento após inatividade" sem mensagens (padrão 120 minutos, de 15 minutos a 48 horas). Ele aparece como Finalizado em Conversas, e a próxima mensagem do cliente abre um atendimento novo.
- **Apareceu "Token expirado".** Na API oficial, o Meta recusou o token e a IA parou de responder. Os administradores recebem um e-mail. Gere um token novo (de preferência permanente) e cole em "Access Token".
- **O status ficou "Pendente".** No QR Code, gere um novo e leia de novo. Na API oficial, falta preencher credenciais ou verificar o webhook.
- **A IA só responde alguns números.** Se a lista de "Números Habilitados" tem algum número, a IA responde só quem está nela. Esvazie a lista para atender todos.
- **O que é a pausa após atendimento humano?** Depois que uma pessoa responde, a IA fica em silêncio pelo tempo definido (padrão 60 minutos, máximo 1440).
- **O que acontece fora do horário humano?** A IA avisa que não há atendente disponível e oferece alternativas.
- **Quem recebe o aviso quando a IA passa a conversa?** O contato de escalonamento, por mensagem de WhatsApp.
- **Posso desconectar?** Sim, no QR Code há "Desconectar WhatsApp", com confirmação.
- **Posso mandar muitas mensagens pelo QR Code?** Com cuidado. O QR Code (Evolution) usa o WhatsApp Web, não a conexão oficial, e o WhatsApp pode restringir ou desconectar, sem aviso, o número que parecer spam. A tela mostra o quadro "Como usar o Evolution sem arriscar o seu número": número novo precisa aquecer (nas primeiras semanas, algo como 10 a 20 mensagens por dia, aumentando aos poucos), prefira quem já conversou com você e, para prospectar ou disparar em volume, use a API oficial com modelo aprovado.
- **A conexão do QR Code caiu.** Antes de gerar um QR Code novo, veja no celular se há aviso de restrição do número. Se houver, pare os envios por alguns dias.

## Pelo Claude
atualizar_ai_settings ajusta o comportamento da IA, inclusive o tempo de inatividade para encerrar o atendimento. Conexão do WhatsApp, QR Code e credenciais: só pelo painel. No QR Code, enviar_mensagem avisa quando o Claude já mandou 20 ou mais mensagens nas últimas 24 horas: o Claude repassa o aviso e sugere parar por hoje ou usar uma campanha.

## English
The WhatsApp page connects the business number (QR Code or the official API), sets who gets escalations and when humans are available, and tunes how the AI behaves, including when an idle conversation closes (default 120 minutes). A "Token expirado" badge means Meta rejected the official API token and the AI is not replying. The connection itself can only be done in the dashboard. The QR Code connection (Evolution) runs on WhatsApp Web: WhatsApp may restrict or log out a number that looks like spam, so warm up a new number (around 10 to 20 messages a day at first), prefer people who already talked to you and use the official API for bulk sending. Through Claude, enviar_mensagem warns once it sent 20 or more messages in 24 hours on this connection.
