# Automações: Ações, espera e decisões

Os blocos que mexem no atendimento e no CRM, esperam, escolhem o caminho do fluxo ou passam a conversa para um agente, e as variáveis que eles usam.

Na Central de Ajuda: https://docs.convergefy.com.br/#/automacoes-acoes

## Em resumo

Cada **bloco** é uma caixa no quadro da automação, e cada **saída** é o ponto de onde você liga o bloco ao próximo. Esta página cobre os blocos que mexem no atendimento e no CRM (CRM é o cadastro de contatos e negócios), os que esperam, os que escolhem o caminho, o que passa a conversa a um agente e as variáveis das mensagens.

### Algo deu errado?

Procure o que você está vendo e siga a coluna da direita. O detalhe de cada caso está mais abaixo.

| O que você vê                                                                         | O que fazer                                                                                                                                 |
| ------------------------------------------------------------------------------------- | ------------------------------------------------------------------------------------------------------------------------------------------- |
| _"A soma das porcentagens precisa ser 100% (hoje: 90%)"_ no Randomizador              | Ajuste as porcentagens até somarem 100%, ou use "Dividir igualmente".                                                                       |
| Randomizador com resultado longe do configurado                                       | É esperado com pouco volume: o sorteio não tem memória. Veja o aviso "A divisão é aproximada".                                              |
| _"Selecione pelo menos um: departamento ou atendente."_                               | Escolha departamento, atendente ou os dois no passo Transferir atendimento.                                                                 |
| "Etapa de destino" desativada (_"Escolha um funil primeiro"_)                         | Escolha o Funil antes.                                                                                                                      |
| _"Nem todos os caminhos que chegam aqui possuem um negócio criado…"_                  | Coloque, antes do passo, um que crie ou carregue o negócio. Veja [Ativar e acompanhar](https://docs.convergefy.com.br/kb/automacoes-ativar.md). |
| _"Adicione ao menos um dia ao horário de funcionamento."_                             | Clique em "Adicionar horário" e marque os dias.                                                                                             |
| Laço de Horário de funcionamento que para antes de o horário abrir                    | Aumente o limite em "Máximo de vezes" (padrão 10), sob o cabeçalho "Execução" do painel.                                                    |
| O passo do Agente de automação para com "Conexão indisponível"                        | Confira a conexão escolhida no bloco, ou ligue a saída "Tratamento de erro" para o fluxo seguir.                                            |
| _"Nenhuma saída de automação publicada. Publique no agente para ramificar por elas."_ | Publique o agente com as saídas de automação.                                                                                               |

## Bloco Ações: mexer no atendimento e no CRM

> **Estes passos têm efeito na hora**
>
> - "Definir produto do negócio" **substitui** o produto atual do negócio.
> - "Cancelar execuções do contato" interrompe outras automações do contato que estejam Em andamento ou Em espera. Ele nunca cancela a si mesmo.
> - "Mover negócio" pode disparar o gatilho "Negócio movido" de outras automações.
> - "Remover tag" tira só as tags escolhidas; as demais continuam.

### Negócios

- **Criar negócio** — Abre um negócio no funil. Ajustes: Funil, Etapa inicial e o produto (Produto cadastrado, ou Nome do produto e Valor do produto). Não há campo de título: o negócio recebe o **nome do contato**. Sem nome, recebe o telefone; sem nenhum dos dois, _"Novo negócio"_.
- **Mover negócio** — Troca o negócio de etapa, **inclusive para outro funil** (ex.: de _SDR_ para _Vendas_). Ajustes: Funil e Etapa de destino (desativada até escolher o funil: _"Escolha um funil primeiro"_). Algum passo antes precisa ter **criado ou carregado** um negócio (veja [Ativar e acompanhar](https://docs.convergefy.com.br/kb/automacoes-ativar.md)). Cair na etapa de destino pode disparar o gatilho "Negócio movido" de outras automações.
- **Finalizar negócio** — Marca como ganho ou perda. Ajuste: Status do negócio (_Ganho_ / _Perda_).
- **Definir produto do negócio** — _"Coloca um produto no negócio, no lugar do atual"_. O negócio guarda **um produto só**: _"Se o negócio já tiver um produto, ele será substituído por este."_ Há duas formas de preencher. Com um Produto cadastrado, _"Nome e valor seguem o cadastro do produto."_ e, se o preço mudar no cadastro, as próximas execuções usam o novo. Com Nome do produto e Valor do produto digitados, o negócio fica sem valor se você deixar o valor vazio. Editar nome ou valor de um produto escolhido desfaz a escolha. Se o produto for excluído do cadastro, ou o negócio já estiver ganho ou perdido, o passo segue pelo "Tratamento de erro".

### Tags

- **Aplicar tag** — Marca o contato com uma tag. Ajuste: Tags (uma ou mais).
- **Remover tag** — Ajuste: Tags (obrigatório; uma ou mais): _"Tags retiradas do contato quando o passo é executado. As demais tags dele continuam."_ Se o contato não tem a tag, nada acontece e não dá erro. Tag excluída do sistema é ignorada em silêncio.

### Atendimento

- **Transferir atendimento** — Passa para outro departamento ou atendente. Ajuste: Departamento e/ou Atendente (_"Selecione pelo menos um: departamento ou atendente."_).
- **Iniciar atendimento** — Ajuste: o Atendente (_"O contato será atribuído a este atendente e movido para 'em atendimento'."_).
- **Reabrir atendimento** — Retoma um atendimento finalizado: devolve o contato para _Aguardando_. Atendente e departamento continuam os mesmos. Sem ajustes.
- **Finalizar atendimento** — Finaliza o atendimento do contato. Sem ajustes.

### Controle do fluxo

- **Cancelar execuções do contato** — Interrompe outras automações do contato que estejam Em andamento ou Em espera. Em "Cancelar quais automações", escolha **"Todas em execução para este contato"** ou **"Automações específicas"**. Nunca cancela a si mesma.
- **Aguardar tempo** — Pausa por um tempo (mesmo passo do bloco Espera).
- **Randomizador** — Divide os contatos por porcentagem. Veja abaixo.

### Randomizador (teste A/B)

_"Cada vez que um contato chega aqui, um dos caminhos é sorteado de acordo com as porcentagens."_ Serve para testar duas mensagens ou variações de um fluxo (teste A/B).

> **A divisão é aproximada**
>
> O sorteio é feito a cada passagem e **não tem memória**: ele não faz rodízio nem compensa o que já saiu. Com pouco volume, os caminhos ficam longe do que você configurou (ex.: 44 contatos em 3 caminhos iguais podem dar 17, 15 e 12). Por isso o Randomizador **não serve para dividir contatos de forma equilibrada entre atendentes**. Para isso, use a "Distribuição de conversas" do departamento (veja [Tags e Departamentos](https://docs.convergefy.com.br/kb/tags-departamentos.md)).

- Começa com duas ramificações, A e B, com 50% cada. Cada uma vira uma saída no quadro (ex.: _A · 50%_).
- **"Adicionar ramificação"** cria outra; **"Dividir igualmente"** reparte as porcentagens por igual. O rodapé mostra o Total.
- As porcentagens são inteiros de 0 a 100 e precisam somar 100% (_"A soma das porcentagens precisa ser 100% (hoje: 90%)"_). São necessárias pelo menos duas ramificações.
- Como cria saídas, precisa ser o **último** passo do bloco Ações.

## Bloco Espera: esperar

- **Aguardar tempo** — Ajuste: "Quanto tempo aguardar?", com 30s, 1 min, 5 min, 30 min, 1 h ou "Outro…" (_"Dá ritmo humano ao atendimento e evita parecer um robô."_). O passo novo vem com 5 minutos.
- **Aguardar resposta** — Aguarda o contato responder (mesmo passo do bloco Mensagem).
- **Aguardar evento** — Pausa até um evento. Ajustes: "Evento esperado" e "Tempo limite". Em _Status do contato alterado_, dá para filtrar Status de origem e Status de destino. Saídas: "Evento recebido" / "Tempo esgotado".

**Eventos que o Aguardar evento aceita**

Os nomes são os mesmos dos gatilhos: _Status do contato alterado_, _Contato criado_, _Atendimento transferido_, _Tag adicionada_, _Negócio criado_, _Negócio movido_, _Negócio finalizado_, _Mensagem recebida_ e _Mensagem enviada_.

Nas esperas de resposta (Menu, Menu interativo e Aguardar resposta), o tempo padrão é **1 hora**. Qualquer espera vai até no máximo **90 dias**.

## Blocos que decidem o caminho

Ficam em **Condições** no catálogo. Cada um cria **várias saídas** para você ligar a caminhos diferentes, além da saída "Tratamento de erro".

> **Não existe um bloco de “condição” genérico**
>
> Estes blocos decidem pelo que **encontram** ou **leem** (um contato, um negócio, o anexo, o horário). Condição por regra livre (_"se a tag for X"_, _"se o valor for maior que Y"_) **não está disponível**.

> **Esperar o horário abrir num laço**
>
> Num laço (ex.: esperar e testar o Horário de funcionamento de novo até abrir), cada volta conta no "Máximo de vezes" (padrão 10). Para esperar a próxima janela abrir, aumente esse limite em "Máximo de vezes", sob o cabeçalho "Execução" do painel.

- **Contato existente** — Procura um contato cadastrado. Ajustes: critérios (telefone, e-mail, ID externo ou tag; vários combinam como "E") e "Se achar mais de um" (_Mais recente_ / _Mais antigo_). Saídas: Encontrado / Não encontrado. Quando encontra, esse contato vira o "contato atual" do fluxo, útil logo após um gatilho de Webhook.
- **Negócio existente** — Procura um negócio. Ajustes: critérios (ID do negócio, título, ID do contato, telefone ou e-mail do contato), filtros de funil, etapa e status, e "Se achar mais de um" (_Mais recente_ / _Mais antigo_ / _Maior valor_). Saídas: Encontrado / Não encontrado.
- **É do atendente principal** — _"Verifica se o atendente principal do contato tem acesso à conexão em que a mensagem chegou e, com isso, pode responder essa conversa."_ Sem ajustes. Saídas: Sim, Não e Não tem atendente principal.
- **Tipo do anexo da mensagem** — Lê o anexo da última mensagem recebida. Sem ajustes. Saídas: Imagem, Vídeo, Áudio, Documento, Outro tipo e Sem anexo.
- **Status do atendimento** — Verifica se o atendimento está Aguardando, Em atendimento ou Finalizado. Ajuste: "Status do atendimento" (obrigatório): _"Vale se alguma conversa do contato estiver nesse status, em qualquer conexão."_ Saídas: Sim / Não. Contato sem conversa cai em Não.
- **Horário de funcionamento** — Separa quem chega dentro e fora dos dias e horários que você definir. Saídas: Dentro do horário / Fora do horário. Veja abaixo.

**Como o Tipo do anexo agrupa os formatos**

- **Documento**: _"PDF, planilha, .zip, .txt: todo arquivo que o contato manda pelo seletor de arquivo."_
- **Outro tipo**: _"Figurinha, e arquivo cujo formato o WhatsApp não informou."_
- **Sem anexo**: _"Mensagem escrita, localização, contato compartilhado, resposta de botão."_

**Configurar o Horário de funcionamento**

- **"Dias e horários"** (obrigatório): clique em **"Adicionar horário"**, marque os dias (_Seg_ a _Dom_) e o intervalo (ex.: _09:00 – 18:00_). Dá para adicionar vários horários (um para dias úteis, outro para sábado). _"Só os dias adicionados contam como abertos."_ Sem nenhum dia: _"Adicione ao menos um dia ao horário de funcionamento."_
- **"Fuso horário"**: padrão _America/Sao\_Paulo_. _"Os horários acima são lidos neste fuso."_ Em fuso com horário de verão, o editor avisa que, nos dias da virada, uma hora não existe e outra acontece duas vezes.

## Bloco Agente de automação (categoria IA)

O bloco "Agente de automação" entrega a conversa a um **agente** criado em [Agentes de IA](https://docs.convergefy.com.br/kb/agentes-ia.md). O agente responde sozinho ao contato e espera o desfecho, então o bloco **pausa** o fluxo até a conversa se resolver.

> **O agente precisa estar publicado**
>
> As saídas de automação só aparecem com o agente **publicado** com elas. Sem saídas publicadas: _"Nenhuma saída de automação publicada. Publique no agente para ramificar por elas."_ Se uma saída for removida do agente, a correspondente sai do bloco (com aviso). Ver [Agentes de IA](https://docs.convergefy.com.br/kb/agentes-ia.md).

> **Conexão fixa não troca sozinha**
>
> Com conexão fixa, ou com a variável "Conexão do atendente principal", o agente não troca de conexão. O passo para com o erro "Conexão indisponível" (ou segue pela saída "Tratamento de erro", se ela estiver ligada) quando:
>
> - a conexão estiver desligada;
> - o contato não tiver atendente principal;
> - o atendente não tiver conexão preferencial.

- **Conexão** — Por onde o agente responde: "Auto: conexão da conversa" (usa a conexão da conversa) ou uma conexão fixa.
- **Agente (obrigatório)** — Qual agente atende (_"Selecione um agente"_). A lista mostra o estado de cada um (Atendendo / Pausado).

**Seção "Controle" (limites da conversa)**

- **Limite de respostas** — _"Opcional. Vazio, a conversa só termina quando o contato para de responder. Preenchido, adiciona a saída 'Limite de respostas', por onde o fluxo segue ao atingir o número."_
- **Inatividade** — Tempo sem resposta do contato antes de sair por "Sem resposta do contato" (padrão **1 hora**; máximo **90 dias**).
- **Avançado: Espera mínima (s) / Espera máxima (s)** — _"Antes de responder, o agente espera o contato terminar de mandar mensagens."_ Padrão **4** e **8 segundos**, para não responder mensagem por mensagem.

**Saídas do bloco Agente de automação**

Ligue cada saída a um caminho do fluxo:

- **Atendente entrou na conversa** (blue) — um atendente humano respondeu e assumiu o atendimento; o agente para por aqui.
- **Sem resposta do contato** (blue) — o contato ficou sem responder pelo tempo de Inatividade.
- **Limite de respostas** (orange) — o agente atingiu o número máximo de respostas. Como resolver: só aparece quando você define um limite de respostas.
- **Uma saída por saída de automação publicada** (green) — cada saída de automação que o agente reconhece (ex.: _Interessado em comprar_) vira um ponto de saída próprio.

Há ainda "Tratamento de erro": _"Segue por aqui quando o agente falha, como em erro de conexão."_

## Encerrar o fluxo

- **Encerrar fluxo** — Termina a automação ali. Sem ajustes. Para também finalizar ou transferir o atendimento, coloque esses passos **antes** do encerramento.

## Variáveis

Variáveis são dados que a automação preenche com o valor de cada contato. No texto das mensagens, digite **{{** para abrir a lista. Elas aparecem como etiquetas (ex.: _Primeiro Nome_). Os grupos são:

- **Contato**: dados do contato e do atendente principal.
- **Negócio**: dados do negócio.
- **Webhook**: dados da requisição recebida (fluxos iniciados pelo gatilho Webhook recebido). Webhook é o aviso que outro sistema envia para a Convergefy.
- **Dados da compra**: só aparece quando um gatilho de Gateway de pagamento chega até a mensagem.

**Todas as variáveis de cada grupo**

- **Contato**: _ID do contato_, _Telefone do contato_, _Nome do contato_, _Primeiro Nome_, _Sobrenome_, _E-mail do contato_, _CPF/CNPJ do contato_, _Endereço do contato_, _ID externo do contato_, _Data de criação do contato_ e os dados do atendente principal (nome, conexão e ID).
- **Negócio**: ID, título, observações, produto, valor do produto, status, datas de criação e conclusão, etapa e funil.
- **Webhook**: _Método HTTP_, _Query string_, _Headers expostos_ e _Corpo da requisição_.
- **Dados da compra**: traz _Valor_, _Produto_, dados do comprador, _Link do checkout_ e, conforme a forma de pagamento, _Link do boleto_, _Linha digitável do boleto_, _Link do pix_, _Pix copia e cola_, _Vencimento do boleto_, _Validade do pix_, _Forma de pagamento_ (Boleto, Cartão ou Pix), _Nome do gateway_ e, só em cartão recusado, _Motivo da recusa_.
- **Carrinho abandonado**: não houve venda. Entram os dados do comprador, o _Produto_, o _Valor_ (o preço do produto) e o _Link do checkout_, que leva a pessoa de volta ao carrinho.

Na lista, use as setas para navegar, ← → para trocar de grupo e Enter para inserir. Para **trocar** uma variável já inserida, clique na etiqueta e escolha outra.

Os campos de botão do passo Texto (link, código e telefone) também aceitam variáveis, por exemplo para levar o _Pix copia e cola_ da compra no botão **Copiar código**.
