# Cobranças
Link: https://aizapzap.com.br/dashboard/customers (aba "Cobranças" do CRM, com todas as cobranças; ou abra a ficha do cliente, aba "Cobranças")
Para quem: todos. A baixa automática pelo comprovante é só nos planos Negócio e Rede.

## Para que serve
Cobrar um valor avulso de um cliente pelo WhatsApp, com Pix. Você cria a cobrança na ficha do cliente e o AIZapZap manda a mensagem com o valor, a descrição, o vencimento e a sua chave Pix. Depois você acompanha se foi paga.

Depois de enviada, a cobrança lembra o cliente sozinha: 1 dia antes do vencimento, no dia, 3 e 7 dias depois. Veja "Lembretes automáticos".

Nos planos Negócio e Rede, o cliente manda a foto do comprovante na conversa e a cobrança recebe baixa sozinha. No plano Solo, você marca como paga.

As cobranças ficam em dois lugares:
- **Ficha do cliente, aba "Cobranças":** onde você cria, reenvia, dá baixa, cancela e para os lembretes.
- **CRM, aba "Cobranças":** todas as cobranças do negócio numa lista só, com o total em aberto e o total vencido. Serve para acompanhar. Veja "Aba Cobranças do CRM".

## Como usar

### Antes: dados de recebimento
1. Abra o Perfil do Estabelecimento (https://aizapzap.com.br/dashboard/profile) e desça até o cartão "Dados de recebimento".
2. Preencha "Titular" (o nome que aparece para quem paga o Pix), "CPF/CNPJ" e "Chaves Pix (uma por linha)". Se aceita cartão, preencha também "Nomes na fatura do cartão (um por linha)", o nome que a maquininha mostra na fatura.
3. Clique em "Salvar" do próprio cartão. Ele salva separado do resto do perfil.

Só a primeira chave Pix vai na mensagem ao cliente. As outras servem para conferir comprovantes.

### Criar e enviar
1. No CRM, clique no cliente para abrir a ficha e vá na aba "Cobranças".
2. Clique em "Nova cobrança".
3. Preencha "Valor (R$)" (de R$ 1,00 a R$ 100.000,00), "Vencimento" (vem com uma semana à frente) e "Descrição" (até 140 caracteres, por exemplo "Sessão de outubro"). Em atendimento de saúde, não descreva o procedimento: a descrição vai na mensagem.
4. Clique em "Criar e enviar". A mensagem sai na hora pelo WhatsApp.

O cliente recebe este texto:

> Olá, [nome do cliente]. [nome do seu negócio] registrou uma cobrança de [valor] referente a "[descrição]", com vencimento em [dia/mês]. Pague por Pix para [titular] (chave [sua primeira chave Pix]). Depois de pagar, envie o comprovante por aqui.

O que está entre colchetes é trocado pelos dados reais.

No plano Solo, a última frase é "Depois de pagar, avise por aqui."

### Acompanhar
Cada cobrança aparece na lista com valor, descrição, vencimento e a situação. Embaixo de uma cobrança em aberto ficam os botões:
- **"Reenviar":** manda a mesma mensagem de novo.
- **"Marcar como pago":** dá baixa à mão, por exemplo quando o cliente pagou em dinheiro. Pede confirmação.
- **"Cancelar":** encerra a cobrança. O cliente não é avisado.
- **"Parar lembretes":** interrompe os lembretes automáticos dessa cobrança. Aparece só enquanto há um próximo lembrete marcado.

Paga e cancelada são finais: não voltam a ficar em aberto (exceto "Desfazer baixa", veja abaixo).

### O que quer dizer cada situação
- **Não enviada:** a cobrança foi criada, mas a mensagem nunca chegou a sair. Embaixo aparece o motivo em vermelho.
- **Aguardando pagamento:** a mensagem foi enviada e o vencimento ainda não passou.
- **Vencida:** a mensagem foi enviada e o vencimento já passou.
- **Paga:** mostra a data e como foi a baixa, "baixa manual" ou "comprovante".
- **Cancelada:** você cancelou.

### Comprovante pelo WhatsApp (planos Negócio e Rede)
1. O cliente paga e manda a foto ou o print do comprovante na conversa.
2. O AIZapZap confere o comprovante. Se estiver certo, a cobrança vira "Paga", com "pago em dd/mm (comprovante)", e a IA confirma para o cliente. Se não, a IA explica o que está errado e a cobrança segue em aberto.
3. Na cobrança paga, "Ver comprovante" abre a imagem.
4. Se descobrir que o dinheiro não entrou, use "Desfazer baixa". A cobrança volta a ficar em aberto e aquele comprovante não vale mais para ela.

O que é conferido:
- Se é mesmo o comprovante. A tela de detalhe do Pix não serve: precisa ser o comprovante completo, gerado no app do banco.
- Se o pagamento foi para você: o recebedor tem o nome do "Titular". Se o comprovante mostra parte do CPF/CNPJ ou a chave Pix, eles precisam bater com os seus. No cartão, o nome tem que estar em "Nomes na fatura do cartão".
- Se o valor não é menor que o da cobrança. Pagar a mais dá baixa.
- Se a data não é anterior à criação da cobrança nem futura (Pix agendado não vale).
- Se o comprovante não foi usado antes, em outra cobrança ou em vaga de aula.

### Lembretes automáticos
Toda cobrança enviada lembra o cliente pelo WhatsApp, sem você fazer nada. Você não precisa ligar.

Quando saem:
- 1 dia antes do vencimento, no dia do vencimento, 3 dias depois e 7 dias depois. No máximo 4 lembretes por cobrança.
- Só entre 9h e 18h, no fuso do seu negócio. Normalmente saem a partir das 9h do dia marcado.
- Só para cobranças que foram enviadas. Cobrança "Não enviada" não tem lembrete.
- O primeiro lembrete sai pelo menos 12 horas depois do envio da cobrança. Se um dia marcado cai antes disso, ele é pulado. Exemplo: cobrança criada hoje com vencimento amanhã não recebe o lembrete de "vence amanhã".
- Um lembrete que passou da hora não é mandado atrasado junto com outros: o cliente recebe um só e o próximo fica para o próximo dia marcado.

O cliente recebe este texto (o que está entre colchetes é trocado pelos dados reais):

> Olá, [nome do cliente]. Lembrete de [nome do seu negócio]: a cobrança de [valor] referente a "[descrição]" vence amanhã, [dia/mês]. Pague por Pix para [titular] (chave [sua primeira chave Pix]). Depois de pagar, envie o comprovante por aqui.

A parte do meio muda conforme o dia:
- Antes do vencimento: "vence amanhã, [dia/mês]."
- No dia: "vence hoje, [dia/mês]."
- Depois: "venceu em [dia/mês] e ainda está em aberto."

A última frase segue o plano, como na cobrança: no Solo, "Depois de pagar, avise por aqui."; no Negócio e na Rede, "Depois de pagar, envie o comprovante por aqui."

No WhatsApp oficial, quando o cliente não fala com você há mais de 24 horas, vai um modelo de mensagem com um texto só para os três casos:

> Olá, [nome do cliente]. Lembrete de [nome do seu negócio]: a cobrança de [valor] referente a "[descrição]", com vencimento em [dia/mês], ainda está em aberto. Pague por Pix para [titular] (chave [sua primeira chave Pix]). Depois de pagar, envie o comprovante por aqui.

Quem nunca recebe lembrete:
- O cliente que respondeu SAIR. Os lembretes das cobranças dele param sozinhos. A cobrança em si continua em aberto.
- Cobrança paga, cancelada ou com os lembretes parados.

Limites:
- No máximo um lembrete por cliente por dia. Se o cliente tem duas cobranças com lembrete no mesmo dia, uma sai hoje e a outra no dia seguinte.
- O AIZapZap manda os lembretes em rodadas, a cada poucos minutos, com até 20 por negócio em cada rodada. O que passar disso sai nas rodadas seguintes, sempre dentro do horário das 9h às 18h.
- No WhatsApp não oficial (QR Code), os lembretes contam no limite diário de envios, junto com as campanhas e as rotinas. Acabou o limite do dia, o restante espera o dia seguinte.
- Cada lembrete enviado conta como uma mensagem do plano. Se acabaram as mensagens do mês, o lembrete não sai.

No WhatsApp oficial, fora das 24 horas, o lembrete precisa de um modelo de mensagem aprovado pela Meta. Ele é mandado para aprovação sozinho na primeira vez que uma cobrança sua sai pelo WhatsApp oficial, e costuma estar aprovado antes do primeiro lembrete. Enquanto não está aprovado, aquele lembrete é pulado. Ele nunca é trocado pela mensagem da cobrança, para o cliente não achar que é uma segunda cobrança.

Como acompanhar na ficha do cliente, aba "Cobranças", embaixo de cada cobrança em aberto já enviada:
- **"Lembretes: 1 de 4, próximo em 20/11":** quantos já saíram e o dia do próximo.
- **"Lembretes: 4 de 4, nenhum outro agendado":** não há mais lembretes para essa cobrança.
- **"O último não saiu: ..."**, no fim da linha: o motivo de o último lembrete ter sido pulado, por exemplo WhatsApp desconectado ou mensagens do plano esgotadas. Lembrete pulado não entra na conta do "X de 4".
- **"Lembretes parados: ..."**: os lembretes pararam, com o motivo e quantos saíram. Os motivos são "você parou os lembretes", "o cliente pediu para parar" (respondeu SAIR depois de receber a cobrança) e "o cliente pediu SAIR" (já tinha pedido para sair antes, ou saiu pelo link do e-mail).

Para parar os lembretes de uma cobrança:
1. Abra a ficha do cliente, aba "Cobranças".
2. Na cobrança, clique em "Parar lembretes" e confirme. A cobrança continua em aberto.
3. A linha passa a mostrar "Lembretes parados: você parou os lembretes".

Não dá para religar os lembretes de uma cobrança. Se quiser que voltem, cancele a cobrança e crie outra.

### Aba Cobranças do CRM
1. No CRM, clique na aba "Cobranças" (a quarta, depois de Lista, Quadro e Rotinas).
2. No topo ficam dois totais:
   - **"Em aberto":** a soma e a quantidade de todas as cobranças em aberto, enviadas ou não, vencidas ou não.
   - **"Vencido":** a soma e a quantidade das cobranças em aberto, já enviadas, com o vencimento antes de hoje.
3. Escolha a situação nos botões "Em aberto" (começa nela), "Vencidas", "Não enviadas", "Pagas", "Canceladas" ou "Todas".
4. Para achar um cliente, digite parte do nome em "Buscar cliente". A busca é só pelo nome.
5. Cada linha mostra o cliente, o valor, a descrição, a data (vence, venceu ou pago em) e a situação. As mais recentes vêm primeiro, 50 por vez. Clique em "Ver mais" para trazer as próximas.
6. Clique no nome do cliente para abrir a ficha dele já na aba "Cobranças". Lá você reenvia, dá baixa, cancela ou para os lembretes. A aba do CRM só mostra.

No Quadro do CRM, o cartão do cliente mostra um selo:
- **"Cobrança em aberto":** o cliente tem ao menos uma cobrança em aberto (inclusive uma ainda não enviada).
- **"Cobrança vencida":** pelo menos uma delas já foi enviada e passou do vencimento.

## Dúvidas comuns
- **Por que o botão "Nova cobrança" está desligado?** O cliente não tem número de WhatsApp no cadastro. A ficha avisa: "Este cliente não tem um número de WhatsApp no cadastro, então não dá para enviar cobrança." Cliente que só fala pelo Instagram também cai aqui. Cadastre o WhatsApp dele.
- **Cliquei em "Nova cobrança" e apareceu um aviso para preencher os dados de recebimento.** Falta o titular ou a chave Pix. Use o link "Abrir o Perfil do Estabelecimento", preencha e salve.
- **Por que a cobrança ficou "Não enviada"?** O motivo aparece embaixo dela. Resolva e clique em "Reenviar". Os motivos mais comuns:
  - o cliente não tem número de WhatsApp;
  - faltam os dados de recebimento (titular e chave Pix);
  - o WhatsApp do negócio não está conectado;
  - acabaram as mensagens do plano no mês (cada cobrança enviada conta como uma mensagem);
  - no WhatsApp oficial, o cliente não fala com você há mais de 24 horas e o modelo de mensagem de cobrança ainda está em aprovação na Meta.
- **O que é essa regra das 24 horas?** No WhatsApp oficial, a mensagem livre só pode ir para quem falou com você nas últimas 24 horas. Fora disso, vai um modelo de mensagem que a Meta aprova uma vez. Enquanto não aprova, a cobrança não sai. Dica: se o cliente mandar qualquer mensagem, a janela de 24 horas abre e a cobrança pode ser reenviada na hora. No WhatsApp não oficial (QR Code) essa regra não existe.
- **Apareceu "O WhatsApp recusou a mensagem de cobrança".** A Meta não aprovou o modelo de mensagem. A cobrança só vai quando o cliente falar com você nas últimas 24 horas.
- **Apareceu "O WhatsApp pausou ou desativou a mensagem de cobrança".** Fale com o suporte do AIZapZap.
- **Apareceu "A mensagem pode ter sido enviada".** O WhatsApp demorou a responder e não dá para saber se a mensagem saiu. A cobrança conta como enviada. Confira a conversa com o cliente antes de reenviar. Ao clicar em "Reenviar", o painel pergunta de novo. Por uns 10 minutos, o reenvio fica bloqueado.
- **Apareceu "Esta cobrança já está sendo enviada. Aguarde um minuto."** A mesma cobrança acabou de ser enviada. Isso evita mandar duas vezes.
- **Existe limite de envios?** Sim: até 30 cobranças por hora no negócio e 5 por cliente em 24 horas. Passou disso, o painel avisa e é só tentar mais tarde.
- **No plano Negócio a mensagem saiu com "avise por aqui" em vez de "envie o comprovante".** No WhatsApp oficial, fora das 24 horas, enquanto a Meta aprova a versão com comprovante vai a versão "avise por aqui". O comprovante que o cliente mandar é conferido do mesmo jeito.
- **O cliente mandou o comprovante e nada aconteceu.** Confira: o plano é Negócio ou Rede? A cobrança chegou a ser enviada (não está "Não enviada")? A conferência vale até 5 comprovantes por cliente por hora. Foto que não é comprovante é tratada como uma foto comum.
- **O que aparece quando o comprovante é recusado?** Na cobrança aparece "Comprovante recusado em dd/mm" e o motivo, por exemplo "o valor pago é menor que o da cobrança" ou "o recebedor do comprovante não confere com os seus dados de recebimento". O cliente recebe a explicação na conversa e pode mandar outro.
- **O cliente tem duas cobranças. Qual recebe a baixa?** A de valor igual ao do comprovante (a de vencimento mais antigo, se houver mais de uma). Se nenhuma tem o mesmo valor, a mais antiga que o valor pago cobre.
- **O que é "Pago por outra pessoa: confira o comprovante"?** O nome de quem pagou não bate com o do cliente, por exemplo um parente pagou. A baixa é feita assim mesmo, mas vale você conferir.
- **E "Confira o comprovante: pagamento com cartão sem código de autorização"?** O comprovante do cartão não mostra o código de autorização. A baixa é feita, mas confira.
- **Recebo algum aviso?** Sim, pelo WhatsApp, nos telefones de "Notificações" do Perfil e no contato de escalonamento do WhatsApp, quando o comprovante é válido mas menor que todas as cobranças do cliente, ou quando os seus dados de recebimento estão incompletos. No máximo um aviso por cliente por hora.
- **Dá para desfazer uma baixa manual?** Não. "Desfazer baixa" aparece só nas cobranças pagas por comprovante.
- **Posso mudar o valor ou o vencimento?** Não. Cancele e crie outra.
- **O que a IA fala sobre as cobranças?** A IA sabe as cobranças em aberto do cliente (até 3, vencimento mais antigo primeiro) e responde quanto ele deve, a que se refere, o vencimento e o Pix. Ela nunca confirma um pagamento por conta própria: no Solo, diz que o negócio vai conferir; no Negócio e na Rede, pede o comprovante por ali. Ela não negocia valor nem prazo e encaminha esse pedido para você.
- **Contas de demonstração podem cobrar?** Não. Na demonstração dá só para ver.
- **Os dados de recebimento das aulas pagas mudaram de lugar?** Sim. Agora ficam no Perfil do Estabelecimento, valem para cobranças e aulas, e aparecem para todos os tipos de negócio.
- **Por que um lembrete não saiu?** Veja a linha "Lembretes" embaixo da cobrança, na ficha do cliente. Se aparece "O último não saiu", o motivo vem logo depois. Os mais comuns: WhatsApp do negócio desconectado; faltam os dados de recebimento; acabaram as mensagens do plano no mês; o cliente não tem número de WhatsApp; no WhatsApp oficial, o cliente não fala com você há mais de 24 horas e o modelo de mensagem do lembrete ainda está em aprovação ou foi recusado pela Meta. O lembrete pulado não volta: o próximo sai no próximo dia marcado. Se não aparece motivo, confira se a cobrança foi enviada, se não está paga ou cancelada, se os lembretes não foram parados e se o cliente não respondeu SAIR. Lembrete que cairia fora das 9h às 18h espera o horário.
- **O cliente tem duas cobranças e recebeu só um lembrete no dia. Por quê?** Para não encher o cliente de mensagens, sai no máximo um lembrete por cliente por dia. O outro sai no dia seguinte, com o texto certo para aquela data.
- **Como paro os lembretes de um cliente?** Os lembretes são por cobrança. Abra a ficha do cliente, aba "Cobranças", e clique em "Parar lembretes" em cada cobrança em aberto dele.
- **Cancelar a cobrança para os lembretes?** Sim. Cobrança cancelada não recebe mais lembretes.
- **Marcar como pago para os lembretes?** Sim. Cobrança paga, à mão ou por comprovante, não recebe mais lembretes. Se você usar "Desfazer baixa" de um comprovante, os lembretes voltam, a partir de 12 horas depois, a não ser que você tenha parado antes.
- **E se o cliente pagar bem na hora em que o lembrete vai sair?** Logo antes de enviar, o AIZapZap confere de novo se a cobrança continua em aberto e com os lembretes ligados. Só se a baixa cair no mesmo instante do envio o lembrete ainda pode sair.
- **"Reenviar" recomeça os lembretes?** Não. Os lembretes começam uma vez, quando a cobrança é enviada pela primeira vez, e seguem as datas do vencimento. Uma cobrança que ficou "Não enviada" e depois foi reenviada com sucesso passa a ter lembretes a partir daí.
- **Apareceram lembretes em cobranças antigas, criadas antes desta novidade. É normal?** Sim. Os lembretes chegaram em 18/11/2026 e passaram a valer também para as cobranças que já estavam em aberto e tinham sido enviadas. Ninguém recebeu lembretes atrasados de uma vez. A regra foi esta:
  - ainda não tinha vencido: recebe os lembretes que faltam;
  - vencida há até 2 dias: recebe os de 3 e de 7 dias depois do vencimento;
  - vencida há 3 a 7 dias: recebe só o de 7 dias;
  - vencida há mais de 7 dias: não recebe nenhum.

  Se não quiser lembrete numa delas, use "Parar lembretes".
- **O cliente que respondeu SAIR ainda recebe a cobrança?** A cobrança, sim, se você enviar: o envio da cobrança não olha o pedido de SAIR. Os lembretes, não.

## Pelo Claude
O Claude pode consultar as cobranças com a ferramenta listar_cobrancas. Peça, por exemplo: "Quais cobranças estão vencidas?", "Quanto tenho em aberto?" ou "Mostra as cobranças da Maria".
- Filtra por situação: em aberto (o padrão, inclui as não enviadas), vencida, paga, cancelada ou todas.
- Busca pela parte do nome do cliente.
- Traz até 50 por vez, das mais recentes para as mais antigas, e o total em aberto e o total vencido.
- Cada cobrança vem com cliente, valor, descrição, vencimento, situação (inclusive "não enviada"), data de envio, data e forma de pagamento (manual ou comprovante) e quantos lembretes já saíram.
- Nunca mostra a imagem do comprovante.

O resto é só pelo painel. O Claude não cria, não envia, não dá baixa, não cancela cobranças e não para lembretes, e também não muda os dados de recebimento (titular e chave Pix).

## English
Charges lets any business bill a customer a one-off amount over WhatsApp with Pix, from the "Cobranças" tab of the customer's file in the CRM. First fill in the payment receiver card in the Business Profile (account holder, CPF/CNPJ, Pix keys and card statement names); only the first Pix key goes in the message. "Nova cobrança" asks for amount (R$ 1 to R$ 100,000), due date and description (up to 140 characters; health businesses must not describe the procedure), and "Criar e enviar" sends it at once. Statuses: not sent, awaiting payment, overdue, paid (by hand or by receipt) and cancelled; open charges can be resent, marked as paid or cancelled (the customer is not told). A charge stays "not sent" when the customer has no WhatsApp number, receiver data is missing, WhatsApp is disconnected, the monthly message quota is used up, or, on the official WhatsApp, the customer has not written in 24 hours while Meta still reviews the message model (a new message from the customer opens the window). Limits: 30 charges per hour per business and 5 per customer in 24 hours. On the Negócio and Rede plans, a receipt image sent in the chat settles the charge after checking receiver, amount (not lower), date (not before the charge, not in the future) and reuse; "Paid by someone else" is accepted but flagged, and "Undo settlement" reopens it. On Solo the owner marks it paid. The AI knows the open charges, never confirms a payment itself and does not negotiate. Every sent charge reminds the customer automatically 1 day before the due date, on the due date, and 3 and 7 days after (at most 4, only between 9am and 6pm in the business time zone, the first at least 12 hours after the charge was sent; a missed slot is not sent late in bulk). The text says "is due tomorrow", "is due today" or "was due on ... and is still open", with the plan's last sentence; outside the official WhatsApp 24-hour window a Meta-approved reminder message model is used (submitted automatically on the first charge sent through the official WhatsApp; until approved that reminder is skipped, never replaced by the charge text). No reminders for customers who replied SAIR, nor for paid, cancelled or stopped charges; at most one reminder per customer per day, up to 20 per business per round; each reminder counts as one plan message and, on the unofficial WhatsApp, in the daily sending limit shared with campaigns. The customer file shows "Lembretes: X de 4, próximo em dd/mm" and the reason a reminder was skipped; "Parar lembretes" stops them for good (to restart, cancel and create a new charge). Charges open and sent on release day (18/11/2026) got the remaining slots: not yet due = all remaining, 0 to 2 days overdue = +3 and +7, 3 to 7 days = +7 only, more than 7 days = none. The CRM "Cobranças" tab lists every charge, newest first, 50 at a time with "Ver mais", with "Em aberto" (all open charges, sent or not) and "Vencido" (open, sent and past due) totals, status filters and search by customer name; clicking the name opens the customer file on its Charges tab. Board cards show "Cobrança em aberto" or "Cobrança vencida". Claude can list charges (listar_cobrancas: status filter, name search, up to 50 per page, totals, reminders sent; never receipt images) but cannot create, send, settle, cancel charges, stop reminders, nor change the Pix data.
