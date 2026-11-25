# Formulários
Link: https://aizapzap.com.br/dashboard/formularios
Para quem: todos.

## Para que serve
Formulários que o cliente responde pelo WhatsApp, uma pergunta por vez: pesquisa de satisfação, ficha de cadastro, inscrição, questionário. Você cria quantos quiser, envia na hora para um cliente ou para vários, ou deixa sair sozinho depois de um atendimento, de um pedido ou da primeira reserva. As respostas aparecem no painel, com indicadores e exportação em CSV.

Para começar mais rápido, use o seletor "Começar de um modelo":
- **Pesquisa de satisfação:** nota de 0 a 10 e um comentário opcional, com alerta quando a nota é menor que 6.
- **Ficha de matrícula:** nome, nascimento, e-mail, plano ou turma, horário preferido e como conheceu.
- **Inscrição em evento:** nome, se confirma presença, quantos acompanhantes e uma observação.
- **Anamnese** (só no perfil profissional): motivo da consulta, remédios, alergias e problemas de saúde.

## Como usar
1. Clique em "Novo formulário" ou escolha um modelo em "Começar de um modelo".
2. Dê um nome (1 a 80 letras). Se quiser, escreva uma "Descrição (só para você)" (até 300), a "Mensagem de abertura" e a "Mensagem de agradecimento" (até 500 cada).
3. Adicione de 1 a 30 perguntas. Tipos: texto, número, escala (de/até, padrão 0 a 10), sim ou não, escolha única e várias escolhas (2 a 10 opções) e data (dd/mm/aaaa). Pergunta que não é obrigatória pode ser pulada: o cliente responde PULAR. No salão / estúdio / box e no profissional autônomo, com "Atividades dos atletas" ligado em Integrações, também há a pergunta de treinos.
4. Em "Quando enviar", escolha o gatilho e, se quiser, um "Atraso (minutos)" (0 a 10080, ou seja, até 7 dias):
   - **Manual:** você envia pela ficha do cliente ou pela lista do CRM (veja abaixo).
   - **Depois do atendimento:** conta a partir do horário marcado mais a duração do serviço (30 minutos se não houver serviço), mais o atraso.
   - **Depois do pedido:** conta a partir do pedido entregue.
   - **Primeira reserva confirmada:** vai uma vez para cada cliente, quando a primeira reserva dele é confirmada e o horário ainda não chegou. Reserva cancelada ou recusada antes não conta, e quem já recebeu este formulário não recebe de novo. Bom para mandar a ficha antes da primeira visita.
5. Em "Prazo para responder (dias)", diga quanto tempo o cliente tem (1 a 30, padrão 7).
6. Em "Como o cliente responde", escolha "WhatsApp (uma pergunta por vez)" (padrão), "Link (página com as perguntas)" ou "WhatsApp e link". O link abre sem login, vale até o fim do prazo e aceita uma resposta só.
7. Em "Lembretes para quem não respondeu", escolha de 0 a 3 (padrão 0). Sai no máximo 1 por dia, 24 horas depois da última mensagem sem resposta, das 9h às 20h.
8. Em "Avisar o dono quando a resposta for", crie alertas para perguntas de número, escala, escolha única ou sim ou não: escolha a comparação (menor, igual, maior) e o valor. Numa pergunta de escala, o valor do alerta precisa estar dentro da escala (por exemplo, de 0 a 10). Quando o cliente termina, você recebe o aviso pelo WhatsApp.
9. Clique em "Salvar". O status pode ser ativo, pausado ou arquivado.

### Enviar para um cliente ou para vários
- **Um cliente:** abra a ficha dele no CRM, aba "Formulários", e clique em "Enviar formulário".
- **Vários clientes:** no CRM, aba "Lista", marque as caixinhas ao lado dos nomes (ou a caixinha do topo, que marca a lista filtrada) até 200 por vez. Aparece o botão "Enviar formulário": escolha o formulário e clique em "Enviar". O resumo mostra quantos foram para a fila e quantos foram pulados, com o motivo.

