# CRM
Link: https://aizapzap.com.br/dashboard/customers
Para quem: todos.

## Para que serve
Reúne os clientes do negócio. No menu, esta tela se chamava "Clientes" e agora se chama "CRM", no mesmo endereço. Tem quatro abas:
- **Lista:** os clientes com etapa, etiquetas, visitas, tempo sem visita, total gasto e se aceitam receber novidades. Dá para cadastrar, editar, importar uma planilha e exportar em CSV. Marcando as caixinhas ao lado dos nomes (até 200), aparece o botão "Enviar formulário": veja [Formulários](formularios.md).
- **Quadro:** uma coluna para cada etapa e um cartão para cada cliente, com nome, último contato, número de atendimentos e etiquetas. Serve para acompanhar em que pé está cada cliente.
- **Rotinas:** mensagens que saem sozinhas pelo WhatsApp, no dia e hora que você escolher, para os clientes que se encaixam no público. Por exemplo: toda segunda, para quem não volta há 30 dias.
- **Cobranças:** todas as cobranças do negócio, com o total em aberto e o vencido no topo, filtro por situação e busca pelo nome do cliente. Só para acompanhar: clique no nome para abrir a ficha do cliente na aba "Cobranças".

Ao clicar em um cliente, na lista ou no quadro, abre a ficha com histórico, cobranças e arquivos. Na aba "Cobranças" da ficha você cobra um valor avulso pelo WhatsApp, com Pix, e o cliente recebe lembretes automáticos: veja [Cobranças](cobrancas.md).

No quadro, o cartão do cliente mostra o selo "Cobrança em aberto" quando ele tem cobrança em aberto, ou "Cobrança vencida" quando uma delas já foi enviada e passou do vencimento.

Nem todo contato precisa ser cliente. No cadastro, o "Tipo de contato" pode ser "Cliente" (o padrão), "Fornecedor" ou "Outro" (um sócio, um parceiro). Fornecedor e Outro podem receber cobranças, inclusive de resposta, mas ficam fora das campanhas, das rotinas e do Quadro. Na Lista eles aparecem com um selo do tipo.

## Como usar
1. Use a busca para achar por nome, telefone, CPF ou e-mail.
2. Na aba "Lista", filtre por etapa, por etiqueta, por tempo sem atendimento (menos de 30 dias, 30 a 90, mais de 90, sem atendimentos), por consentimento de novidades ou por tipo de contato ("Tipo": Cliente, Fornecedor ou Outro). Ordene por nome, visitas, tempo sem visita, total gasto ou data de cadastro.
3. Clique em "Novo Cliente" e preencha nome (obrigatório) e telefone. Em "Tipo de contato", escolha "Cliente", "Fornecedor" ou "Outro". Campos extras variam por tipo de negócio: nascimento no salão / estúdio / box, endereço de entrega na marca local.
4. Para trazer vários de uma vez, clique em "Importar" e confirme a relação entre as colunas e os campos.
5. Na aba "Quadro", mude um cliente de etapa arrastando o cartão para outra coluna ou escolhendo a etapa no campo "Mover para", embaixo do cartão. No celular, use o campo.
6. Para mudar as etapas, clique em "Editar etapas" no quadro. Dá para renomear, adicionar ("Nova etapa"), subir ou descer. No fim, clique em "Salvar etapas".
7. Para remover uma etapa, use a lixeira ao lado dela e escolha para qual etapa vão os clientes que estão nela. Se você mudou algo na lista de etapas, salve antes de remover.
8. Clique no cliente para ver a ficha e enviar arquivos.
9. Para mandar um formulário a vários clientes, marque as caixinhas na aba "Lista" (a do topo marca a lista filtrada), até 200 por vez, e clique em "Enviar formulário". Para um cliente só, use a aba "Formulários" da ficha.

