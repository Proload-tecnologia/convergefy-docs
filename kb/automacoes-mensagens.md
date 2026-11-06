# Automações: Mensagens e menus

Os blocos que falam com o contato: mensagem de texto e mídia, botões e menus do WhatsApp Web e templates da API Oficial.

Na Central de Ajuda: https://docs.convergefy.com.br/#/automacoes-mensagens

## Bloco Mensagem: falar com o contato

Algumas opções dependem do tipo de conexão do bloco: WhatsApp Web (liga por QR Code) ou API Oficial (o WhatsApp Business da Meta, também chamado WABA). Veja [Conexões de WhatsApp](https://docs.convergefy.com.br/kb/conexoes.md).

### Algo deu errado?

Procure o que você está vendo e siga a coluna da direita. O detalhe de cada caso está mais abaixo.

| O que você vê                                                                                                                                               | O que fazer                                                                                                                                                                  |
| ----------------------------------------------------------------------------------------------------------------------------------------------------------- | ---------------------------------------------------------------------------------------------------------------------------------------------------------------------------- |
| "Botões só funcionam em conexões WhatsApp Web. Troque a conexão do bloco Mensagem ou remova os botões para publicar." (ou o mesmo aviso do Menu interativo) | A publicação fica bloqueada. Troque a conexão do bloco por uma do WhatsApp Web ou remova os botões / o passo. Na API Oficial, use template com botões.                       |
| "O WhatsApp mostra no máximo 3 botões, e este passo tem 5. Remova 2 botões." (ou outro aviso de limite)                                                     | Ajuste ao limite do WhatsApp. A publicação fica bloqueada até lá. Veja "Limites do WhatsApp em cada formato".                                                                |
| "Template só sai por conexão da API Oficial. Escolha uma no topo do bloco ou remova este passo."                                                            | Escolha uma conexão da API Oficial no topo do bloco ou remova o passo Template.                                                                                              |
| "Nenhum template aprovado nesta conexão. Aprove um no painel da Meta."                                                                                      | Só aparecem templates já aprovados na Meta. Aprove um no painel da Meta.                                                                                                     |
| "O template selecionado não está mais disponível nesta conexão. Selecione outro."                                                                           | Escolha outro template.                                                                                                                                                      |
| Texto ou anexo não chega ao cliente na API Oficial, depois de 24h da última mensagem dele                                                                   | Use o passo Template. O editor não avisa isso no passo de texto.                                                                                                             |
| O passo falha com "Conexão indisponível"                                                                                                                    | Não há plano B: o bloco não usa outra conexão. Confira se a conexão fixa está ligada e se a variável de conexão tem valor, e ligue a saída de erro a um caminho alternativo. |

A grade de passos do bloco Mensagem mostra:

- **Texto** — Mensagem escrita. Aceita variáveis e, em conexões WhatsApp Web, botões (veja _Botões e menus interativos_).
- **Áudio** — Grave ou importe o áudio.
- **Anexo** — Imagem, vídeo ou arquivo, com legenda opcional.
- **Nota interna** — _"Só os atendentes veem. Não vai para o contato."_
- **Mensagem rápida** — Usa uma mensagem salva (veja [Mensagens rápidas](https://docs.convergefy.com.br/kb/mensagens-rapidas.md)).
- **Template** — _"Modelo aprovado pela Meta"_ (mensagem-modelo que a Meta precisa aprovar antes do uso), com o selo "API Oficial". Fica sempre na grade, mas só sai por conexão da API Oficial: com outra conexão, o passo avisa e a publicação é bloqueada (veja _Templates da API Oficial_).
- **Menu** — _"Opções escritas na mensagem"_: o cliente responde digitando. Ajustes: a mensagem; cada opção com suas "Palavras-chave esperadas" (_"Cada opção vira um caminho da automação. As palavras-chave são o que o contato pode digitar para escolher."_); e "Quanto tempo esperar pela resposta?". Saídas: uma por opção + "Outra resposta" + "Tempo esgotado".
- **Menu interativo** — _"Botões ou lista"_, com o selo "WhatsApp Web": o cliente toca na opção. Só funciona no WhatsApp Web (veja abaixo).
- **Aguardar tempo** — Pausa por um tempo (mesmo passo do bloco Espera).
- **Aguardar resposta** — Aguarda o contato responder. Ajustes: opções com "Palavras-chave esperadas" e "Quanto tempo esperar pela resposta?". Sem opções, _qualquer resposta segue pela saída "Outra resposta"._ Saídas: uma por opção + "Outra resposta" (resposta que não bate com nenhuma opção) + "Tempo esgotado".
- **Cancelar execuções do contato** — Interrompe outras automações do contato (veja _Bloco Ações_ em [Ações, espera e decisões](https://docs.convergefy.com.br/kb/automacoes-acoes.md)).

**Conexão de envio do bloco**

No topo do painel fica "Conexão de envio": _"Esta conexão será usada por todas as mensagens deste bloco."_

O padrão é "Auto: conexão da conversa": o bloco envia pela conexão da conversa em que o gatilho aconteceu. Quando dá para saber qual será, o campo mostra o nome (ex.: _"Auto · usará Comercial"_). Bloco com conexão fixa vale também para os blocos seguintes em Auto, e cada ramo do fluxo segue com a sua. Sem conversa no gatilho (como em _Tag adicionada_), vale a última conexão usada com o contato. Com gatilhos em conexões diferentes, o campo mostra _"Auto · varia conforme o gatilho"_.

Em vez de uma conexão, dá para escolher "Usar variável": a conexão vem de uma variável, como a do webhook ou a conexão do atendente principal.

> **Conexão fixa não tem plano B**
>
> Com conexão fixa (ou variável), o bloco não usa outra conexão no lugar. Se a conexão estiver desligada, ou se a variável vier vazia, o passo falha com "Conexão indisponível" (ou segue pela saída de erro, se ela estiver ligada). A variável "Conexão do atendente principal" vem vazia quando o contato não tem atendente principal ou quando esse atendente não tem conexão preferencial definida (veja [Equipe e permissões](https://docs.convergefy.com.br/kb/equipe-permissoes.md)). Se isso pode acontecer no seu fluxo, ligue a saída de erro a um caminho alternativo.

**"Mostrar digitando" (parecer mais humano)**

Nos passos de mensagem, o toggle "Mostrar digitando" (ou "Mostrar gravando", em áudio) liga o indicador de _digitando…_ / _gravando áudio…_ no WhatsApp do cliente antes do envio. Só funciona em conexões WhatsApp Web: na API Oficial o toggle nem aparece.

O passo nasce com o toggle ligado, por 5 segundos, em Texto, Áudio, Anexo, Mensagem rápida, Menu e Menu interativo. Nota interna e Template não têm o toggle.

Em "Por quanto tempo?", escolha 2s, 5s, 10s, 30s, 60s ou "Outro…", sempre entre 1 e 60 segundos. O editor confirma em palavras (_"Mostra o indicador por 5 segundos."_).

Em anexo documento o indicador não existe; em imagem ou vídeo ele exige uma legenda.

## Botões e menus interativos (WhatsApp Web)

> **Interativo é exclusivo do WhatsApp Web**
>
> Botões nativos e Menu interativo não funcionam em conexões da API Oficial, e isso não tem a ver com a janela de 24h. O campo de botões avisa _"Botões só funcionam em conexões WhatsApp Web. Troque a conexão do bloco Mensagem ou remova os botões para publicar."_ e o passo avisa _"Menu interativo só funciona em conexões WhatsApp Web. Troque a conexão do bloco Mensagem ou remova este passo para publicar."_ O Menu interativo continua na grade, com o selo "WhatsApp Web", mas a publicação é bloqueada enquanto a conexão do bloco for da API Oficial. Na API Oficial, o equivalente são os templates com botões (abaixo).

Em conexões WhatsApp Web, a automação pode mandar botões de verdade, que o cliente toca em vez de digitar o número da opção. São dois recursos:

- **Botões no passo Texto** — Botões embaixo da mensagem, para oferecer uma ação (abrir um link, copiar um cupom, ligar). Não ramifica o fluxo: _"Este passo envia e segue adiante, sem esperar resposta. Para ramificar pelo que o contato tocar, adicione um passo Aguardar resposta em seguida."_
- **Menu interativo** — Passo próprio que pergunta e espera: cada opção vira um caminho do fluxo.

### Botões numa mensagem de texto

No passo Texto, abaixo da caixa de mensagem, clique em **"Adicionar botão"**. Cada botão abre um mini-formulário:

- **Tipo** — Resposta rápida (o cliente toca e o texto do botão volta como resposta dele), Link (abre um endereço), Copiar código (copia um cupom) ou Ligar (disca um telefone). Depois aparece o campo do tipo: _"Endereço do link"_, _"Código a copiar"_ ou _"Telefone"_.
- **Texto do botão** — O que o cliente lê no botão. O contador x/20 avisa: o WhatsApp corta acima disso.

O máximo é 3 botões; ao chegar lá, "Adicionar botão" desliga e aparece _"Máximo de 3 botões no WhatsApp."_ Para reordenar, arraste pela alça à esquerda. "Ver prévia" mostra "Como fica no WhatsApp" (em maiúsculas na tela): o balão como o cliente vai ver.

### Menu interativo

No bloco Mensagem, adicione **"Menu interativo"** (na grade: _"Botões ou lista"_; no painel, o título é "Menu interativo (só WhatsApp Web)").

1. **Escrever a pergunta** — "Título": _"Opcional. Aparece em destaque acima da mensagem. Até 60 caracteres."_ Depois, a mensagem com a pergunta ou o aviso; as opções ficam abaixo dela.
2. **Escolher o formato das opções** — Com a lista de opções vazia, escolha **"Adicionar botão"** ou **"Adicionar lista"**. Botões aparecem abaixo da mensagem; a lista abre numa gaveta. Use botões para poucas opções e lista para muitas.
3. **Definir o tempo de espera** — "Quanto tempo esperar pela resposta?": 5 min, 30 min, 1 h, 6 h, 1 dia ou "Outro…". O editor confirma em palavras: _"Aguarda até 30 minutos pela resposta."_
4. **Ligar os caminhos** — Um aviso no topo do passo antecipa os caminhos (_"Este passo criará 3 saídas no canvas."_). O bloco ganha uma saída por opção, mais "Outra resposta" (o cliente digitou outra coisa) e "Tempo esgotado".

As opções são sempre resposta rápida: não há link nem telefone no Menu interativo. Dá para arrastar as opções para reordenar e conferir tudo em "Ver prévia".

**Limites do WhatsApp em cada formato**

Os limites são do WhatsApp. O editor os aplica antes de publicar, para a mensagem não ser recusada no envio.

|                      | Botões               | Lista                |
| -------------------- | -------------------- | -------------------- |
| Quantidade de opções | até 3                | até 10               |
| Texto de cada opção  | até 20 caracteres    | até 24 caracteres    |
| Texto da mensagem    | até 1.024 caracteres | até 4.096 caracteres |

O título vai até 60 caracteres nos dois formatos.

Passar de um limite bloqueia a publicação, com uma mensagem que diz o que fazer, por exemplo _"O WhatsApp mostra no máximo 3 botões, e este passo tem 5. Remova 2 botões."_ (no Menu interativo ela sugere ainda trocar para Lista, que aceita até 10) ou _"Com botões, o WhatsApp mostra no máximo 1024 caracteres na mensagem."_

## Templates da API Oficial

Na API Oficial, o WhatsApp só entrega mensagem proativa (fora de uma conversa aberta) por template aprovado pela Meta. Por isso, com uma conexão da API Oficial no bloco, o editor ganha recursos de template.

> **A janela de 24h**
>
> Na API Oficial, Texto e Anexo só chegam dentro de 24h da última mensagem do cliente. Depois disso, só template chega. Se o fluxo fala com o cliente após 24h (ex.: depois de um Aguardar tempo longo), use o passo Template. O editor não avisa isso no passo de texto.

### Enviar um template

No passo Template, a conexão da API Oficial é obrigatória. Sem ela: _"Template só sai por conexão da API Oficial. Escolha uma no topo do bloco ou remova este passo."_

1. **Escolher o template** — Clique em **"Selecionar template"**: abre "Templates aprovados" com busca (_"Buscar template…"_). A lista traz só templates aprovados na Meta, com nome, categoria e idioma. Vazio: _"Nenhum template aprovado nesta conexão. Aprove um no painel da Meta."_
2. **Preencher os parâmetros** — Se o template tem variáveis, a seção "Parâmetros" traz um campo por variável, com "Prévia" ao vivo. Cada campo aceita texto fixo ou uma variável. Sem variáveis: _"Este template não tem parâmetros para preencher."_
3. **Mídia do cabeçalho (se houver)** — Templates com cabeçalho de imagem, vídeo ou documento mostram "Mídia do cabeçalho" para anexar o arquivo, no formato que o template exige.

> **O envio de template não ramifica sozinho**
>
> O passo Template só envia, sem criar saídas. Para ramificar pela resposta de um botão de resposta rápida, o editor sugere: _"Este template tem botões de resposta rápida. Para ramificar o fluxo pelas respostas, adicione um passo Aguardar resposta em seguida."_ (botão "Adicionar passo Aguardar resposta"). Para um menu que já ramifica, use o Menu a partir de template (abaixo).

### Menu a partir de um template com botões

No passo Menu (conexão da API Oficial), o seletor Texto / Template permite usar um template com botões de resposta rápida como menu: cada botão vira uma opção, com o texto do botão fixo (só leitura), e você define as "Palavras-chave esperadas" que reconhecem a escolha. Só botões de resposta rápida geram saídas: botões de link ou telefone aparecem na prévia, mas não ramificam.

> **Limites dos templates**
>
> Cabeçalho de localização ainda não é suportado no envio. Se o template deixar de existir na conexão: _"O template selecionado não está mais disponível nesta conexão. Selecione outro."_
