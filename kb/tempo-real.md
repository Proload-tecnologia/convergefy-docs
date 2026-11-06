# Tempo real

Na Convergefy muita coisa se atualiza na tela sozinha, sem você apertar "atualizar": mensagens novas, contador de não lidas e bolinhas de status. Este guia explica por que isso acontece e o que esperar.

Na Central de Ajuda: https://docs.convergefy.com.br/#/tempo-real

## Em resumo

Você não precisa recarregar a página para ver novidades. Uma mensagem nova aparece na hora, o número de não lidas sobe e zera sozinho, e a bolinha de status muda de cor quando o número conecta ou cai. Tudo isso acontece em **tempo real**.

A ideia central deste guia: por que as coisas mudam sozinhas na sua tela e por que, às vezes, parecem "atrasadas".

### Algo deu errado?

Procure o que você está vendo e siga a coluna da direita. O detalhe de cada caso está mais abaixo.

| O que você vê                                                                                     | O que fazer                                                                                                                                                                     |
| ------------------------------------------------------------------------------------------------- | ------------------------------------------------------------------------------------------------------------------------------------------------------------------------------- |
| A tela "congela" e nada muda sozinho                                                              | Espere alguns segundos. Se nada mudou, recarregue a página e confira sua internet.                                                                                              |
| Bolinha cinza ou vermelha                                                                         | O assunto é a conexão do WhatsApp, não o tempo real. Veja [Conexões](https://docs.convergefy.com.br/kb/conexoes.md).                                                                |
| Bolinha laranja ou vermelha ("Reportada", "Qualidade Baixa", "Restringida", "Banida", "Deletada") | A decisão é da Meta, não da Convergefy. Resolva na conta Meta / WhatsApp Manager.                                                                                               |
| Bolinha vermelha "Acesso recusado"                                                                | Use "Atualizar conexão" (ver [Conexões](https://docs.convergefy.com.br/kb/conexoes.md)).                                                                                            |
| Ícone girando com "Sincronizando…"                                                                | Você pediu a sincronização e a Meta ainda não respondeu. Aguarde o ícone parar de girar.                                                                                        |
| Faixa "Sincronizando histórico" no topo do Chat                                                   | As conversas antigas entram sozinhas. Aguarde.                                                                                                                                  |
| Mensagem entrou na conversa, mas não tocou nem avisou                                             | É de propósito: mensagem do histórico (com mais de 30 segundos) não gera alerta.                                                                                                |
| As mensagens não enviam (e não é só a tela parada)                                                | O problema costuma ser a conexão ou a janela de 24h da API Oficial. Veja [Chat](https://docs.convergefy.com.br/kb/chat.md) e [Conexões](https://docs.convergefy.com.br/kb/conexoes.md). |
| Conversa com "{nome da conexão} · removida"                                                       | O envio fica bloqueado. Veja "Outros motivos de aparente atraso" e [Chat](https://docs.convergefy.com.br/kb/chat.md).                                                               |

**Conceitos rápidos**

- **Tempo real** — A tela reflete o que está acontecendo no servidor no instante em que acontece, sem você apertar "atualizar".
- **Linha direta (WebSocket)** — Uma conexão sempre aberta entre a plataforma e o servidor. Em vez de você pedir novidades, o servidor empurra as novidades para a sua tela. É como um interfone sempre aberto: quando algo muda, você ouve na hora.
- **Não lidas** — As mensagens que você ainda não abriu. Aparecem como um número (badge): nas abas, contando conversas; no card, contando mensagens daquela conversa.
- **API Oficial** — O WhatsApp Business da Meta, também chamado WABA. É o canal de conexão oficial, diferente do WhatsApp Web (que liga por QR Code).
- **Sincronizando** — Em conexão da API Oficial, aparece depois que você pede a sincronização da conexão ("Sincronizar", no menu ⋮ do cartão, ou "Sincronizar status", nas configurações da conexão): a plataforma atualiza a situação do número com a Meta. Até a Meta responder, a bolinha de status vira um ícone girando, com o texto "Sincronizando…".

## O que atualiza ao vivo

Estes itens mudam sozinhos na sua tela, sem recarregar:

- **Mensagens novas (e editadas)** — Aparecem na conversa e na lista no instante em que chegam. Se o cliente editar uma mensagem, a edição também reflete sozinha.
- **Contador de não lidas** — O número sobe quando chega algo e zera conforme você lê. Cuidado com a diferença: nas abas "Aguardando" e "Em Atendimento" o selo conta **conversas** com mensagem nova (acima de 99 vira "99+"); no card da conversa ele conta as **mensagens** dela. A aba "Finalizados" nunca mostra contagem.
- **Seletor “Conversas” / “Grupos”** — Acima das abas, esse par também avisa sozinho: "Conversas" mostra o número de conversas com mensagem nova e "Grupos" mostra só um ponto vermelho (sem número). O seletor só aparece se a empresa atende grupos. Os dois ignoram os filtros aplicados na lista: servem para você saber que há algo do outro lado, mesmo com a tela filtrada.
- **Status da conexão** — A bolinha colorida do WhatsApp muda sozinha quando o número conecta, cai ou muda de situação na Meta (ver [Conexões](https://docs.convergefy.com.br/kb/conexoes.md)). Nas conexões da API Oficial, o texto "Sincronizando…", com um ícone girando, aparece ao lado do status depois que você pede a sincronização da conexão, até a Meta responder.
- **Funil (negócios)** — Quando um negócio é criado ou movido de coluna, o quadro reflete para todos ao vivo (ver [Funis e CRM](https://docs.convergefy.com.br/kb/funis.md)).
- **Execuções de automação** — O andamento de uma automação (rodando → concluída) aparece em tempo real (ver [Automações](https://docs.convergefy.com.br/kb/automacoes.md)).

## As bolinhas de status (e o ícone girando)

A bolinha ao lado da conexão é um resumo visual da situação dela. Verde é bom; amarelo pede atenção; laranja e vermelho bloqueiam o envio. Quando você pede a sincronização da conexão ("Sincronizar" ou "Sincronizar status"), a bolinha vira um ícone girando até a Meta responder.

**O que cada cor quer dizer (resumo)**

- **Verde — tudo certo** (green) — a conexão está "Conectado" (ou "Verificada", na API Oficial) e pronta para enviar e receber.
- **Amarelo — atenção** (amber) — algo está pendente: "Aguardando QR" (falta escanear o QR), "Pendente" ou "Não Verificada" (um passo na Meta ainda não foi concluído).
- **Laranja — envio bloqueado** (orange) — a Meta limitou o número: "Reportada" (usuários reportaram spam), "Qualidade Baixa" ou "Restringida" (limite de envios). Como resolver: resolva na conta Meta / WhatsApp Manager.
- **Azul — em andamento** (blue) — a conexão está em "Preparando…", "Conectando…" ou "Migrada" (número movido de uma conta para outra na Meta).
- **Cinza — desligado** (gray) — o número está "Desconectado" / "Desconectada" ou em "Desligando…". Como resolver: reconecte a conexão.
- **Vermelho — problema sério** (red) — conexão "Banida" ou "Deletada" pela Meta, "Acesso recusado" (a Meta recusou o acesso da conexão) ou "Desconhecido" (problema que a plataforma não identificou). Como resolver: resolva na conta Meta ou recadastre; em “Acesso recusado”, use “Atualizar conexão”.

A legenda completa de cada status (com o texto exato que aparece) está em [Conexões](https://docs.convergefy.com.br/kb/conexoes.md).

> **Por que laranja e vermelho não dependem da Convergefy**
>
> Esses estados vêm de decisões da Meta sobre a sua conta (qualidade, limite de envios ou política). Quando a bolinha está laranja ou vermelha, o problema não é da plataforma: é preciso resolver na conta Meta / WhatsApp Manager. A exceção é "Acesso recusado": ele se resolve na própria Convergefy, com "Atualizar conexão" (ver [Conexões](https://docs.convergefy.com.br/kb/conexoes.md)).

## Selo de qualidade (WABA)

Conexões pela API Oficial mostram, ao lado do status, a qualidade do número definida pela Meta: "Qualidade alta", "Qualidade média" ou "Qualidade baixa". Depois que você pede a sincronização da conexão, o texto "Sincronizando…" toma o lugar da qualidade até a Meta responder.

Essa qualidade influencia diretamente se o número pode enviar mensagens. Se ela cair muito, a bolinha vira laranja ("Qualidade Baixa") e o **envio é bloqueado** até a Meta restabelecer a reputação do número.

> **Como manter a qualidade alta**
>
> Evite disparos em massa para quem não espera contato e não force conteúdo que gere bloqueios ou reportes. A qualidade é avaliada pela Meta ao longo do tempo, não pela Convergefy. Detalhes dos status da API Oficial em [Conexões](https://docs.convergefy.com.br/kb/conexoes.md).

## "Digitando…" e "gravando áudio…"

Esse aviso é o que o cliente vê no WhatsApp dele (_"digitando…"_, _"gravando áudio…"_). Ele parte de dois lugares:

- **Você, no Chat** — Quando você digita ou grava um áudio numa conversa de conexão WhatsApp Web, o cliente vê o aviso. Nota interna não emite o aviso, e conexões da API Oficial também não.
- **Automações** — Pelo toggle "Mostrar digitando" dentro de um passo de mensagem (em passo de áudio ele vira "Mostrar gravando"), para parecer mais humano. Só funciona em conexões WhatsApp Web (ver [Automações](https://docs.convergefy.com.br/kb/automacoes.md)). Passo de template não tem esse aviso.

> **Só existe do lado do cliente**
>
> A Convergefy não mostra na sua tela "o cliente está digitando": o _"digitando…"_ existe só no WhatsApp do cliente.

## Por que às vezes parece "atrasado" ou não notifica

Nem tudo que aparece na tela dispara um alerta. Isso é de propósito:

**Mensagens antigas não notificam**

Quando uma conexão liga e baixa o histórico, essas mensagens já têm mais de 30 segundos e são tratadas como "passado": entram na conversa, mas não disparam alerta sonoro nem visual.

Por quê: evita uma avalanche de notificações de mensagens velhas toda vez que o número reconecta. Se "Silenciar durante sincronização de conexão" estiver ligado (ver [Notificações](https://docs.convergefy.com.br/kb/notificacoes.md)), há ainda uma folga de \~15 segundos logo após conectar, pelo mesmo motivo. Os tempos em si são fixos do sistema: não dá para configurá-los.

**Outros motivos de aparente atraso**

- **Sincronizando histórico** — Ao conectar uma API Oficial em coexistência (quando o número já vinha sendo usado no WhatsApp Business App), quem pode gerenciar conexões vê no topo do Chat uma faixa "Sincronizando histórico" com o andamento. As conversas antigas entram sozinhas (ver [Chat](https://docs.convergefy.com.br/kb/chat.md)).
- **Sincronizando…** — Você pediu a sincronização da conexão e a Meta ainda não respondeu. Aguarde o ícone parar de girar (ver [Conexões](https://docs.convergefy.com.br/kb/conexoes.md)).
- **Conexão removida** — Se o número daquela conversa foi apagado, o envio fica bloqueado e aparece "{nome da conexão} · removida". No modo de atendimento múltiplo o seletor continua ali e dá para pular para outro número do cliente; no modo único o rótulo vem sem seletor e o caminho é recadastrar o número (ver [Chat](https://docs.convergefy.com.br/kb/chat.md)).

## Se nada estiver atualizando

Quando a tela "congela" e nada muda sozinho, em geral é uma queda momentânea da linha direta, normalmente internet instável.

Quando a linha volta, o Chat se atualiza sozinho: ele refaz as mensagens da conversa aberta, a lista de conversas e os contadores de não lidas, para recuperar o que chegou enquanto você estava sem conexão. Se várias quedas seguidas acontecem, o refazer acontece uma vez só, depois de alguns segundos.

1. **Espere alguns segundos** — Na maioria das vezes o Chat já se refaz sozinho assim que a conexão volta.
2. **Recarregue a página** — Se nada mudou, recarregar reabre a linha em tempo real; é a forma mais rápida de voltar ao normal.
3. **Confira sua internet** — Se cair de novo logo em seguida, o problema costuma ser a sua conexão de rede, não a plataforma.
4. **Veja a bolinha da conexão** — Se a bolinha estiver cinza ou vermelha, o assunto é a conexão do WhatsApp, não o tempo real. Siga para [Conexões](https://docs.convergefy.com.br/kb/conexoes.md).

> Recarregar resolve a maioria dos travamentos de tela. Se as mensagens não enviam (e não é só a tela parada), o problema costuma ser a conexão ou a janela de 24h da API Oficial. Veja [Chat](https://docs.convergefy.com.br/kb/chat.md) e [Conexões](https://docs.convergefy.com.br/kb/conexoes.md).
