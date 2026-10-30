# Equipe e permissões

Aqui você gerencia quem trabalha na empresa: adiciona membros, convida pessoas por e-mail e define o acesso de cada um — Administrador (acesso total) ou um nível por área, como Atendimento, Funis e Conexões.

Na Central de Ajuda: https://docs.convergefy.com.br/#/equipe-permissoes

## Em resumo

A equipe é quem tem acesso à empresa. Cada pessoa é um **membro**, e o que ela pode fazer vem do **acesso** dela, em duas camadas:

- **Administrador**: um interruptor que dá acesso total, inclusive a dados da empresa, assinatura, gateways de pagamento, convites e ao acesso dos membros.
- **Um nível por área**: quem não é Administrador recebe, em cada área do produto (Atendimento, Contatos, Funis, Automações, Agentes de IA, Disparo em massa, Conexões, Cadastros e Rastreamento), o nível que o Administrador escolher.

> **Administrador ou Administrar?**
>
> "Administrador" é o papel da pessoa na empresa: acesso total. "Administrar" é um nível dentro de uma área, o mais alto em áreas como Conexões e Funis. O Administrador já tem tudo (as áreas aparecem como "Total"). Quem não é Administrador só tem o nível Administrar nas áreas em que o Administrador der.

### Algo deu errado?

Procure o que você está vendo e siga a coluna da direita. O detalhe de cada caso está mais abaixo.

| O que você vê                                                                                                                                                                           | O que fazer                                                                                                   |
| --------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------- | ------------------------------------------------------------------------------------------------------------- |
| Botão "Enviar Convite" desabilitado, com aviso âmbar de vagas ocupadas (ou "Todas as vagas do plano estão ocupadas. Revogue um convite pendente, remova um membro ou aumente o plano.") | Convite pendente também segura vaga. Revogue um convite na aba "Convites", remova um membro ou suba de plano. |
| Convite "Pendente" que a pessoa não consegue aceitar                                                                                                                                    | Passaram os 14 dias de validade. Revogue o convite vencido e envie um novo em "Convidar membro".              |
| "A empresa precisa de ao menos um administrador ativo."                                                                                                                                 | Promova outra pessoa a Administrador antes de tirar o acesso do último (ou de excluí-lo).                     |
| "Este usuário já pertence à empresa."                                                                                                                                                   | O e-mail convidado já é membro. Procure a pessoa na aba "Membros".                                            |
| "Só dá para revogar convites pendentes."                                                                                                                                                | O convite já foi aceito, recusado ou revogado. Não há o que revogar.                                          |
| E-mail do membro como "Pendente"                                                                                                                                                        | Peça que a pessoa abra o e-mail e confirme o endereço.                                                        |
| "Você não tem acesso a esta área"                                                                                                                                                       | O acesso é definido pelo Administrador da empresa. Fale com ele.                                              |
| Não consigo mudar o acesso, as conexões ou os departamentos de um membro                                                                                                                | Só o Administrador muda. Nem ele edita o acesso do próprio registro: outro Administrador faz isso.            |

Você faz tudo em Configurações → seção ESTRUTURA OPERACIONAL → Membros, a tela _"Gerencie os membros da sua empresa."_ Ela tem duas abas: "Membros" (quem já entrou) e "Convites" (quem foi chamado mas ainda não entrou).

> **Todo membro vê a lista, só o Administrador mexe nela**
>
> A tela de Membros não é escondida de ninguém. É onde cai quem não é Administrador ao abrir Configurações. O que muda é o que dá para fazer: a aba "Convites", o botão "Convidar membro" e a coluna "Ações" (excluir) só aparecem para o Administrador. O painel do membro fica só para consulta, e a aba "Conexões" dele só aparece para o Administrador. Cada pessoa continua podendo ajustar o próprio nome na empresa, a assinatura das mensagens e a "Conexão preferencial".

**Conceitos rápidos**