### Rotinas
Antes, conecte o WhatsApp. Sem conexão, o botão "Nova rotina" fica desligado.
1. Na aba "Rotinas", clique em "Nova rotina".
2. Se quiser, comece por um dos modelos prontos (veja abaixo). Ele preenche tudo e você ajusta.
3. Dê um nome (só para você) e escreva a mensagem. Use {nome} para o nome do cliente.
4. Escolha o público. Os campos podem ser combinados: "Etapa", "Etiqueta", "Chegou nos últimos (dias)", "Só aniversariantes do dia" e, conforme o tipo de negócio, "Sem pedido há (dias)" (restaurante e marca local) ou "Sem visita há (dias)" (salão / estúdio / box, profissional autônomo e creator).
5. Em "Quando", escolha "Todo dia", "Toda semana" (e o dia) ou "Todo mês" (dia 1 a 28). Escolha a "Hora". O horário é o do fuso do seu negócio.
6. Em "Intervalo mínimo para a mesma pessoa receber de novo (dias)", diga de quantos em quantos dias a mesma pessoa pode receber esta rotina (1 a 365, padrão 30).
7. Clique em "Salvar rotina". Ela nasce pausada: nada sai ainda.
8. Para começar, clique em "Ativar" na rotina. Para parar, clique em "Pausar". Para mudar algo, clique em "Editar" e salve de novo.
9. Clique em "Histórico" para ver cada vez que a rotina rodou: a data, a situação do envio e quantas mensagens foram enviadas, falharam ou foram puladas. A linha da rotina mostra o total enviado.

Modelos prontos:
- **"Comprou e não voltou há 30 dias"** (restaurante e marca local) ou **"Veio e não voltou há 30 dias"** (salão / estúdio / box, profissional autônomo e creator): toda segunda às 10h, para quem fez o último pedido ou o último atendimento há mais de 30 dias. Quem nunca pediu ou nunca veio fica de fora. A agência de marketing não tem este modelo.
- **"Boas-vindas (chegaram nos últimos 3 dias)"**: todo dia às 9h, para quem está na primeira etapa e foi cadastrado nos últimos 3 dias. A mesma pessoa só recebe uma vez por ano.
- **"Aniversariantes"**: todo dia às 9h, para quem faz aniversário no dia. Só chega a quem tem a data de nascimento cadastrada.

Cada vez que a rotina roda, ela vira um envio em Campanhas, com o nome da rotina e a data. Lá você acompanha, retoma ou cancela, como numa campanha comum.

