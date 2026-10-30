# Tags e Departamentos

Tags são etiquetas coloridas que você cria para classificar contatos e conversas; departamentos agrupam quem atende cada tipo de conversa e podem distribuir os atendimentos entre os atendentes. As duas organizam sua operação e aparecem no Chat, nos filtros e nas automações.

Na Central de Ajuda: https://docs.convergefy.com.br/#/tags-departamentos

## Em resumo

São duas ferramentas de organização que aparecem em vários cantos da plataforma: contatos, conversas, filtros e automações. A diferença é simples:

- **Tags** classificam: etiquetas coloridas que você inventa para marcar um cliente ou uma conversa com algo que importa para o seu negócio (_VIP_, _Quente_, _Aguardando retorno_).
- **Departamentos** agrupam e encaminham: reúnem quem atende um mesmo tipo de conversa (_Vendas_, _Suporte_, _Financeiro_). Você transfere uma conversa para um departamento e quem está nele assume. Se o departamento distribui conversas, a transferência já escolhe a pessoa. Cada departamento (e a empresa toda) ainda pode distribuir automaticamente as conversas que chegam sem atendente.

### Algo deu errado?

Procure o que você está vendo e siga a coluna da direita. O detalhe de cada caso está mais abaixo.

| O que você vê                                                                          | O que fazer                                                                                                                                                             |
| -------------------------------------------------------------------------------------- | ----------------------------------------------------------------------------------------------------------------------------------------------------------------------- |
| Não aparece o botão "Nova tag" / "Novo departamento", nem editar e excluir             | Falta o nível Administrar em Cadastros. Peça a um administrador.                                                                                                        |
| "Erro ao carregar tags" / "Erro ao carregar departamentos"                             | Clique em "Tentar novamente"; se persistir, recarregue a página.                                                                                                        |
| Ao ligar "Distribuir conversas automaticamente", abre o painel em vez de ligar         | Ninguém da lista tem porcentagem acima de 0%. Monte a lista primeiro.                                                                                                   |
| Não consigo salvar a distribuição                                                      | O total precisa fechar em 100%. O painel mostra _"Total: {N}%. Faltam {M}%."_                                                                                           |
| Conversa nova ficou na fila, sem atendente                                             | Quem está com 0% nunca é escolhido, e quem não tem acesso à conexão da conversa é pulado. Se o departamento não tem distribuição própria, a conversa fica na fila dele. |
| _"Antes de remover do departamento, tire a pessoa da distribuição de conversas dele."_ | Abra a distribuição do departamento, tire a pessoa da lista e salve; depois remova do departamento.                                                                     |
| _"Salvar vai zerar a contagem de todos."_                                              | É um aviso antes de salvar. Veja "Salvar pode zerar a contagem".                                                                                                        |

