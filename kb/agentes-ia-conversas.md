# Agentes de IA: O agente nas conversas

Como um agente de IA entra numa conversa (pela conexão, pelo chat ou por uma automação), o que ele faz enquanto é o responsável e quando ele sai.

Na Central de Ajuda: https://docs.convergefy.com.br/#/agentes-ia-conversas

## Em resumo

Uma conversa tem no máximo um **agente responsável**. Enquanto ele é o responsável, responde toda mensagem do contato sozinho. Ele entra na conversa de três jeitos:

| Jeito                 | Quando usar                                                                              |
| --------------------- | ---------------------------------------------------------------------------------------- |
| Pela **conexão**      | O mesmo agente atende todas as conversas novas daquele número.                           |
| Pelo **chat**         | Um atendente decide colocar o agente numa conversa específica.                           |
| Por uma **automação** | O fluxo escolhe o agente, por exemplo depois de um menu "1 para Suporte, 2 para Vendas". |

O agente precisa estar **publicado e atendendo** (ver [Agentes de IA](https://docs.convergefy.com.br/kb/agentes-ia.md)). Ele sai da conversa quando um atendente manda mensagem, quando ele mesmo pede atendimento humano, quando alguém o tira, ou quando começa um atendimento novo.

### Algo deu errado?

Procure o que você está vendo e siga a coluna da direita. O detalhe de cada caso está mais abaixo.

| O que você vê                                                    | O que fazer                                                                                                                        |
| ---------------------------------------------------------------- | ---------------------------------------------------------------------------------------------------------------------------------- |
| O agente não responde a conversa                                 | Confira se ele está "Atendendo" (pausado não responde) e se a conexão da conversa está conectada. Veja também o horário do agente. |
| Você respondeu o contato e o agente parou                        | É esperado: mensagem de atendente tira o agente da conversa. Atribua de novo pelo chat se quiser.                                  |
| Na triagem, o agente da conexão respondeu junto com o menu       | Uma conversa só tem um agente: deixe a conexão em "Nenhum agente" quando usar o bloco "Transferir para agente de IA".              |
| A lista de agentes do chat está vazia: "Nenhum agente atendendo" | Publique ou retome um agente em "IA" → "Agentes".                                                                                  |
| "NOME foi atribuído. Ele responde quando a conexão voltar."      | A conexão da conversa está fora do ar. Reconecte o número (ver [Conexões](https://docs.convergefy.com.br/kb/conexoes.md)).             |
| "Este agente não atende enquanto estiver assim." na conexão      | O agente ligado à conexão está pausado ou em rascunho. Publique ou retome o agente.                                                |
| O contato voltou e o agente de antes não respondeu               | É esperado: atendimento novo começa com o agente da conexão (ou nenhum). Veja "Quando o agente sai".                               |

## O agente responsável

O agente responsável responde **toda mensagem** do contato, até sair da conversa. Antes de responder, ele espera o contato terminar de escrever (o tempo vem da aba "Config. LLM" do agente) e lê tudo de uma vez.

- **Conversa parada.** Depois de 1 hora sem resposta do contato, o agente para de esperar, mas **continua responsável**. Se o contato escrever depois, ele volta a responder.
- **Agente pausado.** Continua responsável pelas conversas em que está, mas não responde. Ao retomar, volta a responder quando o contato escrever de novo: o que chegou durante a pausa não é respondido.
- **Fora do horário.** Segue o que você escreveu em "O que o agente faz fora do horário" (ver [Horários](https://docs.convergefy.com.br/kb/agentes-ia.md)).
- **Ele lê a conversa.** O agente lê as últimas 50 mensagens da conversa, inclusive as que a automação ou os atendentes mandaram antes de ele entrar. Notas internas ficam de fora.

## Pela conexão

O agente da conexão entra nas conversas **novas** daquele número.

1. **Abrir a conexão** — Em [Conexões](https://docs.convergefy.com.br/kb/conexoes.md), clique na conexão (WhatsApp Web ou API Oficial) e abra a aba **"Agente IA"**.
2. **Escolher o agente** — Em **"Agente de IA"** (_"Quem responde sozinho as conversas novas desta conexão."_), escolha o agente. A lista só oferece agentes atendendo. Para desligar, escolha **"Nenhum agente"** (_"As conversas vão direto para a fila"_).

_"O agente entra quando uma conversa começa ou reabre nesta conexão, mesmo com atendente. Conversas em andamento não mudam."_

- Ver a aba exige o nível Administrar em Agentes de IA. Salvar a escolha exige também o nível Administrar em Conexões (ver [Equipe e permissões](https://docs.convergefy.com.br/kb/equipe-permissoes.md)).
- Se o agente da conexão for pausado ou ficar em rascunho, a aba avisa: _"Este agente não atende enquanto estiver assim. Publique ou reative para ele voltar a responder por aqui."_ Ele continua sendo colocado nas conversas novas, mas não responde.

> **Conexão com agente e triagem por automação não combinam**
>
> O agente da conexão entra logo na primeira mensagem. Se uma automação também manda um menu nessa hora, o contato recebe as duas respostas. Para triar com automação, deixe a conexão em "Nenhum agente".

## Pelo chat

No canto superior direito da conversa fica o botão do agente. Sem agente, ele mostra **"Atribuir agente responsável"**. Com agente, mostra o nome e o que ele está fazendo.

1. **Abrir** — Clique em **"Atribuir agente responsável"**.
2. **Escolher e configurar** — Escolha o **"Agente"**. Se quiser, preencha **"Instruções para esta conversa"** (até 2.000 caracteres, ex.: _"o contato pediu retorno sobre o orçamento de ontem."_) e ligue **"Enviar a primeira mensagem"**.
3. **Atribuir** — Clique em **"Atribuir"**. Aparece _"NOME foi atribuído à conversa."_

- **Agente** — Só aparecem agentes publicados e atendendo. Sem nenhum: _"Nenhum agente atendendo"_, _"Só um agente publicado e atendendo pode entrar numa conversa."_
- **Instruções para esta conversa** — Contexto que o agente usa só nesta conversa, em todas as respostas.
- **Enviar a primeira mensagem** — _"Ligado, o agente escreve para o contato assim que é atribuído. Desligado, ele espera o contato escrever. Se a última mensagem for do contato, ele responde na hora de qualquer jeito."_ Desligado por padrão.

Atribuído pelo chat, o agente atende **a qualquer hora**, mesmo fora do horário configurado nele. Quem pode responder a conversa pode atribuir, trocar ou tirar o agente.

**O que o botão do agente mostra**

- **NOME · esperando o contato** (green) — o agente está atendendo agora. O texto depois do ponto muda: "lendo o contato", "pensando…", "escrevendo…", "digitando…", "enviando…".
- **NOME responsável** (gray) — o agente é o responsável, mas não está conversando agora: _"Responde quando o contato escrever."_
- **Atribuir agente responsável** (gray) — a conversa não tem agente.

Clique no botão para ver o detalhe: o que ele está fazendo, quantas respostas deu e as **"Instruções desta conversa"**, quando houver. Quando foi uma automação que passou a conversa, aparece ali o aviso que o agente recebeu sobre a transferência.

Enquanto houver agente, a caixa de mensagem avisa: _"NOME responde esta conversa. Se você enviar uma mensagem, ele sai."_ Nota interna não tira o agente.

- **Trocar agente**: escolha outro na mesma janela. O anterior para de responder na hora.
- **Tirar da conversa**: sai na hora, sem confirmação (_"NOME saiu da conversa."_).

## Por automação

O bloco **"Transferir para agente de IA"** passa a conversa para um agente e encerra a automação, como uma transferência para um atendente. É o jeito de usar vários agentes num mesmo número: um menu pergunta o assunto e cada opção leva a um agente diferente.

O agente começa a falar sozinho, sem o contato precisar mandar outra mensagem, e sabe que a conversa veio de uma automação. Como configurar o bloco, o que acontece se o agente estiver pausado e as regras do fluxo estão em [Ações, espera e decisões](https://docs.convergefy.com.br/kb/automacoes-acoes.md).

## Quando o agente sai

**O que tira o agente da conversa**

| O que acontece                                                                                                   | O agente sai?                                                            |
| ---------------------------------------------------------------------------------------------------------------- | ------------------------------------------------------------------------ |
| Um atendente manda mensagem pelo painel ou pelo celular                                                          | Sim.                                                                     |
| O agente pede atendimento humano (ferramenta "Pedir atendimento humano")                                         | Sim, e a conversa fica com os atendentes.                                |
| Alguém clica em "Tirar da conversa" ou troca o agente                                                            | Sim.                                                                     |
| O agente é excluído                                                                                              | Sim.                                                                     |
| Começa um atendimento novo (a primeira conversa do contato, ou ele volta depois de o atendimento ser finalizado) | O responsável passa a ser o agente da conexão, ou nenhum.                |
| O agente usa "Encerrar sessão" ou o contato fica 1 hora sem responder                                            | Não: ele continua responsável e volta a responder se o contato escrever. |
| O agente é pausado                                                                                               | Não: continua responsável, só não responde até retomar.                  |
| Uma nota interna                                                                                                 | Não.                                                                     |

> **Atendimento novo começa do zero**
>
> Um agente colocado pelo chat ou por automação vale para aquele atendimento. Quando o contato volta depois de o atendimento ser finalizado, a conversa recomeça com o agente da conexão (ou sem agente), e a sua triagem roda de novo.

## Como as mensagens do agente aparecem

As mensagens do agente aparecem como enviadas pela empresa, com o selo **"Agente de IA"** (ao passar o mouse: _"Enviada pelo agente de IA"_). O selo não diz qual agente enviou. Veja [Enviar mensagens](https://docs.convergefy.com.br/kb/chat-mensagens.md).

## Erros e avisos esperados

- “O agente precisa estar publicado e atendendo.” — tentaram atribuir um agente pausado ou em rascunho. Resolver: publique ou retome o agente em IA → Agentes.
- “Outro agente entrou na conversa ao mesmo tempo.” — duas pessoas atribuíram agentes na mesma hora. Resolver: feche a janela e confira quem é o agente responsável agora.
- “Não foi possível carregar os agentes.” — a lista de agentes não carregou. Resolver: clique em Tentar de novo.