- **Membro** — Uma pessoa com acesso à empresa.
- **Administrador** — O acesso total. Cuida da estrutura da empresa: membros, convites, dados da empresa, assinatura, gateways de pagamento e o token de API da conexão. É o papel dentro da sua empresa. Não confunda com o nível "Administrar" de uma área.
- **Área** — Cada parte do produto com acesso próprio: Atendimento, Contatos, Funis, Automações, Agentes de IA, Disparo em massa, Conexões, Cadastros e Rastreamento.
- **Nível** — O quanto a pessoa pode fazer dentro de uma área (por exemplo, Ver, Operar ou Administrar). Cada área tem um nível só por membro.
- **Modelo** — Um atalho que preenche os níveis de uma vez. Existem Atendente, Operador, Gerente e Supervisor; ao ajustar uma área à mão, o conjunto passa a ser Personalizado. O modelo não é gravado: o que vale são os níveis de cada área. Alguns nomes se repetem entre modelo e nível (Atendente, Supervisor, e Operador × Operar), mas são coisas diferentes.
- **Básico** — O acesso de quem não tem nenhum nível escolhido: só o que todo membro tem. É como um convite novo começa.
- **Convite** — O jeito de trazer alguém novo: você envia para o e-mail da pessoa, e ela entra ao aceitar.

## O que só o administrador faz

Estas ações não fazem parte de nenhum nível de área. Só o Administrador tem:

- gerenciar membros: mudar o acesso, os departamentos e as conexões de cada pessoa, e excluir membros;
- convidar pessoas e revogar convites;
- Dados da empresa (Configurações → Dados da empresa);
- assinatura do plano;
- Gateways de pagamento (Configurações → Gateways de pagamento);
- token de API da conexão (aba "API" da conexão de WhatsApp Web).

Quem não tem acesso a uma área restrita não vê o item no menu e, se abrir o endereço direto, encontra a tela "Você não tem acesso a esta área": _"O acesso de cada membro é definido pelo administrador da empresa. Fale com ele se você precisar entrar aqui."_ Há o botão "Voltar para as conversas".

> **Por que existem níveis por área**
>
> Cada pessoa recebe só o que precisa: quem atende não precisa mexer em funis, e quem cuida de conexões não precisa ver o rastreamento. O Administrador ajusta o acesso de cada membro quando a função da pessoa muda.

