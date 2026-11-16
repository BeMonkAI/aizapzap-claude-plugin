# CRM
Link: https://aizapzap.com.br/dashboard/customers
Para quem: todos.

## Para que serve
Reúne os clientes do negócio. No menu, esta tela se chamava "Clientes" e agora se chama "CRM", no mesmo endereço. Tem duas abas:
- **Lista:** os clientes com etapa, etiquetas, visitas, tempo sem visita, total gasto e se aceitam receber novidades. Dá para cadastrar, editar, importar uma planilha e exportar em CSV.
- **Quadro:** uma coluna para cada etapa e um cartão para cada cliente, com nome, último contato, número de atendimentos e etiquetas. Serve para acompanhar em que pé está cada cliente.

Ao clicar em um cliente, na lista ou no quadro, abre a ficha com histórico e arquivos.

## Como usar
1. Use a busca para achar por nome, telefone, CPF ou e-mail.
2. Na aba "Lista", filtre por etapa, por etiqueta, por tempo sem atendimento (menos de 30 dias, 30 a 90, mais de 90, sem atendimentos) ou por consentimento de novidades. Ordene por nome, visitas, tempo sem visita, total gasto ou data de cadastro.
3. Clique em "Novo Cliente" e preencha nome (obrigatório) e telefone. Campos extras variam por tipo: nascimento no salão / estúdio / box, endereço de entrega na marca local.
4. Para trazer vários de uma vez, clique em "Importar" e confirme a relação entre as colunas e os campos.
5. Na aba "Quadro", mude um cliente de etapa arrastando o cartão para outra coluna ou escolhendo a etapa no campo "Mover para", embaixo do cartão. No celular, use o campo.
6. Para mudar as etapas, clique em "Editar etapas" no quadro. Dá para renomear, adicionar ("Nova etapa"), subir ou descer. No fim, clique em "Salvar etapas".
7. Para remover uma etapa, use a lixeira ao lado dela e escolha para qual etapa vão os clientes que estão nela. Se você mudou algo na lista de etapas, salve antes de remover.
8. Clique no cliente para ver a ficha e enviar arquivos.

## Dúvidas comuns
- **Quais são as etapas no começo?** Novo, Em conversa, Cliente, Em risco e Inativo. Você pode mudar todas.
- **Em que etapa entra um cliente novo?** Na primeira coluna do quadro. Quem chega pelo WhatsApp ou pela importação sem etapa aparece lá.
- **Por que alguns clientes já estão em "Cliente"?** Quem já tinha pedido ou atendimento quando o quadro chegou começou na etapa "Cliente".
- **Se eu mudar a ordem das etapas, os clientes mudam de coluna?** Não. Cada cliente fica na etapa em que estava.
- **O que são as etiquetas?** Palavras curtas para separar clientes, como "vip" ou "atacado". Aparecem na lista, no quadro e na ficha, e dá para filtrar por elas. Hoje quem grava etiquetas é o Claude, ao salvar clientes.
- **Apareceu "As etapas foram alteradas em outra aba". O que faço?** Outra pessoa ou outra aba salvou as etapas antes. A lista foi atualizada: confira e salve de novo.
- **Posso ter dois clientes com o mesmo telefone?** Não. O painel avisa que já existe um cliente com esse telefone (o mesmo vale para CPF).
- **O que significa "Aceita novidades"?** O cliente concordou em receber mensagens de campanha. Os estados são: aceita, recusou, pediu para sair e não perguntado.
- **Como a planilha é lida?** O importador reconhece nomes de coluna comuns, como nome, telefone, celular, e-mail e CPF, e deixa você ajustar ou ignorar colunas.
- **Como o total gasto é calculado?** A partir dos atendimentos do cliente e do preço de cada tipo de atendimento cadastrado.
- **A lixeira do cliente pede confirmação?** Não. A exclusão do cliente é imediata, então confira antes de clicar.
- **Por que alguns campos não aparecem?** O formulário mostra só o que faz sentido para o seu tipo de negócio.

## Pelo Claude
- listar_clientes, para consultar. Cada cliente vem com a etapa e as etiquetas, e dá para trazer só os de uma etapa.
- listar_etapas, para ver as etapas na ordem e quantos clientes há em cada uma.
- salvar_clientes, para cadastrar ou atualizar até 200 clientes por vez (nome, telefone, e-mail, observações, etapa e etiquetas). O cliente é encontrado pelo telefone, com ou sem o 9º dígito. Sem etapa, quem já existe fica onde está. Etapa que não existe recusa só aquela linha, com o motivo. As etiquetas são somadas às que o cliente já tem (até 20, de até 40 letras cada), nunca trocadas. O consentimento de novidades nunca muda: quem pediu para sair continua fora.
- Criar, renomear e remover etapa, excluir cliente e enviar arquivo: só pelo painel.

Para trazer os clientes de outro sistema, peça ao Claude, por exemplo: "Importa meus clientes deste arquivo". Ele:
1. Lê o arquivo exportado do outro sistema.
2. Mostra as suas etapas e combina com você qual etapa daqui corresponde a cada situação de lá. Se faltar uma etapa, crie no painel: CRM, aba "Quadro", "Editar etapas".
3. Organiza nome, telefone, e-mail, observações, etapa e etiquetas.
4. Mostra um resumo (total, quantos por etapa, linhas sem telefone) e espera o seu ok.
5. Grava em partes de até 200 e, no fim, conta quantos foram criados, quantos atualizados e quais linhas foram recusadas, com o motivo.

## English
The "Customers" menu item is now "CRM", at the same address. The List tab shows everyone you serve with stage, tags, visits, days since last visit, total spent and marketing consent, with filters by stage and tag. The Board tab has one column per stage (default: New, In conversation, Customer, At risk, Inactive) and one card per customer; drag a card or use "Move to". "Edit stages" renames, adds, reorders and removes stages; removing one asks where its customers go. Customers with no stage show in the first column. Through Claude you can list stages and save up to 200 customers per call with stage and tags (tags are added, never replaced); stages are only created, renamed or removed in the panel.