Também dá para mandar um formulário dentro de uma campanha ou de uma rotina do CRM, em "Formulário (opcional)": cada cliente recebe o próprio link. Ali só aparecem formulários ativos respondidos pelo link. Veja [Campanhas](campanhas.md) e [CRM](crm.md).

Só formulário ativo pode ser enviado. Ficam de fora quem pediu SAIR, quem não tem telefone e quem já tem este formulário em aberto.

### Respostas
Clique em "Respostas" no formulário. Você vê enviados, respondidos, taxa de resposta, a média das perguntas de número e a contagem das escolhas, e uma tabela com cada envio e a situação dele: na fila, enviado, respondendo, respondido, respondido pelo link, expirado, cancelado, pediu SAIR, fora da janela de 24h ou "Aviso enviado, aguardando resposta". Num envio aberto, "Cancelar" encerra sem avisar o cliente. "Exportar CSV" baixa tudo. Envio com respostas apagadas ou expurgadas mostra "Removido" no nome e no telefone, no painel e no CSV.

### Dado sensível (saúde)
Marque "Contém dado sensível (saúde)" no editor para fichas como anamnese. No perfil profissional, todo formulário novo já nasce marcado. Com a caixa marcada:
- O formulário sai só pelo WhatsApp, e o cliente autoriza antes da primeira pergunta (responde SIM ou NÃO; NÃO encerra sem guardar nada). A qualquer momento ele pode responder APAGAR para apagar as respostas.
- Só o dono ou um administrador vê as respostas, pelo botão "Mostrar respostas (acesso registrado)". Os outros membros veem só a situação, sem CSV. A IA e o Claude só sabem que foi respondido, e o alerta ao dono não traz a resposta.
- As respostas são apagadas sozinhas depois do prazo "Guardar as respostas por (dias)" (1 a 3650, padrão 365).
- Se o cliente pedir a exclusão, use "Apagar respostas" no envio (dono ou administrador). O envio passa a mostrar "Respostas apagadas".

### Acessos às respostas
Dono e administradores têm o botão "Acessos às respostas" no topo da lista de formulários. Ele mostra quem abriu ou apagou respostas sensíveis: quando, quem (o e-mail de quem ainda está na equipe; quem saiu aparece por um código), o que fez (abriu, apagou ou apagamento automático no fim do prazo), qual formulário, quantas respostas e por onde (painel, Claude, sistema ou pedido do cliente pelo WhatsApp). Use para mostrar que você cuida dos dados de saúde dos seus clientes.

## Dúvidas comuns
- **Posso mudar as perguntas depois de enviar?** Não. Depois do primeiro envio as perguntas ficam fixas, para as respostas continuarem comparáveis. Nome, mensagens, gatilho, prazo, alertas e status continuam editáveis. Para outras perguntas, crie um formulário novo.
- **Que horas o formulário chega?** A primeira pergunta sai entre 9h e 20h, no fuso do seu negócio, e cada pessoa recebe no máximo 1 formulário por dia. O cliente responde um formulário por vez; os outros esperam na fila. Envio que fica na fila mais que o prazo para responder expira sem sair.
- **O gatilho automático pega atendimentos antigos?** Só das últimas 48 horas, e só os que não foram cancelados, recusados nem marcados como falta. O mesmo atendimento ou pedido nunca gera dois envios.
- **O que é "Fora da janela de 24h"?** No WhatsApp oficial, quem não falou com o seu número nas últimas 24 horas recebe antes um aviso pelo modelo aprovado pela Meta, e o formulário começa quando a pessoa responde. Se a Meta recusou o modelo de aviso, o envio fica "Fora da janela de 24h". Se ainda está em análise, o sistema tenta de novo mais tarde.
- **Formulário usa o limite do meu plano?** Sim. Cada mensagem do formulário conta na franquia de mensagens do plano, inclusive o aviso e os lembretes.
- **O que acontece se eu pausar ou arquivar?** Os envios em aberto são cancelados e o formulário some da lista de envio.
- **Por que o alerta não salva?** Numa pergunta de escala, o valor do alerta precisa estar dentro da escala. Se a escala vai de 0 a 10, um alerta "menor que 11" é recusado com o aviso "O alerta precisa ficar na escala".
- **Posso mandar para mais de 200 clientes de uma vez?** Não. Marque até 200, envie e depois marque o próximo grupo.
- **Por que não vejo o botão "Acessos às respostas"?** Ele aparece só para o dono e os administradores.
- **Quem pode desmarcar o dado sensível ou mudar o prazo de guarda?** Só o dono ou um administrador. Desmarcar só dá antes do primeiro envio.

