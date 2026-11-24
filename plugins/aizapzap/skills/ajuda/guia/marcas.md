# Marcas
Link: https://aizapzap.com.br/dashboard/brands
Para quem: só agência de marketing. Exige plano pago ou período de teste ativo.

## Para que serve
Cadastro de cada marca que a agência atende e das pessoas que falam por ela. Cada marca tem o próprio kit, briefing, documentos e newsletter de tendências. Os responsáveis cadastrados aqui são as pessoas para quem a IA conta o andamento e de quem ela registra aprovações e ajustes, e são eles que recebem a newsletter de tendências por e-mail.

## Como usar
1. Digite o nome da marca (por exemplo, Pizzaria X) e clique em "Criar".
2. Abra a marca. Em "Responsáveis por <marca>", escolha um cliente sem marca e clique em "Adicionar". A pessoa precisa estar cadastrada antes no CRM.
3. Em "Kit da marca", envie o logo e defina cores, fonte e tom de voz. Clique em "Salvar kit".
4. Em "Briefing", preencha as respostas do cliente (as marcadas com * são obrigatórias) e clique em "Salvar briefing".
5. Em "Documentos do cliente", escolha a qual material o arquivo corresponde e clique em "Enviar arquivo". A lista "Ainda não chegou" mostra o que falta.
6. Em "Tendências para <marca>", clique em "Assinar tendências", escreva até 10 perguntas de tendência (uma por linha, por exemplo "o que está em alta em cardápio de pizzaria?"), escolha a frequência (diária, semanal ou mensal), o dia, a hora e o idioma do e-mail e clique em "Salvar". Use "Editar", "Pausar" ou "Excluir" na assinatura.
7. No fim da página, o cartão "Tendências da agência" mostra as newsletters de todas as marcas. Em "Para mim", você assina uma newsletter para o seu próprio e-mail.
8. Use "Renomear" ou "Arquivar" na lista de marcas. Marque "Mostrar arquivadas" para ver e reativar as arquivadas.

## Dúvidas comuns
- **Uma pessoa pode responder por duas marcas?** Não. Cada pessoa fica em uma marca só. Se o seletor disser "Todos os clientes já têm marca", cadastre a pessoa no CRM primeiro.
- **O que aparece em "Briefing incompleto"?** Falta resposta em alguma pergunta obrigatória. As perguntas vêm da página Processo.
- **Qual o limite dos documentos?** PDF, imagem ou zip de até 25 MB por arquivo.
- **Arquivar apaga a marca?** Não. A marca some da lista e da Gestão, mas os dados ficam. O nome volta a ficar livre.
- **Por que não consigo criar a marca?** O nome precisa ser único entre as marcas ativas, com até 80 caracteres.
- **Por que a arte da marca sai genérica?** Sem logo não dá para gerar arte; sem paleta ela usa cores neutras; com briefing incompleto ela pode sair genérica. Complete o kit e o briefing aqui.
- **O que vai na newsletter de tendências?** A IA pesquisa cada pergunta na web e manda até 3 notícias por pergunta, cada uma com resumo e o link da notícia. Só entra notícia com fonte; pergunta sem notícia nova aparece como "Sem novidades com fonte nesta edição".
- **Quem recebe?** Cada responsável da marca que tem e-mail no cadastro. É um serviço da agência para a marca, então não precisa do consentimento de novidades, mas quem pediu SAIR ou clicou em "Descadastrar" no e-mail fica de fora.
- **A agência fica sabendo do envio?** Sim. Os administradores recebem uma cópia com "[Cliente: <marca>] Tendências" no assunto, dizendo quem recebeu ou por que ninguém recebeu.
- **O que significa "Última edição"?** O resultado do último envio: enviado, nenhum responsável com e-mail, sem notícia com fonte, pesquisa na web falhou (tenta de novo na próxima edição) ou acima do limite do plano.
- **Quantas newsletters posso ter?** Uma por marca e uma "Para mim" por pessoa da equipe. Ficam ativas até 3 no Solo, 20 no Negócio e sem limite no Rede (sem assinatura paga, 1). A assinatura "Para mim" de outra pessoa só ela edita; a equipe pode excluir.

## Pelo Claude
Dá para listar as marcas ativas e ver quantos responsáveis cada uma tem (sem nome nem telefone). Marca com zero responsáveis não recebe nada pelo WhatsApp. Cadastrar, editar, arquivar e escolher responsáveis continuam só pelo painel.

Newsletter de tendências: listar_tendencias mostra as assinaturas (marca ou "para mim", perguntas, frequência, último resultado e motivo) e salvar_tendencias cria (marca_id de listar_marcas, ou para_mim) ou edita (perguntas, frequência, dia, hora, ativo: false pausa). Excluir uma assinatura é só pelo painel. Exemplo: "crie para a Pizzaria X uma newsletter semanal, segunda às 9h, com as tendências de cardápio de pizzaria e delivery".

## English
Brands is the agency's client register. Each brand has its own kit, briefing and documents (up to 25 MB each), plus the people who speak for it. Each person belongs to one brand, and those people are who the WhatsApp AI updates on progress and whose approvals and change requests it records. Each brand can also have a trend newsletter: up to 10 trend questions, daily, weekly or monthly, researched on the web by the AI and e-mailed with the link of each news to the brand's people who have an e-mail (except whoever opted out); the agency's admins get a copy with "[Cliente: <brand>]" in the subject, and "Para mim" sends one to your own e-mail. Active newsletters: 3 on Solo, 20 on Negócio, unlimited on Rede (1 without a paid plan). Through Claude you can list active brands with how many people each has, and list, create, edit or pause trend newsletters (listar_tendencias, salvar_tendencias); other editing stays in the dashboard.
