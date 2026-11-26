# Instagram
Link: https://aizapzap.com.br/dashboard/instagram
Para quem: todos os tipos de negócio, nos planos Negócio e Rede.

## Para que serve
Conecta o Instagram do negócio para a IA responder as mensagens do Direct. A IA usa as mesmas configurações da página WhatsApp: nome do atendente, tom e horários. Com a conta conectada, a seção Comentários mostra os comentários dos posts para você responder ou descartar.

## Como usar
1. Salve antes a página WhatsApp, porque o Instagram aproveita essas configurações.
2. Entre em Instagram e clique em "Conectar Instagram".
3. Autorize a conta na janela que abre.
4. Quando conectar, aparece o @ da conta. Para sair, use "Desconectar".
5. Abaixo do @ fica a seção Comentários, com as abas Pendentes, Respondidos e Descartados.
6. Para responder, escreva na caixa do comentário (até 300 caracteres) e clique em "Responder". A resposta é publicada no próprio post, à vista de todos.
7. Para tirar um comentário dos pendentes sem responder, clique em "Descartar". Isso não apaga o comentário no Instagram.

## Dúvidas comuns
- **Por que aparece "Ver planos"?** A conexão está disponível nos planos Negócio e Rede, e não durante o período de teste gratuito.
- **Quem pode conectar?** Só o administrador do estabelecimento.
- **A conexão expirou.** A tela mostra "Conexão expirada, conecte de novo". Basta conectar outra vez.
- **A janela de autorização não abriu.** O painel tenta continuar na mesma aba se o navegador bloqueou a janela.
- **Dá para configurar a IA só do Instagram?** Não, ela segue a configuração da página WhatsApp.
- **Os comentários não aparecem.** Só chegam os comentários feitos depois da conexão com a permissão de comentários. Se você conectou antes dessa função existir, desconecte e conecte de novo.
- **Apareceu "Este comentário já foi respondido ou descartado".** Outra pessoa da equipe (ou o Claude) já cuidou dele. A lista atualiza sozinha depois da ação.
- **Apareceu "a resposta pode ter sido publicada".** O Instagram não confirmou a tempo. Confira no post antes de tentar de novo; o painel não publica a mesma resposta duas vezes.
- **Dá para curtir um comentário?** Não. O Instagram não permite curtir comentários por integração, só responder, ocultar e apagar.

## Pelo Claude
- `ver_conversas` com canal instagram e `responder_direct`: lê e responde o Direct (uma resposta por vez, até 300 caracteres, até 24 horas depois da última mensagem do cliente).
- `ver_comentarios_instagram`: lista os comentários (pendentes, respondidos, descartados ou todos).
- `responder_comentario_instagram`: publica uma resposta pública a um comentário, com o texto que você aprovou, até 300 caracteres.
- `descartar_comentario_instagram`: tira o comentário dos pendentes sem responder.
- Conectar e desconectar a conta é só pelo painel.

## English
The Instagram page connects your business account so the AI answers Direct messages, using the same settings as the WhatsApp page. It is available on the Negócio and Rede plans (not during the free trial) and only the admin can connect. Once connected, the Comments section lists comments on your posts: reply (a public reply of up to 300 characters, posted on the post itself) or dismiss them. Liking comments is not possible through the Instagram API. Accounts connected before this feature must reconnect to receive comments. Through Claude: ver_comentarios_instagram, responder_comentario_instagram and descartar_comentario_instagram, plus ver_conversas and responder_direct for Direct messages.
