# Automações: Ações, espera e decisões

Os blocos que mexem no atendimento e no CRM, esperam, escolhem o caminho do fluxo ou passam a conversa para um agente, e as variáveis que eles usam.

Na Central de Ajuda: https://docs.convergefy.com.br/#/automacoes-acoes

## Em resumo

Cada **bloco** é uma caixa no quadro da automação, e cada **saída** é o ponto de onde você liga o bloco ao próximo. Esta página cobre os blocos que mexem no atendimento e no CRM (CRM é o cadastro de contatos e negócios), os que esperam, os que escolhem o caminho, o que passa a conversa a um agente e as variáveis das mensagens.

### Algo deu errado?

Procure o que você está vendo e siga a coluna da direita. O detalhe de cada caso está mais abaixo.

| O que você vê                                                                                           | O que fazer                                                                                                                                                                                 |
| ------------------------------------------------------------------------------------------------------- | ------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------- |
| _"A soma das porcentagens precisa ser 100% (hoje: 90%)"_ no Randomizador                                | Ajuste as porcentagens até somarem 100%, ou use "Dividir igualmente".                                                                                                                       |
| Randomizador com resultado longe do configurado                                                         | É esperado com pouco volume: o sorteio não tem memória. Veja o aviso "A divisão é aproximada".                                                                                              |
| _"Departamento ou atendente é obrigatório"_ no passo Transferir atendimento                             | Escolha um departamento, um atendente (ou o "Atendente principal") ou os dois.                                                                                                              |
| "Etapa de destino" desativada (_"Escolha um funil primeiro"_)                                           | Escolha o Funil antes.                                                                                                                                                                      |
| _"Nem todos os caminhos que chegam aqui possuem um negócio criado…"_                                    | Coloque "Criar negócio", "Mover negócio" ou um gatilho de negócio em todos os caminhos que chegam ao passo. Veja [Ativar e acompanhar](https://docs.convergefy.com.br/kb/automacoes-ativar.md). |
| _"Adicione ao menos um dia ao horário de funcionamento."_                                               | Clique em "Adicionar horário" e marque os dias.                                                                                                                                             |
| Laço de Horário de funcionamento que para antes de o horário abrir                                      | Aumente o limite em "Máximo de vezes" (padrão 10), sob o cabeçalho "Execução" do painel.                                                                                                    |
| O agente não assumiu e o fluxo seguiu pelo "Tratamento de erro" do bloco "Transferir para agente de IA" | O agente estava pausado, em rascunho ou foi excluído, ou a conexão da conversa estava desconectada. Veja o motivo em Execuções e publique ou retome o agente, ou reconecte o número.        |
| Na triagem, o contato recebeu a resposta do agente da conexão junto com o menu                          | Deixe a conexão em "Nenhum agente". Veja [O agente nas conversas](https://docs.convergefy.com.br/kb/agentes-ia-conversas.md).                                                      |
| O passo do Agente de automação (antigo) para com "Conexão indisponível"                                 | Confira a conexão escolhida no bloco, ou ligue a saída "Tratamento de erro" para o fluxo seguir.                                                                                            |
| _"Nenhuma saída de automação publicada. Publique no agente para ramificar por elas."_                   | Publique o agente com as saídas de automação.                                                                                                                                               |

## Bloco Ações: mexer no atendimento e no CRM

> **Estes passos têm efeito na hora**
>
> - "Definir produto do negócio" **substitui** o produto atual do negócio.
> - "Cancelar execuções do contato" interrompe outras automações do contato que estejam Em andamento ou Em espera. Ele nunca cancela a si mesmo.
> - "Mover negócio" pode disparar o gatilho "Negócio movido" de outras automações.
> - "Remover tag" tira só as tags escolhidas; as demais continuam.

### Negócios

- **Criar negócio** — Abre um negócio no funil. Ajustes: Funil, Etapa inicial e o produto (Produto cadastrado, ou Nome do produto e Valor do produto). Não há campo de título: o negócio recebe o **nome do contato**. Sem nome, recebe o telefone; sem nenhum dos dois, _"Novo negócio"_.
- **Mover negócio** — Troca o negócio de etapa, **inclusive para outro funil** (ex.: de _SDR_ para _Vendas_). Ajustes: Etapa de origem, Etapa de destino (obrigatória), Dados do negócio e Criar o negócio. No seletor de etapa, os funis ficam à esquerda e as etapas do funil à direita, com busca por etapa ou funil; a primeira opção de cada funil, "Qualquer etapa", vale para o funil inteiro. **Etapa de origem** diz qual negócio mover. Em "Qualquer funil" (padrão): _"Usa o negócio que um passo anterior trouxe. Sem ele, pega o negócio mais recente do contato."_ Com uma etapa ou um funil escolhido: _"Pega o negócio do contato que está aqui. Se um passo anterior trouxe um negócio daqui, usa esse."_ Em **Dados do negócio** (Produto cadastrado, Nome do produto, Valor do produto e Observações), o que estiver preenchido muda o negócio no mesmo passo; campo vazio fica como está, então o passo não apaga dado do negócio. **"Criar o negócio se não houver um"** vem marcado em passo novo: _"Se não encontrar o negócio, cria um em {Funil › Etapa} com o nome do contato e os dados preenchidos acima."_ (antes de escolher o destino, o texto diz "na etapa de destino") Desmarcado: _"Se não encontrar o negócio, a automação termina aqui."_ Ela termina sem erro. O negócio movido ou criado passa a ser o negócio dos passos seguintes. Negócio ganho ou perdido não aceita edição: com dados preenchidos, o passo dá erro sem mover. Cair na etapa de destino pode disparar o gatilho "Negócio movido" de outras automações.
- **Finalizar negócio** — Marca como ganho ou perda. Ajuste: Status do negócio (_Ganho_ / _Perda_).
- **Definir produto do negócio** — _"Coloca um produto no negócio, no lugar do atual"_. O negócio guarda **um produto só**: _"Se o negócio já tiver um produto, ele será substituído por este."_ Há duas formas de preencher. Com um Produto cadastrado, _"Nome e valor seguem o cadastro do produto."_ e, se o preço mudar no cadastro, as próximas execuções usam o novo. Com Nome do produto e Valor do produto digitados, o negócio fica sem valor se você deixar o valor vazio. Editar nome ou valor de um produto escolhido desfaz a escolha. Se o produto for excluído do cadastro, ou o negócio já estiver ganho ou perdido, o passo segue pelo "Tratamento de erro".

**Qual negócio o Mover negócio pega**

Um negócio que um passo anterior trouxe só é usado se estiver na Etapa de origem (em "Qualquer funil", vale qualquer um). Senão, o passo procura entre os negócios do contato que estão na origem: primeiro os abertos, depois os que ainda não estão na etapa de destino e, entre eles, o mais recente. Sem contato na execução, não procura. Na aba Execuções, o passo mostra _"Nenhum negócio encontrado. A automação terminou aqui."_ ou, com a opção de criar marcada, _"Nenhum negócio encontrado. Criou um na etapa de destino."_

### Tags

- **Aplicar tag** — Marca o contato com uma tag. Ajuste: Tags (uma ou mais).
- **Remover tag** — Ajuste: Tags (obrigatório; uma ou mais): _"Tags retiradas do contato quando o passo é executado. As demais tags dele continuam."_ Se o contato não tem a tag, nada acontece e não dá erro. Tag excluída do sistema é ignorada em silêncio.

### Atendimento

- **Transferir atendimento** — Passa para outro departamento ou atendente. Ajustes: Departamento (_Qualquer departamento_ ou um da lista) e Atendente (_Qualquer atendente_, "Atendente principal" ou um da lista). Preencha pelo menos um: _"Selecione pelo menos um: departamento ou atendente."_ Com **"Atendente principal"**, o atendimento vai para o atendente principal de cada contato: _"Sem atendente principal, vai para o departamento. Sem departamento, segue pelo tratamento de erro."_ Escolher "Atendente principal" tira o atendente fixo, e vice-versa.
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
> Estes blocos decidem pelo que **encontram** ou **leem** (um contato, um negócio, o anexo, o horário). O mais livre é o **Comparar campo**, que compara um campo com um texto (_Contém_ ou _É igual a_). Condição por tag ou por número (_"se a tag for X"_, _"se o valor for maior que Y"_) **não está disponível**.

> **Esperar o horário abrir num laço**
>
> Num laço (ex.: esperar e testar o Horário de funcionamento de novo até abrir), cada volta conta no "Máximo de vezes" (padrão 10). Para esperar a próxima janela abrir, aumente esse limite em "Máximo de vezes", sob o cabeçalho "Execução" do painel.

- **Contato existente** — Procura um contato cadastrado. Ajustes: critérios (telefone, e-mail, ID externo ou tag; vários combinam como "E") e "Se achar mais de um" (_Mais recente_ / _Mais antigo_). Saídas: Encontrado / Não encontrado. Quando encontra, esse contato vira o "contato atual" do fluxo, útil logo após um gatilho de Webhook.
- **Negócio existente** — Procura um negócio. Ajustes: critérios (ID do negócio, título, ID do contato, telefone ou e-mail do contato), filtros de funil, etapa e status, e "Se achar mais de um" (_Mais recente_ / _Mais antigo_ / _Maior valor_). Saídas: Encontrado / Não encontrado.
- **É do atendente principal** — _"Verifica se o atendente principal do contato tem acesso à conexão em que a mensagem chegou e, com isso, pode responder essa conversa."_ Sem ajustes. Saídas: Sim, Não e Não tem atendente principal.
- **Tipo do anexo da mensagem** — Lê o anexo da última mensagem recebida. Sem ajustes. Saídas: Imagem, Vídeo, Áudio, Documento, Outro tipo e Sem anexo.
- **Status do atendimento** — Verifica se o atendimento está Aguardando, Em atendimento ou Finalizado. Ajuste: "Status do atendimento" (obrigatório): _"Confere a conversa em que a automação está, não as de outras conexões."_ Saídas: Sim / Não. Contato sem conversa cai em Não.
- **Comparar campo** — _"Compara um campo com um valor e segue caminhos diferentes se a condição for verdadeira ou falsa."_ Ajustes, todos obrigatórios: "Campo" (uma variável do contato, de campo personalizado, do negócio, do webhook ou de resposta de formulário da Meta), "Comparação" (_É igual a_, o padrão, ou _Contém_) e "Valor" (texto, aceita variáveis). Saídas: Condição verdadeira / Condição falsa. Veja abaixo.
- **Horário de funcionamento** — Separa quem chega dentro e fora dos dias e horários que você definir. Saídas: Dentro do horário / Fora do horário. Veja abaixo.

**Como o Comparar campo compara**

- **"É igual a"**: _"Verdadeira só quando o campo é exatamente igual ao valor, inclusive maiúsculas e minúsculas."_
- **"Contém"**: _"Verdadeira quando o valor aparece em qualquer parte do campo. Não diferencia maiúsculas de minúsculas."_
- Campo vazio, ou que o contato não tem, cai em Condição falsa.
- Campo com vários valores dá verdadeira quando algum deles casa.
- Pergunta de formulário com opções: compare com o texto da opção escolhida. O lead de teste da Meta traz texto de exemplo no lugar da opção e cai em Condição falsa.
- O gatilho "Formulário da Meta" vale para qualquer formulário, então a comparação vale para todo formulário que tenha a mesma pergunta.
- Campo, Comparação ou Valor vazio impede ativar: _"Campo é obrigatório"_, _"Valor é obrigatório"_.

**Como o Tipo do anexo agrupa os formatos**

- **Documento**: _"PDF, planilha, .zip, .txt: todo arquivo que o contato manda pelo seletor de arquivo."_
- **Outro tipo**: _"Figurinha, e arquivo cujo formato o WhatsApp não informou."_
- **Sem anexo**: _"Mensagem escrita, localização, contato compartilhado, resposta de botão."_

**Configurar o Horário de funcionamento**

- **"Dias e horários"** (obrigatório): clique em **"Adicionar horário"**, marque os dias (_Seg_ a _Dom_) e o intervalo (ex.: _09:00 – 18:00_). Dá para adicionar vários horários (um para dias úteis, outro para sábado). _"Só os dias adicionados contam como abertos."_ Sem nenhum dia: _"Adicione ao menos um dia ao horário de funcionamento."_
- **"Fuso horário"**: padrão _America/Sao\_Paulo_. _"Os horários acima são lidos neste fuso."_ Em fuso com horário de verão, o editor avisa que, nos dias da virada, uma hora não existe e outra acontece duas vezes.

## Bloco Transferir para agente de IA (categoria IA)

O bloco **"Transferir para agente de IA"** (_"O agente de IA assume a conversa e a automação termina aqui"_) funciona como transferir para um atendente: o [agente de IA](https://docs.convergefy.com.br/kb/agentes-ia.md) vira o responsável pela conversa e a **automação termina** nesse bloco. Daí em diante vale a regra do agente responsável (ver [O agente nas conversas](https://docs.convergefy.com.br/kb/agentes-ia-conversas.md)).

1. **Adicionar** — Puxe uma saída do fluxo (por exemplo, uma opção do Menu) e escolha **"Transferir para agente de IA"**, na categoria IA.
2. **Escolher o agente** — No painel, escolha o **"Agente"**. A lista mostra só agentes publicados e atendendo. Se o agente já escolhido for pausado depois, ele continua no campo, com o aviso de que não está atendendo.
3. **Ligar o tratamento de erro** — Ligue a saída **"Tratamento de erro"** a um caminho, por exemplo "Transferir atendimento" para um departamento. É por ela que o fluxo segue quando o agente não pode assumir.

- **Conexão** — "Auto: conexão da conversa" (padrão) ou uma conexão fixa, como nos outros blocos.
- **Agente (obrigatório)** — Qual agente assume a conversa. Sem agente ativo na empresa: _"Nenhum agente publicado"_, com o link "Criar agente".

* **O agente fala primeiro.** Ele não espera o contato mandar outra mensagem: lê as últimas 50 mensagens da conversa, inclusive o menu e a opção escolhida, e escreve. Ele sabe que as mensagens anteriores foram da automação, não dele.
* **Vale o horário do agente.** Fora do horário, ele segue o que você escreveu para esse caso.
* **Conversa finalizada é reaberta.** Se o bloco roda numa conversa finalizada, ela volta para "Aguardando" antes de o agente entrar.
* **Sem saída de sucesso.** O bloco encerra a automação. Ações como aplicar tag ou criar negócio vão **antes** dele: depois, o agente responde toda mensagem do contato e um bloco seguinte responderia junto.

> **Agente parado ou conexão caída sai pelo tratamento de erro**
>
> Se, na hora de rodar, o agente estiver pausado, em rascunho ou tiver sido excluído, ou se a conexão da conversa estiver desconectada, ele **não** entra na conversa e o fluxo segue pela saída "Tratamento de erro". Sem essa saída ligada, a execução falha. O nó avisa antes: _"Este agente não está atendendo. A automação vai seguir pelo tratamento de erro."_ ou _"O agente escolhido foi excluído."_

> **Triagem com vários agentes**
>
> Monte um Menu (ex.: "1. Suporte", "2. Vendas") e ligue cada opção a um "Transferir para agente de IA" com um agente diferente. Deixe a conexão sem agente: o agente da conexão entraria na primeira mensagem e responderia junto com o menu. Quando o contato volta depois de o atendimento ser finalizado, a triagem roda de novo.

## Bloco Agente de automação (antigo) (categoria IA)

O bloco "Agente de automação (antigo)" entrega a conversa a um **agente de automação**, a versão anterior dos agentes (ver [Agentes de automação](https://docs.convergefy.com.br/kb/agentes-ia-automacao.md)). O agente responde sozinho ao contato e espera o desfecho, então o bloco **pausa** o fluxo até a conversa se resolver.

> **O agente precisa estar publicado**
>
> As saídas de automação só aparecem com o agente **publicado** com elas. Sem saídas publicadas: _"Nenhuma saída de automação publicada. Publique no agente para ramificar por elas."_ Se uma saída for removida do agente, a correspondente sai do bloco (com aviso). Ver [Agentes de automação](https://docs.convergefy.com.br/kb/agentes-ia-automacao.md).

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

**Saídas do bloco Agente de automação (antigo)**

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
- **Campos personalizados do contato**: os campos que a sua empresa criou para o contato. Só aparece se houver algum. Cada um mostra o tipo: Texto, Número, Data ou Seleção.
- **Negócio**: dados do negócio.
- **Webhook**: dados da requisição recebida (fluxos iniciados pelo gatilho Webhook recebido). Webhook é o aviso que outro sistema envia para a Convergefy.
- **Dados da compra**: só aparece quando um gatilho de Gateway de pagamento chega até a mensagem.
- **Formulários da Meta**: as perguntas dos formulários de anúncio, cada uma com o tipo (Texto, ou Seleção com o número de opções). Só aparece quando a automação tem o gatilho "Formulário da Meta". A mesma pergunta em dois formulários vira uma linha só.

Variável do contato ou do formulário sem valor (ex.: pergunta que o formulário de quem respondeu não tinha) fica vazia no texto. Num parâmetro de template, ela impede o envio do template.

**Todas as variáveis de cada grupo**

- **Contato**: _ID do contato_, _Telefone do contato_, _Nome do contato_, _Primeiro Nome_, _Sobrenome_, _E-mail do contato_, _CPF/CNPJ do contato_, _Endereço do contato_, _ID externo do contato_, _Data de criação do contato_ e os dados do atendente principal (nome, conexão e ID).
- **Negócio**: ID, título, observações, produto, valor do produto, status, datas de criação e conclusão, etapa e funil.
- **Webhook**: _Método HTTP_, _Query string_, _Headers expostos_ e _Corpo da requisição_.
- **Dados da compra**: traz _Valor_, _Produto_, dados do comprador, _Link do checkout_ e, conforme a forma de pagamento, _Link do boleto_, _Linha digitável do boleto_, _Link do pix_, _Pix copia e cola_, _Vencimento do boleto_, _Validade do pix_, _Forma de pagamento_ (Boleto, Cartão ou Pix), _Nome do gateway_ e, só em cartão recusado, _Motivo da recusa_.
- **Carrinho abandonado**: não houve venda. Entram os dados do comprador, o _Produto_, o _Valor_ (o preço do produto) e o _Link do checkout_, que leva a pessoa de volta ao carrinho.

Na lista, use as setas para navegar, ← → para trocar de grupo e Enter para inserir. Para **trocar** uma variável já inserida, clique na etiqueta e escolha outra.

Os campos de botão do passo Texto (link, código e telefone) também aceitam variáveis, por exemplo para levar o _Pix copia e cola_ da compra no botão **Copiar código**.