## Dúvidas comuns
- **Quais são as etapas no começo?** Novo, Em conversa, Cliente, Em risco e Inativo. Você pode mudar todas.
- **Em que etapa entra um cliente novo?** Na primeira coluna do quadro. Quem chega pelo WhatsApp ou pela importação sem etapa aparece lá.
- **Por que alguns clientes já estão em "Cliente"?** Quem já tinha pedido ou atendimento quando o quadro chegou começou na etapa "Cliente".
- **Se eu mudar a ordem das etapas, os clientes mudam de coluna?** Não. Cada cliente fica na etapa em que estava.
- **O que são as etiquetas?** Palavras curtas para separar clientes, como "vip" ou "atacado". Aparecem na lista, no quadro e na ficha, e dá para filtrar por elas. Hoje quem grava etiquetas é o Claude, ao salvar clientes.
- **Apareceu "As etapas foram alteradas em outra aba". O que faço?** Outra pessoa ou outra aba salvou as etapas antes. A lista foi atualizada: confira e salve de novo.
- **Quero cobrar um fornecedor. Cadastro como cliente?** Cadastre no CRM e escolha "Fornecedor" em "Tipo de contato". Ele recebe cobranças em dinheiro ou de resposta (veja [Cobranças](cobrancas.md)), mas não entra em campanhas, rotinas nem no Quadro. Se ele paga por conta de empresa, use no nome a razão social que aparece no Pix: a baixa pelo comprovante confere o nome de quem pagou.
- **O fornecedor manda mensagem. A IA atende como cliente?** Sim, a IA conversa com ele normalmente. O tipo só tira o contato de campanhas, rotinas e Quadro.
- **Posso ter dois clientes com o mesmo telefone?** Não. O painel avisa que já existe um cliente com esse telefone (o mesmo vale para CPF).
- **O que significa "Aceita novidades"?** O cliente concordou em receber mensagens de campanha. Os estados são: aceita, recusou, pediu para sair e não perguntado.
- **Como a planilha é lida?** O importador reconhece nomes de coluna comuns, como nome, telefone, celular, e-mail e CPF, e deixa você ajustar ou ignorar colunas.
- **Como o total gasto é calculado?** A partir dos atendimentos do cliente e do preço de cada tipo de atendimento cadastrado.
- **A lixeira do cliente pede confirmação?** Não. A exclusão do cliente é imediata, então confira antes de clicar.
- **Por que alguns campos não aparecem?** O formulário mostra só o que faz sentido para o seu tipo de negócio.
- **Quem recebe a mensagem de uma rotina?** Só quem se encaixa no público e aceitou receber novidades. Quem respondeu SAIR não recebe. No WhatsApp não oficial (QR Code), também é preciso que o cliente já tenha conversado com você.
- **Por que um cliente não recebeu?** Os motivos mais comuns: não aceitou receber novidades; já recebeu outra mensagem de campanha nos últimos 7 dias (vale para rotinas e campanhas juntas); recebeu esta mesma rotina antes do intervalo mínimo; ou acabou o limite. O "Histórico" mostra quantos foram pulados.
- **As rotinas usam o limite do meu plano?** Sim. Cada envio de rotina conta na cota mensal de mensagens de campanha do plano, junto com as campanhas que você manda. No WhatsApp não oficial, também dividem o limite diário de envios.
- **A mensagem de aniversário chegou um dia depois. Por quê?** No WhatsApp não oficial, quando o limite diário acaba, o restante sai no dia seguinte.
- **O que quer dizer "Ativa" e "Pausada"?** Ativa: a rotina vai rodar no próximo dia e hora marcados. Pausada: não roda até você clicar em "Ativar". Toda rotina nova começa pausada.
- **O que quer dizer "Parada pelo envio"?** O último envio da rotina ficou parado em Campanhas, por exemplo por WhatsApp desconectado, muitas falhas, limite do mês atingido ou porque você pausou lá. Enquanto esse envio não termina, a rotina não começa outro. Clique em "Retomar ou cancelar em Campanhas" e resolva por lá.
- **O que quer dizer "Aguardando aprovação da Meta"?** No WhatsApp oficial, a mensagem vira um modelo de mensagem que a Meta precisa aprovar na primeira vez. Depois de aprovado, ele é usado de novo nas próximas vezes. Se você mudar o texto, precisa de nova aprovação. É só esperar.
- **O que quer dizer "Recusada pela Meta: mude o texto"?** A Meta não aprovou o modelo de mensagem. A rotina não tenta de novo com o mesmo texto: clique em "Editar", mude a mensagem e salve.
- **O que quer dizer "Modelo bloqueado pela Meta: altere o texto"?** A Meta tinha aprovado o modelo de mensagem, mas depois pausou ou desativou. Faça o mesmo: edite o texto e salve.
- **O que quer dizer "Etapa removida: edite a rotina"?** A etapa escolhida no público foi removida do quadro. Enquanto isso, a rotina não encontra ninguém. Edite e escolha outra etapa.
- **Apareceu "A conexão mudou". O que faço?** Você trocou a conexão do WhatsApp depois de criar a rotina. Clique em "Editar" e salve de novo para ela enviar pela conexão atual.
- **Não consigo ativar a rotina no WhatsApp não oficial.** A conexão por QR Code não é oficial e envios em massa por ela podem bloquear o seu número. Para ativar, aceite antes o termo de risco em Campanhas.
- **Posso apagar uma rotina?** Não. Pause ou edite. Assim o histórico de envios e o intervalo mínimo de cada cliente continuam valendo.
- **Ativei a rotina. Ela manda na hora?** Não. Ela roda no próximo dia e hora marcados, e o envio começa poucos minutos depois dessa hora.
- **Contas de demonstração podem criar rotinas?** Não. Na demonstração dá só para ver as rotinas e o histórico.

