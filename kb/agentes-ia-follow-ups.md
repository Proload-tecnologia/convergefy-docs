# Agentes de IA: Follow-ups

Um follow-up faz o agente de IA retomar a conversa quando o contato para de responder: você define quanto tempo esperar e o que o agente deve dizer em cada tentativa.

Na Central de Ajuda: https://docs.convergefy.com.br/#/agentes-ia-follow-ups

## Em resumo

Um **follow-up** é uma sequência de até 10 **passos**. Cada passo diz quanto tempo esperar sem resposta do contato e o que o agente deve dizer. Quando o tempo passa, o agente escreve para o contato, com o jeito e as informações dele, seguindo a instrução do passo.

O follow-up pertence a um **agente** e só roda nas conversas em que esse agente é o responsável (ver [O agente nas conversas](https://docs.convergefy.com.br/kb/agentes-ia-conversas.md)). Cada agente pode ter **um follow-up ativo** por vez.

### Algo deu errado?

Procure o que você está vendo e siga a coluna da direita. O detalhe de cada caso está mais abaixo.

| O que você vê                                                                  | O que fazer                                                                                                                                                                                  |
| ------------------------------------------------------------------------------ | -------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------- |
| O follow-up está "Ativo", mas nada sai                                         | Ele só roda em conversas em que o agente dele é o responsável, e só depois da última mensagem da empresa. Veja "Quando o follow-up roda".                                                    |
| Selo "Sem agente"                                                              | O agente foi excluído. Abra o follow-up, escolha outro agente e ative de novo.                                                                                                               |
| "Este agente já tem outro follow-up ativo."                                    | Pause o outro follow-up desse agente antes de ativar este.                                                                                                                                   |
| "O agente precisa estar publicado."                                            | Publique o agente em "IA" → "Agentes".                                                                                                                                                       |
| Tentativa "Pulada" com _"A janela de 24 h do WhatsApp Business está fechada."_ | Na API Oficial, só dá para escrever até 24 horas depois da última mensagem do contato. Use esperas menores nessa conexão.                                                                    |
| Tentativa "Pulada"                                                             | Clique no motivo. O agente pode ter decidido não enviar (ele explica por quê) ou alguém pode ter assumido a conversa antes do envio. Ajuste a instrução do passo se não for o que você quer. |
| Tentativa "Falhou" com _"A conexão estava indisponível."_                      | Reconecte o número (ver [Conexões](https://docs.convergefy.com.br/kb/conexoes.md)).                                                                                                              |

## Onde fica

Na barra lateral, abra o menu **"IA"** e escolha **"Follow-ups"**. Tela **"Follow-ups"**: _"Mensagens que os agentes enviam quando o contato para de responder."_

Cada follow-up é um cartão com nome, selo, número de passos e uma linha como _"Assistente de Vendas · Começa após 4 h sem resposta"_. Clique no cartão para abrir. Sem nenhum: _"Nenhum follow-up"_, _"Crie um para retomar conversas de quem parou de responder."_

**Estado de cada follow-up**

- **Ativo** (green) — roda nas conversas do agente.
- **Pausado** (amber) — não roda. O que você configurou fica guardado.
- **Sem agente** (amber) — o agente dele foi excluído. Fica parado, com o histórico. Como resolver: abra o follow-up, escolha outro agente e ative de novo.

No menu "⋮" do cartão: "Pausar" ou "Ativar" (valem na hora, sem confirmação) e "Excluir". Um follow-up "Sem agente" só tem "Excluir": o agente se escolhe dentro dele.

## Criar um follow-up

1. **Abrir** — Clique em **"Novo follow-up"** e dê um nome no topo (clique em "Nome do follow-up").
2. **Escolher o agente** — Em **"Agente"** (_"Quem escreve as mensagens, com o jeito de falar, as instruções e a base de informações dele."_), escolha um agente publicado.
3. **Montar os passos** — Em **"Passos"**, defina para cada um **"Depois de … sem resposta"** e **"O que o agente deve dizer"**. Use **"Adicionar passo"** para incluir mais (até 10).
4. **Salvar ou ativar** — **"Salvar"** cria o follow-up **pausado**. **"Ativar"** cria e já põe para rodar.

- **Agente** — Só aparecem agentes publicados. Embaixo, o horário que vale: _"Envia só dentro dos horários do agente: …"_ ou _"Envia a qualquer hora, o agente não tem horário definido."_
- **Depois de … sem resposta** — De 1 a 999, em minutos, horas ou dias (1 dia = 24 horas). Um passo novo começa com 1 dia. A partir do segundo passo aparece o total acumulado, ex.: _"total: 1 dia e 4 h sem resposta"_.
- **O que o agente deve dizer** — Até 2.000 caracteres, ex.: _"pergunte se ficou alguma dúvida sobre o orçamento"_. É uma orientação: quem escreve a mensagem é o agente.

_"Cada passo sai uma vez, na ordem, contando a partir do anterior. Se o contato responder, recomeça do passo 1 no próximo silêncio."_

> **Sem rascunho**
>
> Não existe salvamento automático: "Descartar" e "Salvar" aparecem quando você muda algo. O que você salva vale a partir do próximo envio. "Ativar" e "Pausar" no topo também gravam as mudanças pendentes.

## Quando o follow-up roda

1. **O silêncio começa** — A última mensagem da conversa é da empresa (do agente, de uma automação ou de um disparo) e foi enviada sem erro. A conversa precisa ter um agente responsável com follow-up ativo.
2. **O passo sai** — Quando passa o tempo do passo 1 sem resposta, o agente escreve para o contato seguindo a instrução. O passo seguinte conta a partir dessa mensagem.
3. **Fim** — Depois do último passo, nada mais é agendado. Se o contato responder em qualquer momento, o agente segue a conversa e o follow-up recomeça do passo 1 no próximo silêncio.

**Quando o follow-up espera e quando ele para**

**Espera e tenta de novo** (a cada 5 minutos): agente pausado, agente no meio de uma resposta ou conexão desconectada. **Fora do horário do agente**, espera o próximo horário de atendimento.

**Para naquela conversa:** o contato respondeu, o atendimento foi finalizado, um atendente escreveu, o agente deixou de ser o responsável, o follow-up foi pausado ou excluído, a última mensagem falhou, a janela de 24 horas da API Oficial fechou ou o horário do agente não tem mais nenhum dia aberto. Os passos restantes não saem, e no próximo silêncio o follow-up recomeça do passo 1.

Os envios de follow-up de uma mesma conexão saem espaçados, entre 20 e 60 segundos um do outro.

## Histórico

Na aba **"Histórico"** de cada follow-up ficam todas as tentativas, com busca por contato e os filtros "Todas", "Enviadas", "Puladas" e "Falharam". Cada linha mostra o contato, o passo, a data e o motivo. "Ir para a conversa" abre o chat.

**Resultado de cada tentativa**

- **Em andamento** (blue) — _"O agente ainda está na conversa."_
- **Enviada** (green) — o agente mandou a mensagem.
- **Pulada** (amber) — nada foi enviado: o agente decidiu não enviar (com o motivo dele), alguém assumiu a conversa antes ou a janela de 24 horas da API Oficial estava fechada.
- **Falhou** (red) — _"Houve um erro ao gerar a mensagem."_, _"A conexão estava indisponível."_ ou _"O envio falhou."_ Como resolver: confira a conexão e o agente.

Uma tentativa que falhou conta como passo feito: o próximo passo segue normalmente.

## Excluir

> **Não dá para desfazer**
>
> _"“NOME” para de rodar e o histórico dele some. Não dá para desfazer."_ Se for só uma pausa, use "Pausar".

No menu "⋮" do cartão, clique em **"Excluir"** e confirme em "Excluir follow-up".

## Erros e avisos esperados

- “Escolha o agente para ativar o follow-up.” — tentaram ativar sem agente. Resolver: escolha um agente publicado e ative de novo.
- “O agente precisa estar publicado.” — o agente escolhido ainda é rascunho. Resolver: publique o agente em IA → Agentes.
- “Este agente já tem outro follow-up ativo.” — cada agente tem só um follow-up ativo. Resolver: pause o outro follow-up do agente.
- “Publique o agente para o follow-up poder enviar.” — o agente do follow-up ainda não foi publicado. Resolver: publique o agente.
- “O agente deste follow-up foi excluído. Escolha outro e ative de novo.” — o agente foi apagado. Resolver: escolha outro agente e clique em Ativar.
- “Use um número inteiro de 1 a 999.” — a espera está fora do limite. Resolver: corrija a espera do passo.
- “Diga o que o agente deve fazer neste passo.” — o passo está sem instrução. Resolver: preencha a instrução do passo.