## Pelo Claude
- listar_formularios, para ver os formulários com status, gatilho, canal, lembretes, prazo, perguntas numeradas, alertas e quantos foram enviados, respondidos e estão na fila.
- listar_respostas_formulario, para ver até 50 envios de um formulário (formulario) ou de um cliente (cliente_id ou telefone), mais recentes primeiro, com situação e respostas. Com formulario, traz também os indicadores do painel. Em formulário sensível mostra só se foi respondido, nunca as respostas. Envio apagado ou expurgado aparece com nome e telefone "Removido".
- listar_acessos_respostas, para ver o registro de quem abriu ou apagou respostas sensíveis (até 200 por vez; para os mais antigos, o Claude continua de onde parou). Só para administradores, e nunca mostra as respostas.
- salvar_formulario, para criar ou editar um formulário como no editor do painel: nome, descrição, mensagens, status, gatilho (manual, after_booking, after_order ou first_booking_confirmed, com atraso_minutos), prazo_dias, canal, lembretes, perguntas e alertas (numa escala, o valor fica dentro da escala). As perguntas só mudam enquanto o formulário nunca foi enviado. O Claude confirma com você antes.
- enviar_formulario, para enviar um formulário ativo a um cliente (cliente_id ou telefone) ou a uma lista de até 200 (clientes). Confirma antes.
- cancelar_envio_formulario, para cancelar um envio ainda aberto. Confirma antes.
- marcar_formulario_sensivel, para marcar ou desmarcar o dado sensível e mudar o prazo de guarda (retencao_dias, 1 a 3650). Confirma antes.
- apagar_respostas_formulario, para apagar as respostas de um envio ou de todos os envios de um cliente quando ele pede a exclusão. Definitivo, só dono ou administrador. Confirma antes.

Exemplos: "Cria uma pesquisa de satisfação que sai 2 horas depois do atendimento", "Manda a ficha de matrícula para os clientes da etapa Novo", "Quem abriu as respostas da anamnese este mês?".

## English
Forms are answered over WhatsApp, one question at a time, in every business type. Create a form from scratch or with "Começar de um modelo" (start from a template): satisfaction survey (0 to 10 score, alert below 6), enrollment form ("Ficha de matrícula"), event sign-up ("Inscrição em evento") and, for the professional profile only, a health intake form. A form has 1 to 30 questions (text, number, scale, yes or no, single or multiple choice with 2 to 10 options, date), a reply deadline (1 to 30 days, default 7), a channel (WhatsApp, link or both), 0 to 3 reminders and owner alerts on number, scale, choice or yes/no answers; a scale alert value must be inside the scale range. Triggers: manual, after the appointment, after the delivered order, or "Primeira reserva confirmada" (first booking confirmed: once per customer, when their first booking is confirmed and before it starts), with an optional delay of up to 10080 minutes. Send manually from the customer file (Forms tab) or tick up to 200 customers in the CRM List and click "Enviar formulário". Questions freeze after the first send. Forms go out between 9am and 8pm, at most one per person per day, and every message counts toward the plan's message quota. Sensitive (health) forms ask for consent first, show answers only to the owner or an admin (each view is logged) and erase them after the retention period (1 to 3650 days, default 365). "Acessos às respostas" (owner and admins only) lists who opened or erased sensitive answers, when, which form, how many answers and through which channel (dashboard, Claude, system or the customer's WhatsApp request). Claude tools: listar_formularios, listar_respostas_formulario, listar_acessos_respostas, salvar_formulario, enviar_formulario, cancelar_envio_formulario, marcar_formulario_sensivel, apagar_respostas_formulario. Campaigns and CRM routines can carry an active link form, with a personal link per customer. Deleted or purged submissions show "Removido" as name and phone in the dashboard, the CSV and listar_respostas_formulario.