As duas telas ficam em Configurações → **ESTRUTURA OPERACIONAL**. Qualquer membro vê as telas; criar, editar e excluir tags e departamentos exige o nível **Administrar** em **Cadastros**, a área de acesso do membro que cuida de departamentos, tags e produtos (veja [Equipe e permissões](https://docs.convergefy.com.br/kb/equipe-permissoes.md)). Sem esse nível, o botão "Nova tag" / "Novo departamento" e as ações de editar e excluir não aparecem, e a tela vazia mostra só _"As tags criadas aparecem aqui."_ / _"Os departamentos criados aparecem aqui."_

**Conceitos rápidos**

- **Tag (etiqueta)** — Um rótulo colorido que você inventa para marcar contatos e conversas com algo que o sistema não sabe sozinho (ex.: _VIP_, _Inadimplente_, _Interessado no Plano X_). Cada tag tem um nome e uma cor.
- **Departamento** — Um grupo de atendentes da empresa (ex.: _Vendas_, _Suporte_). Serve para encaminhar a conversa certa para quem cuida daquele assunto.
- **Aplicar / marcar** — É quando você cola uma tag num contato ou conversa.
- **Transferir** — Encaminhar uma conversa para um departamento (ou atendente), para que ele a atenda. Ao transferir para um departamento que distribui conversas, a regra dele já escolhe quem atende.
- **Distribuição de conversas** — A divisão automática das conversas novas que chegam sem atendente entre as pessoas de uma lista, por porcentagem.
- **Etiqueta colorida (pílula)** — A tag aparecendo como uma bolinha colorida com texto, dentro de um contato ou negócio.

## Tags

### Por que usar tags

Uma tag é um rótulo que você cria para marcar clientes ou conversas com uma informação que o sistema não descobre sozinho. Vale a pena por três motivos:

- **Enxergar grupos num instante.** Com a tag _VIP_ aplicada, um filtro mostra só os VIPs no Chat ou na lista de Contatos, sem precisar lembrar quem é quem.
- **Priorizar.** Marcar _Quente_ ajuda a equipe a saber em quem focar primeiro.
- **Automatizar.** Uma automação pode reagir a uma tag (gatilho _"Tag adicionada"_), aplicar uma tag sozinha (ação _"Aplicar tag"_) ou tirar uma tag (ação _"Remover tag"_). Por exemplo: marcar _Novo lead_ ao receber a primeira mensagem e tirar _Aguardando retorno_ quando o cliente responde.

> **Criar a tag não marca ninguém**
>
> O fluxo é sempre o mesmo: você cria a tag uma vez, aplica nos contatos e conversas no dia a dia, e usa para filtrar ou disparar automações. Criar a tag só a deixa disponível como opção; ela passa a marcar alguém quando você a aplica.

### Criar ou editar uma tag

Tela "Tags": _"Classifique leads e conversas para organizar a operação."_

1. **Abrir o formulário** — Clique em **"Nova tag"** (ou **"Editar"** num card existente).
2. **Dar um nome** — Preencha o Nome, que é obrigatório. Use algo curto e claro (ex.: _VIP_, _Aguardando retorno_).
3. **Escolher a cor** — O campo "Cor" já vem preenchido com uma cor padrão, mas não pode ficar vazio. Clique no círculo para trocar; o código da cor aparece ao lado. A cor é o que torna a etiqueta fácil de reconhecer de relance.
4. **Confirmar** — Clique em **"Criar"** (ou **"Salvar"**, ao editar). A tag passa a aparecer na lista e fica disponível para aplicar.

Para encontrar uma tag na lista, use a busca "Buscar por nome". As tags aparecem em cards (cor e nome) e, onde houver contatos ou negócios, como etiquetas coloridas.

### Excluir uma tag

> **Excluir tira a etiqueta de todo mundo**
>
> Ao excluir pela tela "Tags", aparece "Excluir tag?" com o texto _"A tag {nome} será removida de todos os leads que a possuem. Esta ação não pode ser desfeita."_ Ou seja, a etiqueta some de todos os leads de uma vez e não dá para reverter. Confirme só se tiver certeza.

Também dá para excluir pelo seletor de tags (veja "Aplicar tags no dia a dia"), com a mesma consequência.

### Aplicar tags no dia a dia

No painel lateral do contato, no painel do contato dentro do Chat e no cartão do negócio, o ícone de tags abre um seletor:

- **Buscar ou criar tag** — Digite para filtrar as tags existentes. Quem tem o nível Administrar em Cadastros vê o campo como "Buscar ou criar tag": se o nome não existir, aparece a opção _Criar "{nome}"_ (com a escolha da cor) e a tag já nasce aplicada ao contato. Sem esse nível o campo é só "Buscar tag".
- **Marcar e desmarcar** — Cada tag da lista tem uma caixa: marque para vincular ao contato, desmarque para tirar. A tela avisa _"Marque para vincular ao contato."_ Quem não pode editar o contato vê _"Sem permissão para alterar as tags deste contato."_ e não consegue marcar.
- **Editar e excluir** — Quem tem o nível Administrar em Cadastros vê, ao passar o mouse numa tag, os ícones de editar (nome e cor) e excluir. Excluir pergunta _Excluir "{nome}"?_ na própria linha, com "Cancelar" e "Excluir".
- **Lista vazia** — Se não há tags, aparece _"Nenhuma tag criada ainda."_; se a busca não acha nada, _"Nenhuma tag encontrada."_

### Onde as tags são usadas

- **No contato** — Marque ou desmarque a tag pelo seletor do contato (ver [Contatos](https://docs.convergefy.com.br/kb/contatos.md)).
- **No negócio** — Gerencie as tags direto no cartão do negócio (ver [Funis e CRM](https://docs.convergefy.com.br/kb/funis.md)).
- **Nos filtros** — Filtre por tag no Chat e na lista de Contatos.
- **Nas automações** — O gatilho _"Tag adicionada"_ e as ações _"Aplicar tag"_ e _"Remover tag"_ (ver [Automações](https://docs.convergefy.com.br/kb/automacoes.md)).
- **No disparo em massa** — As tags definem quem recebe uma campanha (ver [Disparo em massa](https://docs.convergefy.com.br/kb/disparo-em-massa.md)).

**A ação Remover tag nas automações**

A ação _"Remover tag"_ (_"Tira uma tag do contato"_) é a irmã de _"Aplicar tag"_: um passo do bloco "Ações", na categoria Contato. Escolha uma ou mais tags no campo "Tags" (obrigatório): a automação tira essas tags do contato e mantém as outras. Se o contato não tinha a tag, nada acontece e a automação segue normalmente. Se uma das tags escolhidas foi excluída depois, ela é simplesmente ignorada.

## Departamentos

### Para que servem

Departamentos agrupam quem atende um mesmo tipo de conversa. Eles existem para encaminhar e organizar os atendimentos: quando uma conversa precisa de outro grupo, você a transfere para o departamento (_Suporte_, _Financeiro_…) e quem está nele assume. Uma empresa nova já nasce com um departamento chamado "Atendimento", com a pessoa que criou a empresa dentro.

### A tela "Departamentos"

Tela "Departamentos": _"Organize suas equipes operacionais."_ Os departamentos aparecem em cards, cada um com o nome e a quantidade de membros (_"1 membro"_, _"3 membros"_). Clicar no card inteiro abre o painel do departamento. Quem pode excluir vê também a lixeira no card.

### Criar um departamento

1. **Abrir o formulário** — Clique em **"Novo departamento"**. Abre o painel "Novo departamento": _"Agrupa quem atende um mesmo tipo de conversa."_
2. **Dar um nome** — Preencha o Nome (ex.: _Vendas_), que é obrigatório. É o único campo.
3. **Criar** — Clique em **"Criar"**. Aparece "Departamento criado com sucesso". A tela lembra: _"Depois de criar, abra o departamento para adicionar quem atende por ele e configurar a distribuição."_ (a frase muda conforme o que você tem permissão de fazer).

### O painel do departamento

Ao clicar no card, abre um painel lateral com o nome no topo, a quantidade de membros e as seções abaixo.

- **Nome** — Clique no nome para editar. Salva ao sair do campo (Enter também confirma); Esc desfaz; se você apagar tudo, o nome volta ao anterior. Aparece "Departamento atualizado com sucesso". Editar o nome exige o nível Administrar em Cadastros.
- **Membros** — A lista de quem está no departamento (nome e e-mail), com um × (_"Remover {nome} do departamento"_) para tirar cada pessoa. Para incluir alguém, use a busca "+ Adicionar atendente". Adicionar e remover membros é tarefa de administrador. Avisos da lista: _"Ninguém neste departamento ainda. Adicione quem atende por ele."_ quando não há ninguém; _"Todos já estão no departamento."_ quando todos já estão; _"Ninguém encontrado com esse nome."_ quando a busca não acha.
- **Distribuição de conversas** — Aparece só para quem tem o nível Administrar em Atendimento. Veja a seção "Distribuição de conversas".
- **Excluir departamento** — Botão no rodapé do painel (só com o nível Administrar em Cadastros).

**Tirar do departamento quem está na distribuição**

Se a pessoa faz parte da distribuição do departamento, o × não remove direto: abre _"Remover {nome} do departamento?"_ com o texto _"{nome} também sai da distribuição de conversas do departamento."_ Se ela era a única que recebia, a mensagem acrescenta _"Mais ninguém recebe por ela: as conversas novas do departamento ficam na fila sem atendente."_ Os botões são "Cancelar" e "Remover". A mesma confirmação aparece ao desmarcar o departamento no painel do membro (lá o título cita o nome do departamento; ver [Equipe e permissões](https://docs.convergefy.com.br/kb/equipe-permissoes.md)). Se o sistema recusar a saída, a tela avisa _"Antes de remover do departamento, tire a pessoa da distribuição de conversas dele."_

### Excluir um departamento

> **Excluir é permanente**
>
> Você exclui pela lixeira do card ou pelo botão "Excluir departamento" no painel. Aparece _"Excluir {nome}?"_:
>
> _"Os membros continuam na empresa. Não dá para desfazer."_ E, quando o departamento está na distribuição da empresa (e você tem acesso a ela): _"Os membros continuam na empresa. Ele também sai da distribuição da empresa. Não dá para desfazer."_ Os botões são "Cancelar" e "Excluir", e depois aparece "Departamento removido com sucesso".
>
> O que acontece com o resto:
>
> - As conversas e conexões que estavam no departamento **não são apagadas**: ficam sem departamento, e você precisará reatribuí-las.
> - Os vínculos dos membros com o departamento e as regras de distribuição dele **são apagados**.

### Onde os departamentos são usados

- **Transferir conversas** — No Chat, encaminhe uma conversa para um departamento.
- **Filtrar** — Filtre contatos e conversas por departamento.
- **Distribuir conversas** — Cada departamento pode ter a sua própria regra de distribuição, e a regra da empresa pode mandar conversas para um departamento (veja abaixo).
- **Nas automações** — O gatilho _"Atendimento transferido"_ e o passo _"Transferir atendimento"_ (ver [Automações](https://docs.convergefy.com.br/kb/automacoes.md)).

## Distribuição de conversas

A distribuição manda automaticamente cada conversa nova que chega sem atendente para alguém de uma lista, respeitando as porcentagens que você definir. Existem duas regras independentes, que podem trabalhar juntas:

- **A da empresa** vale para as conversas que chegam sem departamento. Pode ter atendentes e departamentos na lista.
- **A de cada departamento** vale para as conversas que estão naquele departamento. Só pode ter membros daquele departamento na lista.

Para configurar, é preciso o nível Administrar em **Atendimento** (veja [Equipe e permissões](https://docs.convergefy.com.br/kb/equipe-permissoes.md)). Quem não tem esse nível não vê a seção.

### Onde configurar

1. **Abrir as configurações** — Escolha de quem é a regra. Nos dois casos, a seção tem o interruptor "Distribuir conversas automaticamente".

   - Da empresa: no Chat, clique na engrenagem "Configurações de atendimento", ao lado do filtro da lista de conversas (ela não aparece na aba de grupos). A seção é "Para toda a empresa".
   - De um departamento: em Configurações → Departamentos, abra o departamento e vá na seção "Distribuição de conversas".
2. **Ligar** — O texto do interruptor explica: na empresa, _"Conversa que chega em Aguardando sem atendente vai para alguém da lista."_; no departamento, _"Conversa que chega neste departamento sem atendente vai para alguém da lista."_

   Se ninguém da lista tem porcentagem acima de 0% (lista vazia ou todos pausados), ligar abre o painel de configuração em vez de ligar. Monte a lista primeiro.
3. **Configurar** — Com a regra ligada aparece um resumo (por exemplo, _"Rodízio entre 3, 1 pausado"_ e _"12 conversas desde 24/10"_, ou _"Nenhuma conversa distribuída ainda"_) e o botão **"Configurar"**, que abre o painel "Distribuição de conversas" (_"Para quem vão as conversas que chegam sem atendente."_). No departamento, o painel se chama "Distribuição de {departamento}", com a seta de voltar.
4. **Salvar** — No painel, as mudanças só valem depois de **"Salvar"** (e "Descartar" volta ao que estava salvo). Antes de salvar, leia o aviso logo abaixo: salvar pode zerar a contagem. Salvar sempre deixa a regra ligada. Ligar e desligar o interruptor, ao contrário, grava na hora. Ao desligar, as conversas novas ficam na fila sem atendente.

> **Salvar pode zerar a contagem**
>
> A contagem de conversas recebidas por cada um, que o Rodízio usa para saber quem está abaixo da meta e que o relatório mostra, **zera** quando entra alguém novo na lista, quando uma porcentagem muda ou quando o modo muda. Nesses casos, antes de salvar, a tela avisa _"Salvar vai zerar a contagem de todos."_ Tirar alguém da lista, mudar a ordem ou ligar e desligar o interruptor não zera.

### O painel de configuração

- **Modo** — Como a regra escolhe a próxima pessoa. Em "Rodízio", cada um recebe na sua vez, na proporção das porcentagens (a tela chama de _"Round robin ponderado"_). Em "Sorteio", a escolha é aleatória, também pelas porcentagens. Os textos da tela estão logo abaixo.
- **Quem recebe** — A lista de atendentes (e, na regra da empresa, também departamentos), cada um com uma porcentagem num controle deslizante e um campo numérico. Quem entra começa com 0%. O × tira da lista. Lista vazia: _"Ninguém na lista ainda. Adicione quem vai receber as conversas."_
- **Adicionar à lista** — Use "+ Adicionar atendente ou departamento" (no departamento: "+ Adicionar atendente").
- **Porcentagens** — A soma precisa dar 100%. O painel mostra _"Total: 100%"_ ou _"Total: {N}%. Faltam {M}%."_, e só dá para salvar com o total fechado. "Dividir igualmente" reparte a mesma fatia entre todos.
- **Pausa com 0%** — Quem está com 0% fica pausado (a linha mostra "pausado"), sem sair da lista, e não recebe conversas. Para voltar a receber, dê uma porcentagem a ele.
- **Como foi dividido** — Um relatório com o que cada um recebeu contra a meta, desde o último zerar da contagem, por exemplo _"12 conversas distribuídas desde 24/10, às 09:30"_, ou _"Nenhuma conversa distribuída ainda. A divisão aparece aqui quando a primeira conversa chegar."_

**O que a tela diz sobre os modos e as porcentagens**

- "Rodízio": _"Round robin ponderado. Divide na proporção exata das porcentagens. A próxima conversa vai para quem está mais abaixo da meta."_
- "Sorteio": _"Aleatório ponderado. Cada conversa é sorteada pelas porcentagens, sem ordem previsível. Com o tempo fica perto da meta, mas não exato."_
- O painel explica a regra das porcentagens: _"A porcentagem é a fatia de cada um, e a soma precisa dar 100%. Aumentar alguém tira dos outros; diminuir deixa a diferença para você distribuir. Com 0% a pessoa fica pausada, sem sair da lista. A contagem zera quando entra alguém na lista, quando uma porcentagem muda ou quando o modo muda."_

**Como a conversa chega até a pessoa**

- **Quando a conversa entra na distribuição.** Em três situações, sempre sem atendente:

  - Na primeira mensagem da conversa, não quando ela é só aberta. Se essa primeira mensagem for enviada por um atendente, ele já fica com a conversa e nada é distribuído.
  - Quando ela entra em "Aguardando" sem atendente, vinda de outro status.
  - Quando é transferida para um departamento: passa pela regra dele. Se ele distribui, a pessoa já sai escolhida; se não, a conversa fica na fila do departamento. Devolver a conversa ao departamento em que ela já está não distribui de novo.

  Uma conversa que já tem atendente não é redistribuída.
- **Qual regra vale.** Conversa sem departamento usa a regra da empresa. Se a regra da empresa escolher um departamento, a conversa vai para ele e a regra desse departamento escolhe a pessoa. Conversa que já está num departamento usa a regra dele.
- **Departamento sem distribuição própria.** Se a empresa manda conversas para um departamento que não distribui, a conversa fica na fila dele, sem atendente. A tela avisa na lista da empresa: _"Sem distribuição própria: a conversa fica na fila do departamento, sem atendente."_ (com o atalho "Configurar distribuição") e, no resumo, _"{N} departamento(s) sem distribuição própria"_. Quando o departamento distribui, aparece _"Distribui entre {N} atendentes"_ (com "Ver distribuição").
- **Quem é pulado.** Quem está com 0% nunca é escolhido. Atendente sem acesso à conexão por onde a conversa chegou também é pulado (ver as conexões de cada membro em [Equipe e permissões](https://docs.convergefy.com.br/kb/equipe-permissoes.md)). Se ninguém puder receber, a conversa fica na fila sem atendente.
- **Quando o atendente é excluído.** Ele sai de todas as regras de distribuição, e as conversas que ele atendia voltam para "Aguardando" e passam pela distribuição.

> **Sair do painel com mudanças não salvas**
>
> Se você tem alterações e tenta voltar ou fechar o painel, aparece "Você tem mudanças não salvas" com o texto _"As mudanças na distribuição de conversas se perdem se você sair sem salvar."_ Escolha "Cancelar" (ficar), "Descartar e ir" ou "Salvar e ir" (este só fica disponível com o total em 100%).

## Erros e avisos esperados

Dois dos itens abaixo são só o aviso de lista vazia, não erros de fato.

- “Nenhuma tag cadastrada” — você ainda não tem nenhuma tag; é só o aviso de lista vazia. A tela mostra _"Crie sua primeira tag para classificar leads e conversas."_ Resolver: clique em “Nova tag” para criar a primeira (se você não vê o botão, peça o nível Administrar em Cadastros a um administrador).
- “Nenhuma tag encontrada” — a busca por nome não achou nenhuma tag com esse texto. Resolver: ajuste o termo da busca ou crie uma nova tag.
- “Erro ao carregar tags” — a plataforma não conseguiu listar as tags agora. Resolver: clique em “Tentar novamente”; se persistir, recarregue a página.
- “Nenhum departamento configurado” — você ainda não tem nenhum departamento; é só o aviso de lista vazia. A tela mostra _"Crie seu primeiro departamento para organizar a equipe e os atendimentos."_ Resolver: clique em “Novo departamento” para criar o primeiro.
- “Erro ao carregar departamentos” — a plataforma não conseguiu listar os departamentos agora. Resolver: clique em “Tentar novamente”; se persistir, recarregue a página.
- “Antes de remover do departamento, tire a pessoa da distribuição de conversas dele.” — a pessoa ainda recebe conversas pela regra do departamento. Resolver: abra a distribuição do departamento, tire a pessoa da lista e salve; depois remova do departamento.
