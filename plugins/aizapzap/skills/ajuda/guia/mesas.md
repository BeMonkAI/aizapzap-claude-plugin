# Mesas (restaurante)
Link: https://aizapzap.com.br/dashboard/profile (cartão "Mesas" no Perfil do Estabelecimento). A mesa de cada reserva aparece em https://aizapzap.com.br/dashboard/reservations
Para quem: só restaurante com "Aceitar reservas" ligado no Perfil.

## Para que serve
Cadastra as mesas do restaurante, com lugares e dias em que aceitam reserva, e o tempo que cada reserva ocupa a mesa. Com mesas cadastradas, a IA só confirma reserva quando há mesa do tamanho do grupo, e o sistema escolhe a mesa sozinho (ou junta até 3). Mesa que não aceita reserva fica para quem chega sem reservar.

## Como usar
1. No Perfil, vá até o cartão "Mesas" e clique em "Adicionar mesa".
2. Preencha "Nome da mesa" e "Lugares" (de 1 a 100).
3. Ligue ou desligue "Aceita reserva" e "Pode juntar" (se a mesa pode ser unida a outras para grupos maiores).
4. Em "Dias com reserva", marque os dias da semana em que a mesa aceita reserva (seg a dom).
5. Em "Tempo de mesa por reserva", deixe "Mesma regra todos os dias" e informe os minutos, ou ligue a chave para "Varia por dia" e informe os minutos de cada dia (de 30 a 480; o padrão é 120).
6. Clique em "Salvar mesas". Esse cartão tem botão próprio, separado do "Salvar Alterações" do Perfil. O salvamento é tudo ou nada: se der erro (por exemplo, nome repetido), nada é salvo e suas edições continuam na tela para corrigir.
7. Na tela Reservas, cada reserva mostra a mesa ("Mesa: ...") ou o selo "sem mesa". Para mudar, use "Trocar mesa", escolha de 1 a 3 mesas e clique em "Salvar mesa". A troca aparece na hora na tela, sem recarregar.

## Dúvidas comuns
- **Como o sistema escolhe a mesa?** Pega a menor mesa livre que caiba o grupo. Se nenhuma couber sozinha, junta 2 e depois 3 mesas marcadas como "Pode juntar", com a menor sobra de lugares.
- **A IA conta ao cliente qual é a mesa?** Não. A IA nunca cita nem escolhe mesa. Ela também pergunta para quantas pessoas é a reserva antes de confirmar.
- **E se não houver mesa livre?** A IA não confirma aquele horário e oferece outro. No painel, "Nova reserva" avisa "Sem mesa livre para N pessoas nesse horário".
- **Qual tempo de mesa vale numa reserva?** O do dia em que a reserva começa. Mudar o tempo ou os dias de uma mesa não altera reservas já feitas.
- **O que acontece ao salvar?** Reservas futuras que ainda não tinham mesa recebem uma. Se alguma não couber, aparece o aviso "N reservas ficaram sem mesa": veja em Reservas e troque a mesa à mão.
- **Quando a mesa fica livre de novo?** Quando a reserva é cancelada, recusada ou marcada como não compareceu. A mesa de quem não compareceu volta a ficar livre e pode receber quem chega sem reservar.
- **E se a reserva ficar sem número de pessoas?** A IA sempre pergunta para quantas pessoas antes de confirmar. Se uma reserva futura ficar sem esse número, você recebe um aviso pelo WhatsApp, uma vez por reserva.
- **Posso excluir uma mesa?** Só se ela nunca teve reserva. Se já teve, use "Desativar": ela sai das novas reservas e pode voltar com "Reativar".
- **Na troca, posso escolher mesa menor que o grupo?** Sim, a decisão é sua (o painel mostra um aviso). Mesa desativada, fora dos dias de reserva ou já ocupada no horário não pode. O cliente não é avisado da troca.
- **E se eu não cadastrar mesas?** As reservas seguem como antes, sem limite de lugares. Se as mesas existem mas nenhuma aceita reserva num dia, esse dia fica sem horário de reserva.
- **Posso ter duas mesas com o mesmo nome?** Não entre as ativas.

## Pelo Claude
listar_mesas mostra as mesas (lugares, se aceita reserva, dias de reserva, se pode juntar, se está ativa) e o tempo de mesa. salvar_mesas cria ou edita mesas e o tempo de mesa (tempo_mesa_minutos para todos os dias, tempo_mesa_por_dia para dias específicos, como { sab: 180 }; null volta para a mesma regra) e conta as reservas que ficaram sem mesa. Como no painel, é tudo ou nada: se der erro, nada é salvo. Para tirar uma mesa de uso, ativa false. listar_reservas mostra as mesas de cada reserva e trocar_mesa_reserva troca a mesa de uma reserva (1 a 3 mesas, no mesmo horário). Excluir mesa: só pelo painel.

## English
Tables (restaurants with reservations on) live in the "Mesas" card of the Business Profile. Register each table with seats, whether it takes reservations, booking days and whether it can be joined, plus the table time per reservation (same every day or per day, 30 to 480 minutes, default 120). The AI only confirms a booking when a table fits the party, and the system picks the smallest fit or joins up to 3 tables; the AI never names the table. Saving is all or nothing. A table is freed when the reservation is cancelled, rejected or marked as no show, so it can take walk-ins. Reservations shows each booking's table or a "sem mesa" badge, and "Trocar mesa" swaps it, showing up right away. Claude can use listar_mesas, salvar_mesas and trocar_mesa_reserva; deleting a table is panel only.