## Pelo Claude
- listar_clientes, para consultar. Cada cliente vem com a etapa e as etiquetas, e dá para trazer só os de uma etapa.
- listar_etapas, para ver as etapas na ordem e quantos clientes há em cada uma.
- salvar_clientes, para cadastrar ou atualizar até 200 clientes por vez (nome, telefone, e-mail, observações, etapa e etiquetas). O cliente é encontrado pelo telefone, com ou sem o 9º dígito. Sem etapa, quem já existe fica onde está. Etapa que não existe recusa só aquela linha, com o motivo. As etiquetas são somadas às que o cliente já tem (até 20, de até 40 letras cada), nunca trocadas. O consentimento de novidades nunca muda: quem pediu para sair continua fora.
- Criar, renomear e remover etapa, excluir cliente, enviar arquivo e mudar o "Tipo de contato": só pelo painel. Quem o Claude cadastra entra como "Cliente".
- enviar_formulario manda um formulário para até 200 clientes de uma vez (veja [Formulários](formularios.md)).
- Rotinas: só pelo painel. O Claude não cria, não edita, não ativa e não pausa rotinas.

Para trazer os clientes de outro sistema, peça ao Claude, por exemplo: "Importa meus clientes deste arquivo". Ele:
1. Lê o arquivo exportado do outro sistema.
2. Mostra as suas etapas e combina com você qual etapa daqui corresponde a cada situação de lá. Se faltar uma etapa, crie no painel: CRM, aba "Quadro", "Editar etapas".
3. Organiza nome, telefone, e-mail, observações, etapa e etiquetas.
4. Mostra um resumo (total, quantos por etapa, linhas sem telefone) e espera o seu ok.
5. Grava em partes de até 200 e, no fim, conta quantos foram criados, quantos atualizados e quais linhas foram recusadas, com o motivo.

## English
The "Customers" menu item is now "CRM", at the same address. The List tab shows everyone you serve with stage, tags, visits, days since last visit, total spent and marketing consent, with filters by stage and tag. The Board tab has one column per stage (default: New, In conversation, Customer, At risk, Inactive) and one card per customer; drag a card or use "Move to". "Edit stages" renames, adds, reorders and removes stages; removing one asks where its customers go. Customers with no stage show in the first column. Through Claude you can list stages and save up to 200 customers per call with stage and tags (tags are added, never replaced); stages are only created, renamed or removed in the panel. The Routines tab sends a WhatsApp message on its own (every day, week or month, at a chosen hour) to customers who fit the audience (stage, tag, arrived in the last N days, today's birthdays, no order or no visit for N days) and agreed to receive news. Ready-made models: away for 30 days, welcome (arrived in the last 3 days) and birthdays. A routine is created paused; "Activate" and "Pause" control it, and it cannot be deleted. Each run becomes a send in Campaigns, sharing the monthly campaign quota and the one-campaign-message-per-7-days cap; a customer does not get the same routine again before its minimum interval (default 30 days). On the official WhatsApp, Meta approves the text the first time and again whenever it changes; the unofficial connection needs the risk term in Campaigns. Routines are dashboard-only: Claude cannot create, edit or activate them. The Charges tab lists every one-off charge with open and overdue totals, status filters and search by customer name; clicking a name opens the customer file on its Charges tab. Board cards show "Cobrança em aberto" or "Cobrança vencida" (see cobrancas.md). Each contact has a "Tipo de contato": Cliente (default), Fornecedor (supplier) or Outro (other). Suppliers and other contacts can receive charges, including answer requests, but stay out of campaigns, routines and the Board; the List shows a type badge and a "Tipo" filter. The type is set only in the dashboard; contacts saved through Claude are customers. Tick up to 200 customers in the List to send them a form with "Enviar formulário" (see formularios.md).
