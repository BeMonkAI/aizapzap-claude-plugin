# Cobranças
Link: https://aizapzap.com.br/dashboard/customers (abra a ficha do cliente, aba "Cobranças")
Para quem: todos. A baixa automática pelo comprovante é só nos planos Negócio e Rede.

## Para que serve
Cobrar um valor avulso de um cliente pelo WhatsApp, com Pix. Você cria a cobrança na ficha do cliente e o AIZapZap manda a mensagem com o valor, a descrição, o vencimento e a sua chave Pix. Depois você acompanha se foi paga.

Nos planos Negócio e Rede, o cliente manda a foto do comprovante na conversa e a cobrança recebe baixa sozinha. No plano Solo, você marca como paga.

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

## Pelo Claude
Só pelo painel. O Claude não cria, não envia, não dá baixa e não cancela cobranças, e também não muda os dados de recebimento (titular e chave Pix).

## English
Charges lets any business bill a customer a one-off amount over WhatsApp with Pix, from the "Cobranças" tab of the customer's file in the CRM. First fill in the payment receiver card in the Business Profile (account holder, CPF/CNPJ, Pix keys and card statement names); only the first Pix key goes in the message. "Nova cobrança" asks for amount (R$ 1 to R$ 100,000), due date and description (up to 140 characters; health businesses must not describe the procedure), and "Criar e enviar" sends it at once. Statuses: not sent, awaiting payment, overdue, paid (by hand or by receipt) and cancelled; open charges can be resent, marked as paid or cancelled (the customer is not told). A charge stays "not sent" when the customer has no WhatsApp number, receiver data is missing, WhatsApp is disconnected, the monthly message quota is used up, or, on the official WhatsApp, the customer has not written in 24 hours while Meta still reviews the message model (a new message from the customer opens the window). Limits: 30 charges per hour per business and 5 per customer in 24 hours. On the Negócio and Rede plans, a receipt image sent in the chat settles the charge after checking receiver, amount (not lower), date (not before the charge, not in the future) and reuse; "Paid by someone else" is accepted but flagged, and "Undo settlement" reopens it. On Solo the owner marks it paid. The AI knows the open charges, never confirms a payment itself and does not negotiate. Claude cannot create, send, settle or cancel charges, nor change the Pix data.
