# Atendimento / Chat

O Chat é a tela onde a equipe conversa com os clientes pelo WhatsApp, em tempo real. Cada conversa fica ligada a um contato e a uma conexão, e passa por três fases até o atendimento terminar.

Na Central de Ajuda: https://docs.convergefy.com.br/#/chat

## Em resumo

O Chat é onde a equipe fala com os clientes pelo WhatsApp. Você chega por **Barra lateral → Chat** (ícone de balão). "Conversas" e "Grupos" são os seletores no topo da lista, não o título da página.

Toda conversa está ligada a um contato e a uma conexão. Para enviar ou receber mensagens é preciso ter pelo menos uma **conexão ativa** (ver [Conexões](https://docs.convergefy.com.br/kb/conexoes.md)). Qualquer membro atende, mas quais conversas cada pessoa vê depende do dono da conversa, do departamento e das permissões (veja "Quem enxerga cada conversa").

### Algo deu errado?

Procure o que você está vendo e siga a coluna da direita. O detalhe de cada caso está mais abaixo.

| O que você vê                                                                                                            | O que fazer                                                                                                                                                                                                              |
| ------------------------------------------------------------------------------------------------------------------------ | ------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------ |
| "{nome} é responsável por essa conversa" no lugar da conversa (ou "Esta conversa está restrita")                         | A conversa é de outro atendente. Peça a transferência: o atendente responsável (ou quem pode ver todas as conversas) transfere o atendimento para você.                                                                  |
| "Todos os atendimentos deste contato estão sendo conduzidos por outros atendentes. Você não tem acesso para abrir aqui." | Peça a transferência ao colega responsável, ou a alguém que pode ver todas as conversas.                                                                                                                                 |
| "Você não tem permissão para fazer isso."                                                                                | A conversa é de outra pessoa ou de uma conexão que você não acessa: peça transferência ou apoio de quem pode ver todas.                                                                                                  |
| Conversa que não aparece na lista, ou com o conteúdo "Conteúdo restrito"                                                 | É uma conversa de uma conexão que você não pode acessar. As conexões de cada membro são definidas em [Aba "Conexões"](https://docs.convergefy.com.br/kb/equipe-permissoes.md).                                  |
| Cabeçalho com "{nome da conexão} · removida" e caixa de digitação bloqueada                                              | A conexão da conversa foi apagada. No modo único, recadastre o número (ver [Conexões](https://docs.convergefy.com.br/kb/conexoes.md)). No modo múltiplo, use o seletor para ir a outra conversa do cliente, em outro número. |
| Não aparece o seletor "Grupos"                                                                                           | Ele só aparece quando alguma conexão WhatsApp Web da empresa atende grupos (opção da aba "Grupos" da conexão).                                                                                                           |
| Mensagem que falhou ao enviar                                                                                            | Veja "Status de envio no balão" em [Enviar mensagens](https://docs.convergefy.com.br/kb/chat-mensagens.md).                                                                                                                  |

### O dia a dia em quatro passos

1. **Abrir** — Na aba Aguardando, clique na conversa do cliente que ninguém respondeu ainda.
2. **Responder** — Escreva e envie. Ao enviar, você vira o dono da conversa, e ela vai para Em Atendimento. Veja como em [Enviar mensagens](https://docs.convergefy.com.br/kb/chat-mensagens.md).
3. **Transferir, se for de outra equipe** — Clique em **"Transferir"** no cabeçalho e escolha o departamento ou o atendente.
4. **Finalizar** — Clique em **"Finalizar"**. A conversa vai para Finalizados.

**Conceitos rápidos**

- **Lead / contato** — A pessoa do outro lado da conversa (ver [Contatos](https://docs.convergefy.com.br/kb/contatos.md)).
- **Dono do atendimento** — O atendente que assumiu a conversa. Ela é dele até ser transferida ou finalizada.
- **Conexão** — O número de WhatsApp por onde a mensagem sai e entra (ver [Conexões](https://docs.convergefy.com.br/kb/conexoes.md)). Pode ser WhatsApp Web (liga por QR Code) ou API Oficial.
- **API Oficial** — O WhatsApp Business da Meta, também chamado WABA. Exige conta na Meta (ver [Conexões](https://docs.convergefy.com.br/kb/conexoes.md)).
- **Nota interna** — Recado só para a equipe, registrado na conversa. Não vai ao cliente.
- **Template** — Modelo de mensagem aprovado pela Meta, usado só em conexões da API Oficial.

## Como funciona o atendimento

### As três fases de um atendimento

Toda conversa está em uma de três situações, por isso a lista tem três abas:

- **Aguardando**: o cliente falou e ninguém respondeu ainda. Está na fila. Entra aqui quando o cliente escreve pela primeira vez, quando um cliente com conversa finalizada volta a escrever ou quando a conversa é transferida.
- **Em Atendimento**: alguém assumiu e está cuidando. Entra aqui quando alguém envia uma mensagem numa conversa que não estava em atendimento ou clica em "Reabrir" numa finalizada.
- **Finalizados**: atendimento encerrado. Entra aqui quando alguém clica em "Finalizar".

Conversa já em atendimento continua assim quando o cliente manda mais mensagens.

**Contagem de não lidas e linhas do histórico**

As abas Aguardando e Em Atendimento mostram quantas conversas têm mensagem não lida. A conta é por conversa: uma conversa com dez não lidas conta 1. Acima de 99 aparece "99+", e o número respeita os filtros ligados.

O histórico registra cada mudança numa linha cinza, por exemplo:

- _"Aguardando -> Atendimento, para Maria"_: alguém respondeu e assumiu.
- _"Atendimento -> Aguardando, de João, para departamento Vendas"_: foi transferido.
- _"Atendimento -> Finalizado, para Maria"_: foi encerrado por quem atendia.

Cada linha traz a situação anterior e a nova, e, quando se aplica, de quem, para quem e por quem foi feita. As partes que não se aplicam somem. Se a distribuição automática entregou a conversa, a linha termina com _", por distribuição automática"_. Se a conversa reabriu sozinha porque o cliente voltou a escrever, aparece só _"Finalizado -> Aguardando"_.

### Quem assume e quem vê (o "dono" da conversa)

Ao enviar uma mensagem, **você vira o dono** da conversa, até ela ser transferida ou finalizada. Assim dois atendentes não respondem o mesmo cliente ao mesmo tempo. Escrever uma nota interna não assume a conversa.

**Quem enxerga cada conversa**

- Quem pode ver todas vê todas, inclusive as de outro atendente. São os administradores e quem tem o nível Supervisor ou Administrar na área Atendimento (o que cada nível libera está em [Aba "Acesso"](https://docs.convergefy.com.br/kb/equipe-permissoes.md)).
- Os demais veem as conversas que assumiram, as sem dono (na fila) dos departamentos a que pertencem e as sem dono e sem departamento.
- Conversa de outro atendente não aparece para quem não pode ver todas. Se você abrir o contato por outra tela, pode ver _"Todos os atendimentos deste contato estão sendo conduzidos por outros atendentes."_ (ver "Permissões de acesso ao atendimento").
- Há um segundo filtro, independente do dono: conversa de uma conexão que você não pode acessar não aparece na lista, ou aparece com o conteúdo _"Conteúdo restrito"_. As conexões de cada membro são definidas em [Aba "Conexões"](https://docs.convergefy.com.br/kb/equipe-permissoes.md).

Transferir manda a conversa para a fila (Aguardando) de um departamento ou de um atendente, útil quando o assunto é de outra equipe.

Finalizar e Reabrir são reversíveis. Finalizar arquiva em Finalizados. Se o cliente escrever de novo, a conversa reabre sozinha em Aguardando, por padrão com o mesmo atendente e departamento de antes (ajuste em "Configurações de atendimento"). Já o botão "Reabrir" faz você assumir a conversa, que vai direto para Em Atendimento.

A reabertura pelo cliente conta como início de atendimento: automações com gatilho de mensagem configurado para rodar só no início do atendimento disparam de novo (ver [Automações](https://docs.convergefy.com.br/kb/automacoes.md)).

### Um número ou vários: modo único × múltiplo

A empresa funciona em um de dois modos. Não há tela para trocar: o modo é definido para a empresa (empresas novas nascem no múltiplo). Você o percebe no seletor de conexão do cabeçalho da conversa.

- **Único**: cada contato tem uma só conversa, e você escolhe de qual número enviar cada mensagem, no seletor do cabeçalho. Faz sentido com um número, ou quando tanto faz por qual responder.
- **Múltiplo**: cada contato pode ter uma conversa por número. A conversa fica presa ao número por onde o cliente falou, e o seletor alterna entre as conversas do mesmo cliente. Faz sentido com vários números (lojas, filiais) e históricos separados por linha.

> **Se a conexão da conversa for apagada**
>
> O envio fica bloqueado, a caixa de digitação desativa e o cabeçalho mostra "{nome da conexão} · removida" no lugar do seletor. No modo único, recadastre o número (ver [Conexões](https://docs.convergefy.com.br/kb/conexoes.md)). No modo múltiplo, use o seletor para ir a outra conversa do cliente, em outro número.

## A tela em 3 colunas

- **Lista de conversas (esquerda)** — Seletor "Conversas" / "Grupos", botão "Nova Conversa", busca, abas e filtros.
- **Sala da conversa (centro)** — Cabeçalho do cliente, histórico e caixa de digitação. Mensagens seguidas do mesmo remetente, pela mesma conexão e no mesmo minuto ficam agrupadas: nome e canal saem na primeira bolha, horário e status de envio na última.
- **Painel do contato (direita)** — O contato, a origem dele, os negócios, as notas internas e os agendamentos. Arraste a borda esquerda para redimensionar. O botão de painel no cabeçalho ("Ocultar informações do contato" / "Mostrar informações do contato") esconde e mostra a coluna.

**Lista de conversas (esquerda) em detalhe**

- Botão "Nova Conversa". Com a coluna estreita, aparece só o +.
- "Conversas" e, se a empresa usa grupos, "Grupos". Com grupos, "Conversas" mostra a contagem de não lidas e "Grupos" só um ponto vermelho. A contagem do topo ignora os filtros; a das abas não.
- Busca _"Buscar cliente..."_. Abaixo das conversas achadas, a seção "Iniciar nova conversa" lista contatos sem conversa. Clicar num deles abre "Abrir conversa com {nome}?" (_"A conversa ficará disponível em Em Atendimento."_) e o botão "Confirmar". No modo múltiplo, a janela também pede a conexão.
- Abas "Aguardando", "Em Atendimento" e "Finalizados". Só as duas primeiras mostram contagem.
- Filtros rápidos "Tudo", "Não lidas" e "Não respondidas" (este some em Grupos).
- Botão de filtro, com "Departamento", "Atendentes", "Conexão", "Origem", "Período" e "Tags":
  - "Atendentes" só aparece para quem pode ver todas as conversas. Quem não pode vê, em "Departamento", só os seus.
  - "Conexão" lista só as conexões que você acessa.
  - "Origem" inclui "Não rastreados" (contatos sem origem de anúncio ou link).
  - "Período" filtra por "Início da conversa" ou "Última mensagem".
- Engrenagem ao lado do filtro: "Configurações de atendimento" (seção própria abaixo). Não aparece em Grupos.
- Cada card mostra avatar, nome, data, prévia da última mensagem e a contagem de não lidas (ver [Tempo real](https://docs.convergefy.com.br/kb/tempo-real.md)).
- Contato com origem rastreada ganha um ícone antes do nome: Meta Ads, Google Ads ou Outras origens (link com UTM, a marcação de campanha no endereço, sem anúncio). Sem rastreio, sem ícone. Se veio por formulário de anúncio, o ícone leva a etiqueta "Form". Só em conversa individual.
- Lista vazia ou busca sem resultado: "Nenhuma conversa encontrada."
- Marcar como lida ou não lida: botão direito no card (computador) ou dedo pressionado (celular), depois "Marcar como não lida" / "Marcar como lida". A marcada à mão conta no filtro "Não lidas".
- Esc fecha a conversa aberta (só no computador). O cabeçalho lembra: _"Pressione Esc para fechar a conversa"_.

**Painel do contato (direita) em detalhe**

O painel começa pela foto, nome, telefone (com "Copiar telefone") e tags. Clique no nome ou telefone para editar no lugar: Enter ou clicar fora salva, Esc cancela. Nas tags, o botão "Tag" abre o seletor (ver "Marcar tags pelo painel"), o × de cada tag a remove e o "+N" mostra as que não couberam.

Editar o contato e usar "Tag" exigem o nível Editar na área Contatos. Com ele, contato sem nome mostra "Adicionar nome" e campo vazio mostra "Adicionar". Sem ele, campo vazio mostra "Não informado".

A seta à direita ("Mostrar dados do contato") abre E-mail, CPF/CNPJ, Endereço, ID Externo e os campos personalizados da empresa. Clique no valor para editar; o botão de copiar fica à direita.

Abaixo vêm as seções:

- "Origem do contato": de onde o contato veio (anúncio da Meta, do Google ou link com UTM) e as respostas de formulário de anúncio. Só aparece se houver. Detalhes em [Rastreamento](https://docs.convergefy.com.br/kb/meta-ads.md).
- "Negócios": um card por negócio (ver "Os negócios no painel"). Ao lado do título, o total em reais; no mouse: _"Soma dos negócios em aberto e dos ganhos deste contato. Negócios perdidos não entram na conta."_ Some se for zero.
- "Notas internas": da mais recente para a mais antiga. Nota longa mostra três linhas e "Ver mais". Sem nota: _"Nenhuma nota interna"_.
- "Agendamentos": cada mensagem programada com quando sai (_"Hoje às 18:00"_, _"Amanhã às 09:30"_), quanto falta (_"em 2 h"_) e o tipo (Mensagem, Nota interna, Mídia, Mensagem rápida ou Template). Sem agendamento: _"Nenhum agendamento"_.

Notas e agendamentos só carregam quando você abre a seção. A largura do painel fica salva no navegador.

Editar aqui ou na página [Contatos](https://docs.convergefy.com.br/kb/contatos.md) dá no mesmo: é o mesmo contato. Aqui você ajusta sem sair da conversa.

### Os negócios no painel

Cada negócio vira um card com produto, valor, funil e etapa, com a posição no funil (ex.: "3/7"). A faixa do topo tem a cor da etapa (verde no Ganho, vermelha na Perda). As abas "Todos", "Abertos", "Ganhos" e "Perdas" filtram os cards e mostram quantos há em cada. A lista abre em "Abertos", ou em "Todos" se não houver negócio aberto.

> **Ganho e Perda não voltam atrás**
>
> As confirmações de ganho e de perda avisam: _"Depois de marcado, o negócio não volta a ficar em aberto."_ O que trava e o que continua possível depois: [Ganhar ou perder um negócio](https://docs.convergefy.com.br/kb/funis.md).

1. **Avançar ou voltar uma etapa** — No card aberto, **"Avançar para ‹próxima etapa›"** move o negócio na hora, e a seta "Voltar para ‹etapa anterior›" desfaz o passo. Na última etapa o botão vira "Concluir como Ganho", com a mesma confirmação do Ganho.
2. **Ir direto para uma etapa** — No computador, a trilha do card aberto tem um pedaço por etapa; clicar move o negócio para ela, sem janela. No celular a trilha não aparece: use o botão de avançar.
3. **Marcar o desfecho** — O troféu (**"Marcar como ganho"**) e o x (**"Marcar como perda"**) abrem a confirmação. Os detalhes das duas janelas estão logo abaixo.

**As janelas de Ganho e de Perda**

No ganho, a janela "Marcar como Ganho?" traz o campo "Valor da venda" (_"Confira o valor fechado. Ele entra no total do funil e do contato."_) e o botão "Marcar como Ganho". Na perda, a janela é "Marcar como Perda?", com o botão "Marcar como Perda". O negócio finalizado mostra o selo Ganho ou Perda com _"Concluído em"_ e a data.

Só um card fica aberto por vez: clique num fechado para abrir e na seta para recolher. Fechado, o card em andamento mostra uma trilha pequena com a posição no funil, e o finalizado mostra o selo Ganho ou Perda.

**Editar, mover e excluir um negócio**

Em negócio em andamento, produto e valor editam no próprio card: clique no produto para buscar ou criar outro e no valor para digitar um novo (Enter salva, Esc cancela). Sem produto, o card aberto mostra "Vincular produto" e o recolhido, "Sem produto". O menu ⋯ tem "Editar", "Mover negócio" e "Excluir". Em negócio finalizado, só "Mover negócio" e "Excluir", e a trilha continua movendo a etapa. Mover de etapa pode iniciar automações da etapa de destino, como no [Funil](https://docs.convergefy.com.br/kb/funis.md).

As ações de negócio exigem o nível Operar ou Administrar na área Funis. Sem ele, os cards ficam só para consulta.

No celular o painel fica atrás do ícone do contato, então o cabeçalho ganha o botão "Negócios", que abre uma gaveta só com os negócios do contato.

### Marcar tags pelo painel

O botão "Tag" abre o seletor. O campo "Buscar ou criar tag" ("Buscar tag" para quem não gerencia tags) filtra a lista enquanto você digita. **Marque a caixinha** para vincular a tag ao contato e desmarque para tirar. Enter marca a tag de mesmo nome; se não existe, cria uma nova com a cor escolhida ("Criar "‹texto›"").

> **Excluir uma tag a tira de todos os contatos**
>
> No mouse sobre a tag aparecem editar (nome e cor) e excluir (confirma na linha: _"Excluir "‹nome›"?"_). Excluir tira a tag de todos os contatos.

Criar, editar e excluir exigem a permissão de gerenciar tags; marcar e desmarcar, a de editar contatos.

## Iniciar uma nova conversa

1. **Abrir** — Clique em **"Nova Conversa"**: _"Inicie uma nova conversa com um contato novo ou existente."_
2. **Escolher o contato** — Busque um contato (_"Buscar por nome ou telefone..."_) ou use **"Novo Lead"** (_"Criar um novo contato e iniciar conversa"_), que pede Nome, Telefone (obrigatório) e E-mail (Opcional).
3. **Confirmar** — Aparece _"Iniciar conversa com {contato}?"_ Sucesso: "Conversa iniciada com sucesso!". Pelo caminho de contato novo: "Tudo pronto! Sua nova conversa foi criada."

**Novo Lead: telefone que já existe e quem vê a opção**

Se o telefone já é de um contato, aparece _"Esse telefone já é do contato {nome}."_ com "Abrir conversa", que leva à confirmação da conversa com ele; o "Criar Conversa" fica desabilitado.

O "Novo Lead" só aparece para quem tem o nível Editar na área Contatos; sem ele, a janela diz _"Inicie uma nova conversa com um contato existente."_

**Por que já entra em 'Em Atendimento' (e não em 'Aguardando')**

Quem inicia a conversa é você, então já é o dono. Não há fila a esperar.

Escolher a conexão: no modo múltiplo a janela sempre pede o número. No modo único só pede quando o contato ainda não tem mensagem; com histórico, a conversa abre no número da última mensagem e você troca no seletor do cabeçalho ao enviar.

## O cabeçalho da conversa

No topo da sala aparecem o cliente, a conexão usada (com a bolinha de status) e as ações:

- **Seletor de conexão** — Fica no cabeçalho, não na barra de digitação. No modo único, escolhe de qual número a mensagem sai. No modo múltiplo, alterna entre as conversas do cliente.
- **Finalizar** — Encerra a conversa e a leva para Finalizados. Enquanto processa: _"Finalizando..."_.
- **Reabrir** — Aparece no lugar de "Finalizar" numa conversa finalizada (_"Reabrindo..."_). Você assume a conversa, que vai para Em Atendimento.
- **Transferir** — Passa o atendimento a outro atendente ou departamento (ver "Transferir e encaminhar" em [Enviar mensagens](https://docs.convergefy.com.br/kb/chat-mensagens.md)).
- **Automações da conversa** — O botão fica sempre no cabeçalho. Com automação rodando, vira "1 automação em execução" / "{N} automações em execução", com bolinha verde pulsando. Ao clicar, o painel "Automações da conversa" lista _"As que rodaram ou estão rodando com este contato, tenham começado sozinhas ou pela mão de alguém."_, com filtros de período e status. No modo múltiplo o botão conta só as automações daquele número, então conversas do mesmo cliente podem mostrar números diferentes.

## Configurações de atendimento

A engrenagem ao lado do filtro abre a janela lateral "Configurações de atendimento" (_"Como as conversas aparecem na lista e o que acontece ao finalizar."_), com duas partes.

- **Para você** — "Fechar conversa ao finalizar": ao finalizar, a conversa sai da tela e você volta para a lista. Desligado, ela continua aberta. Vale só para a sua conta.
- **Para toda a empresa** — Só aparece para quem tem o nível Administrar na área Atendimento, ou para administradores.

Em "Para toda a empresa":

- **Manter atendente ao finalizar** — A conversa continua com quem atendeu. Desligado, fica sem atendente ao finalizar. Vem ligado.
- **Manter departamento ao finalizar** — A conversa continua no departamento para onde foi transferida. Desligado, fica sem departamento ao finalizar. Vem ligado.
- **Distribuição de conversas** — Abre o painel "Distribuição de conversas" (_"Para quem vão as conversas que chegam sem atendente."_). Explicada em [Tags e Departamentos](https://docs.convergefy.com.br/kb/tags-departamentos.md).
- **Mostrar nome do atendente na lista** — O primeiro nome de quem atende aparece no card da conversa. Desligado, só o ícone. Vem desligado.

Como os dois primeiros vêm ligados, um cliente finalizado que volta a escrever reabre em Aguardando com o mesmo atendente e departamento.

## Grupos

O seletor "Grupos" só aparece quando alguma conexão WhatsApp Web da empresa atende grupos (opção da aba "Grupos" da conexão; ver [Conexões](https://docs.convergefy.com.br/kb/conexoes.md)). Sem isso, a lista mostra só "Conversas".

- **A lista** — Mostra os grupos, com a busca "Buscar grupo..." e os filtros "Tudo" e "Não lidas" (sem "Não respondidas"). Com mais de um número, o filtro "Número" escolhe por qual conexão o grupo chegou. Sem engrenagem de configurações. Sem grupos: _"Nenhum grupo encontrado."_ (ou _"Nenhum grupo liberado para a equipe ainda."_ para quem só vê os liberados).
- **Quem vê cada grupo** — Um grupo pode estar liberado para a empresa toda ou restrito. Quem tem o nível Supervisor na área Atendimento vê também os restritos; os demais, só os liberados.
- **Liberar ou restringir** — Quem tem o nível Administrar na área Atendimento decide. Dentro do grupo, no painel de dados, use o interruptor "Visível para toda a empresa". Na lista, botão direito no card: "Liberar grupo" / "Restringir grupo".
- **Na conversa do grupo** — Você escreve e anexa como numa conversa comum. @ abre a lista de participantes para mencionar ("Todos" menciona o grupo inteiro). O painel à direita mostra nome, descrição, quantidade de membros e a lista de participantes, com busca.

**O que muda em grupo: limites e regras**

- **O que não existe em grupo** — Nota interna, Agendar mensagem, Automações manuais, Template e os recibos de leitura.
- **Quem fala no grupo e os contatos** — Falar num grupo nunca cria contato novo: o participante só é ligado a um contato que já existe na sua base. A opção "Bloquear mensagens recebidas" do contato não vale em grupo, então o que ele escreve ali aparece normalmente. Mensagem de grupo também não dispara automação nem agente de IA e não muda o status de nenhuma conversa.
- **Grupo só para administradores** — Se o grupo só deixa administradores escreverem e a conta da conexão não é administradora, aparece um aviso acima da caixa de mensagem. O envio é recusado na hora: a mensagem fica marcada como "Não foi possível enviar" em vez de ficar pendente.
- **Avisos do WhatsApp** — Os avisos de sistema do WhatsApp, como quem entrou ou saiu do grupo, não aparecem no histórico da conversa.

Os avisos de mensagem de grupo têm configuração própria (ver [Notificações](https://docs.convergefy.com.br/kb/notificacoes.md)).

## Permissões de acesso ao atendimento

Conversa de outro atendente fica travada para quem não pode ver todas as conversas, para duas pessoas não mexerem no mesmo cliente. O que aparece depende de onde você tentou abrir:

- “{nome} é responsável por essa conversa” — tela no lugar da conversa quando ela é de outra pessoa. Se não dá para saber quem é, o título é _"Esta conversa está restrita"_, com o recado _"Peça a transferência para continuar esse atendimento."_ Resolver: peça a transferência: o atendente responsável (ou quem pode ver todas as conversas) transfere o atendimento para você.
- “Todos os atendimentos deste contato estão sendo conduzidos por outros atendentes. Você não tem acesso para abrir aqui.” — aparece ao abrir a conversa a partir de outra tela (cartão do Funil, painel de Rastreamento): nenhuma conversa desse contato está livre para você. Na tela de Chat elas simplesmente não são listadas. Resolver: peça a transferência ao colega responsável, ou a alguém que pode ver todas as conversas.
- “Você não tem permissão para fazer isso.” — aviso ao tentar agir no chat de outro atendente. Resolver: a conversa é de outra pessoa ou de uma conexão que você não acessa: peça transferência ou apoio de quem pode ver todas.