> **Ações em massa na coluna do funil**
>
> "Excluir negócios", no menu (⋮) de uma coluna do funil, apaga os negócios daquela coluna de uma vez, sem desfazer (ver [Funis e CRM](https://docs.convergefy.com.br/kb/funis.md)). Ele exige o nível Operar em Funis, o mesmo de "Mover negócios" e "Finalizar negócios". "Disparar em massa" exige o nível Operar em Disparo em massa. Só "Exportar negócios" fica disponível para qualquer membro.

## Convidar pessoas novas

Quando alguém ainda não tem conta, você não cadastra direto: você convida. A pessoa recebe um e-mail e entra ao aceitar.

1. **Abrir o convite** — Clique em "Convidar membro". Abre um painel lateral: _"Envie um convite para adicionar novos membros à equipe."_
2. **Preencher os dados** — Informe o Nome (_"Ex: João TI"_) e o E-mail (_<email@exemplo.com>_), ambos obrigatórios. Se a empresa tiver departamentos, escolha os Departamentos (um ou vários). No bloco "Acesso" defina o acesso inicial, no mesmo editor da aba "Acesso" do membro. O convite começa no Básico.
3. **Enviar** — Clique em "Enviar Convite" (aparece "Enviando..."). A pessoa recebe o convite por e-mail e, ao aceitar, entra na empresa: "Convite aceito com sucesso".

O formulário avisa: _"O convidado começa com acesso a todas as conexões. Para restringir, abra o membro em Membros depois que ele aceitar o convite."_

> **O convite vale 14 dias**
>
> O convite aparece na aba "Convites" com uma Data de Expiração. Ele vale 14 dias. Passado esse prazo, não pode mais ser aceito e deixa de segurar vaga, embora continue aparecendo como Pendente na lista. Para convidar a pessoa de novo, revogue o convite vencido e envie um novo em "Convidar membro".

### Limite de vagas do plano

O plano tem um número de vagas, e a conta é membros + convites pendentes: um convite pendente já segura uma vaga. Em "Dados da empresa" e na tela de cobrança, o campo "Limite de membros" mostra as vagas usadas / total (ex.: 1 / 3) e, havendo convite pendente, uma linha como _"2 membros e 1 convite pendente"_. Plano sem limite mostra só "Membros" e a quantidade. Quando as vagas acabam, o painel de convite mostra um aviso âmbar logo no topo:

_"As {N} vagas do plano estão ocupadas: {X membros e Y convites pendentes}. Para convidar alguém, revogue um convite na aba Convites, remova um membro ou aumente o plano."_

Sem convites pendentes, o aviso lista só os membros e termina com _"Para convidar alguém, remova um membro ou aumente o plano."_ Nos dois casos, o botão "Enviar Convite" fica desabilitado. Se a recusa vier depois do envio, aparece _"Todas as vagas do plano estão ocupadas. Revogue um convite pendente, remova um membro ou aumente o plano."_ Confira o limite em Dados da empresa → Informações do plano (ver [Dados da empresa](https://docs.convergefy.com.br/kb/organizacao.md) e [Cobrança](https://docs.convergefy.com.br/kb/cobranca.md)).

### A aba "Convites"

Só o Administrador vê a aba. As colunas são "E-mail / Nome", "Status" e "Data de Expiração". Os status são:

- **Pendente** (amber) — o convite foi enviado e a pessoa ainda não respondeu. Segura uma vaga do plano, até vencer. Passados os 14 dias, o convite continua aparecendo como Pendente, mas já não segura vaga e não pode mais ser aceito.
- **Aceito** (green) — a pessoa aceitou e já é membro.
- **Revogado** (gray) — o convite foi cancelado por você.
- **Recusado** (red) — a pessoa recusou o convite.

**Cancelar um convite ou acompanhar do outro lado**

Convites pendentes podem ser cancelados na lixeira da linha ("Revogar"). O diálogo pergunta "Revogar Convite?": _"Isso invalidará o convite enviado para {e-mail}. Esta ação não pode ser desfeita."_ O botão mostra "Revogando..." enquanto cancela. Quem foi convidado encontra os convites recebidos em Minha conta → Convites (ver [Perfil e conta](https://docs.convergefy.com.br/kb/perfil-usuario.md)).

## Editar o acesso de um membro

Para adicionar alguém, o caminho é o convite: a pessoa precisa ter (ou criar) uma conta ao aceitar (veja Convidar pessoas novas). Para ajustar quem já entrou, **clique na linha do membro** na aba "Membros". Abre um painel lateral, à direita, com:

- o nome da pessoa no topo;
- os selos de acesso ("Administrador", o modelo ou "Básico") e de situação do e-mail ("Verificado" ou "Pendente");
- a data _"Criado em {data}"_;
- até três abas: "Informações", "Acesso" e "Conexões".

A aba "Conexões" só aparece para o Administrador e no registro da própria pessoa. Quem não é Administrador, ao abrir outro membro, vê só "Informações" e "Acesso". Não há botão "Salvar": cada ajuste **salva sozinho** na hora.

> **Só o Administrador muda o acesso e os departamentos**
>
> O acesso (aba "Acesso"), as conexões (aba "Conexões") e os departamentos de um membro só podem ser alterados por um Administrador. Cada pessoa ajusta, no máximo, os próprios dados: o Nome na empresa, a assinatura e a "Conexão preferencial". Nem o Administrador edita o acesso do próprio registro: outro Administrador faz isso.

### Aba "Informações"

1. **Contato (só leitura)** — A seção "Contato" mostra o E-mail e o Telefone do login da pessoa. Vêm da conta dela e não se editam por aqui.
2. **Na empresa** — A seção "Na empresa" mostra o "Nome na empresa" (como a pessoa aparece para a equipe; opcional, e vazio usa o nome cadastrado na conta) e os "Departamentos" a que ela pertence. Para mudar o nome, clique no nome no topo do painel (o ícone de lápis fica ao lado; Enter salva). Os departamentos são botões: clique para incluir ou tirar a pessoa de cada um. Quem não pode editar vê só o resultado (ou "Nenhum").
3. **Assinatura de mensagem** — Logo abaixo, ligue (ou não) a "Assinar mensagens com o nome" (detalhe adiante). Tudo é aplicado no ato, sem passo de salvar.

**Tirar alguém de um departamento que está na distribuição de conversas**

Se o departamento usa a distribuição de conversas e a pessoa está na lista dele, tirá-la abre uma confirmação: "Remover {nome} de {departamento}?": _"{nome} também sai da distribuição de conversas do departamento."_ Se a pessoa era a única, aparece também _"Mais ninguém recebe por ela: as conversas novas do departamento ficam na fila sem atendente."_ Os botões são "Cancelar" e "Remover". Veja a distribuição em [Tags e Departamentos](https://docs.convergefy.com.br/kb/tags-departamentos.md).

### Aba "Acesso"

Aqui o Administrador define o que a pessoa pode fazer. De cima para baixo:

- **Administrador** — Interruptor com o texto _"Acesso total, inclusive dados da empresa, assinatura, gateways de pagamento, convites e o acesso dos membros."_ Ligado, as áreas abaixo aparecem como "Total" e ficam travadas; o acesso por área fica guardado e volta se a pessoa deixar de ser Administrador.
- **Modelo** — Atalhos Atendente, Operador, Gerente e Supervisor que preenchem os níveis de uma vez, mais o selo Personalizado (a combinação feita à mão). Ao passar o mouse num modelo, a tela mostra a descrição dele. O modelo é só um atalho: depois de aplicado, ajuste cada área como quiser.
- **Áreas** — Uma linha por área, que se expande para mostrar os níveis (um por vez). A tela avisa: _"Em cada área, o nível de cima inclui tudo dos de baixo."_

> **Automações e Agentes de IA rodam como sistema**
>
> Em Automações e Agentes de IA, o nível mais alto traz o aviso: _"Automações rodam como sistema: quem as edita consegue agir em conexões fora da própria restrição."_ (e o mesmo para agentes). Ou seja, mesmo uma pessoa com restrição de conexões (aba "Conexões") pode, ao editar uma automação ou um agente, fazer algo numa conexão que ela não atende diretamente.

**Áreas e níveis, com o texto da tela**

Cada área começa num nível base (o que todo membro tem) e sobe a partir dele.

| Área                                                                              | Nível                                                                     | O que libera                                                                                                                                                                                                              |
| --------------------------------------------------------------------------------- | ------------------------------------------------------------------------- | ------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------- |
| **Atendimento**: _Conversas do chat e grupos do WhatsApp._                        | Atendente (base; nível da área Atendimento, não é o modelo de mesmo nome) | Atende os próprios chats e a fila dos seus departamentos: envia mensagens, notas internas e agendamentos, transfere, finaliza, marca como lido, usa o agente de IA e roda automações no chat. Vê os grupos não restritos. |
|                                                                                   | Supervisor (nível da área Atendimento, não é o modelo de mesmo nome)      | Vê e age em todos os chats, sem a regra de fila, dentro das conexões que pode acessar. Vê também os grupos restritos.                                                                                                     |
|                                                                                   | Administrar                                                               | Tudo do Supervisor, mais as configurações de atendimento da empresa, liberar e restringir grupos e o modo de grupos de cada conexão.                                                                                      |
| **Contatos**: _Cadastro de contatos e os dados de cada um._                       | Ver (base)                                                                | Lista e abre contatos, inclusive a aba Rastreio.                                                                                                                                                                          |
|                                                                                   | Editar                                                                    | Cria, edita, apaga e importa contatos.                                                                                                                                                                                    |
|                                                                                   | Administrar                                                               | Tudo de Editar, mais os campos personalizados e as configurações do contato.                                                                                                                                              |
| **Funis**: _Funis, etapas e negócios._                                            | Ver (base)                                                                | Vê os funis, as etapas e os negócios.                                                                                                                                                                                     |
|                                                                                   | Operar                                                                    | Cria, edita, move, finaliza e apaga negócios, um a um ou em massa.                                                                                                                                                        |
|                                                                                   | Administrar                                                               | Tudo de Operar, mais criar, editar, reordenar e apagar funis e etapas.                                                                                                                                                    |
| **Automações**: _Fluxos automáticos e as execuções deles._                        | Ver (base)                                                                | Vê as automações e as pastas e acompanha as execuções, sem alterar.                                                                                                                                                       |
|                                                                                   | Administrar                                                               | Cria, edita, ativa, pausa e apaga automações e pastas, e cancela execuções.                                                                                                                                               |
| **Agentes de IA**: _Agentes que respondem e agem pela empresa._                   | Ver (base)                                                                | Escolhe agentes e intenções dentro do editor de automações.                                                                                                                                                               |
|                                                                                   | Administrar                                                               | Cria e configura os agentes de IA.                                                                                                                                                                                        |
| **Disparo em massa**: _Campanhas de envio para listas de contatos._               | Nenhum (base)                                                             | Não vê as campanhas.                                                                                                                                                                                                      |
|                                                                                   | Operar                                                                    | Vê, cria, edita, inicia, pausa e cancela campanhas.                                                                                                                                                                       |
| **Conexões**: _Números de WhatsApp Web e API Oficial._                            | Ver (base)                                                                | Vê as conexões e os templates.                                                                                                                                                                                            |
|                                                                                   | Administrar                                                               | Cria, edita, apaga, conecta, desconecta e sincroniza conexões. Acompanha a sincronização de histórico.                                                                                                                    |
| **Cadastros**: _Departamentos, tags, mensagens rápidas e produtos._               | Ver (base)                                                                | Vê e usa departamentos, tags, mensagens rápidas e produtos.                                                                                                                                                               |
|                                                                                   | Administrar                                                               | Cria, edita e apaga departamentos, tags, mensagens rápidas e produtos.                                                                                                                                                    |
| **Rastreamento**: _Origem dos contatos e conversões enviadas para Meta e Google._ | Nenhum (base)                                                             | Não vê a tela de rastreamento.                                                                                                                                                                                            |
|                                                                                   | Ver                                                                       | Vê o dashboard, os eventos de conversão, as regras e os links mágicos (os links rastreáveis, ver [Links rastreáveis](https://docs.convergefy.com.br/kb/links-rastreaveis.md)), sem alterar.                                   |
|                                                                                   | Administrar                                                               | Tudo de Ver, mais as integrações Meta e Google Ads, sincronizar regras, criar e girar links mágicos e buscar respostas de formulários da Meta.                                                                            |

**Quando a pessoa não pode editar: o resumo de acesso**

Quem não gerencia membros vê, na aba "Acesso", um resumo somente leitura: o modelo ("Seu acesso" no próprio painel, ou "Acesso de {nome}") e, área por área, o que a pessoa consegue fazer. Áreas sem acesso (como Disparo em massa e Rastreamento no nível Nenhum) não aparecem.

### Aba "Conexões"

A seção "Conexões de atendimento" define por quais conexões a pessoa atende. Só o Administrador altera a restrição; a própria pessoa vê um resumo.

- **Acesso total às conexões** — Interruptor, ligado por padrão. Ligado: _"Atende em todas as conexões da empresa. É o padrão."_ Desligado: _"Atende só nas conexões escolhidas abaixo."_ E aparece a lista para escolher as conexões liberadas. Se desligar e não escolher nenhuma, _"Sem nenhuma conexão escolhida, o membro não atende em nenhuma conexão."_
- **Conexão preferencial** — _"Por qual conexão este membro atende por padrão. Usada para atribuir a ele as conversas que chegam por ela."_ O campo mostra "Nenhuma conexão preferencial" até alguém escolher, e só oferece as conexões que a pessoa alcança (_"Nenhuma conexão liberada."_ se não houver). A própria pessoa também escolhe a dela.

* **Administrador não tem restrição.** No painel de um Administrador, a tela diz: _"Administradores alcançam todas as conexões da empresa. Não há o que restringir aqui."_
* **Resumo para a própria pessoa** (sem permissão de editar): _"Você atende em todas as conexões da empresa."_, _"Você atende só nas conexões abaixo."_ (com as conexões liberadas) ou _"Você não atende em nenhuma conexão. Fale com um administrador."_
* Se a conexão preferencial deixar de ser permitida, a tela recusa com _"Este membro não pode usar essa conexão como principal."_

### Assinar mensagens com o nome

Na aba "Informações" há o interruptor "Assinar mensagens com o nome": _"Adiciona o nome antes de cada mensagem enviada, para o cliente saber quem está falando."_ Ligado, cada mensagem que aquele atendente manda sai com o nome dele em negrito, numa linha antes do texto. A tela mostra uma "Prévia" do resultado:

```
*João*:
Olá, tudo bem?
```

**Como a assinatura funciona na prática**

- **Que nome entra:** o "Nome na empresa". Se estiver vazio, cai para o nome cadastrado da pessoa. A Prévia (que só aparece com a opção ligada) já mostra o nome que será usado.
- **Onde aplica:** mensagens de texto e legendas de mídia. Áudio não é assinado: o WhatsApp descarta legenda em áudio.
- **Onde não entra o nome:** template da API Oficial (mensagem-modelo aprovada pela Meta), nota interna, cartão de contato, mensagem com botões ou lista e mensagem enviada num grupo. Ao editar uma mensagem já enviada, o nome também não é refeito: vale o texto que você deixar na edição.
- **Quais mensagens:** só as enviadas por um atendente (envio no Chat) e as das automações de execução manual, com o nome de quem as iniciou. Mensagens agendadas, de disparo em massa, do agente de IA, de automações que começam sozinhas e do passo Menu interativo não recebem assinatura.
- **Quem liga:** o próprio membro (na sua conta) ou quem gerencia membros (o Administrador), para qualquer membro.

## A lista de membros

A aba "Membros" tem a busca "Buscar membros..." e o filtro "Departamentos". Ao lado do título aparece o total, como _"({N} resultados)"_. As colunas são:

| Coluna        | O que mostra                                                                             |
| ------------- | ---------------------------------------------------------------------------------------- |
| Nome          | Nome na empresa (ou o nome cadastrado). Clique no título da coluna para ordenar.         |
| Contato       | E-mail e telefone da pessoa.                                                             |
| Verificado    | Ícone da situação do e-mail (ver abaixo).                                                |
| Departamentos | Os departamentos da pessoa.                                                              |
| Acesso        | "Administrador", ou o modelo do acesso (Básico, Operador, Personalizado etc.).           |
| Ações         | A lixeira para excluir. Só aparece para o Administrador, e nunca na linha de você mesmo. |

**Situação do e-mail de cada membro**

Na lista, a coluna "Verificado" mostra um ícone; passando o mouse aparece o texto. No painel do membro, o selo diz "Verificado" ou "Pendente".

- **Verificado** (green) — a pessoa confirmou o e-mail; tudo certo (passando o mouse: _"E-mail verificado"_).
- **Pendente** (amber) — falta a pessoa confirmar o e-mail (passando o mouse: _"Aguardando verificação do e-mail"_).

### Remover um membro

> **Excluir um membro não dá para desfazer**
>
> A pessoa perde o acesso à empresa. As conversas em atendimento dela voltam para Aguardando.

Dois caminhos, ambos só para o Administrador e nunca no próprio registro: o ícone de lixeira na coluna "Ações" da lista, ou o botão "Excluir membro" no rodapé do painel do membro. Abre a confirmação "Excluir {nome}?":

_"As conversas em atendimento de {nome} voltam para Aguardando. Não dá para desfazer."_

Os botões são "Cancelar" e "Excluir membro" (mostra "Excluindo..." enquanto remove), e o aviso de sucesso é "Membro removido com sucesso".

**O que acontece com as conversas e a distribuição**

As conversas que a pessoa estava atendendo voltam para "Aguardando" e, se a empresa usa a distribuição de conversas, são repassadas a outro atendente. A pessoa também é retirada de todas as regras de distribuição (da empresa e dos departamentos). Os contatos que tinham essa pessoa como atendente principal ficam sem ela. Veja [Tags e Departamentos](https://docs.convergefy.com.br/kb/tags-departamentos.md).

## Mensagens e erros esperados

Durante as ações, a tela mostra mensagens de processo: "Enviando..." ao mandar um convite, "Revogando..." ao cancelar um convite e "Excluindo..." ao remover um membro. Quando o convite é aceito, aparece "Convite aceito com sucesso".

Algumas situações comuns para ter em mente:

- **O convite não vale mais.** O convite expira depois de 14 dias ou quando é revogado. Nesse caso, envie um novo em "Convidar membro".
- **A pessoa ainda não confirmou o e-mail.** O membro entrou, mas o e-mail fica marcado como "Pendente". Peça que ela abra o e-mail e confirme o endereço.
- **O convite não é enviado.** Em geral são as vagas do plano (membros + convites pendentes): o painel mostra o aviso de vagas ocupadas. Revogue um convite, remova um membro ou suba de plano (ver [Cobrança](https://docs.convergefy.com.br/kb/cobranca.md)).
- **O acesso de administrador não muda.** A empresa precisa ter pelo menos um Administrador. Se você tentar tirar o acesso do último Administrador (ou excluí-lo), aparece _"A empresa precisa de ao menos um administrador ativo."_ Promova outra pessoa antes.
- **O e-mail convidado já é membro.** Aparece _"Este usuário já pertence à empresa."_ A pessoa já está na lista de Membros.
- **Só dá para revogar convites pendentes.** Se o convite já foi aceito, recusado ou revogado, aparece _"Só dá para revogar convites pendentes."_
