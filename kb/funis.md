# Funis e CRM

O Funil é o quadro Kanban de vendas da empresa: colunas (etapas) lado a lado e cartões (negócios) que avançam até fechar. Mostra em que ponto está cada oportunidade.

Na Central de Ajuda: https://docs.convergefy.com.br/#/funis

## Em resumo

O **Funil** é o seu quadro de vendas no estilo Kanban (colunas lado a lado, cartões que avançam). As colunas são as **etapas** (ex.: _Contato_, _Qualificação_, _Proposta_). Cada **negócio** é um cartão ligado a um contato, com título, valor, produto e observações, que você arrasta de etapa em etapa. Uma empresa pode ter vários funis (ex.: _Vendas_, _SDR_, _Pós-Venda_).

No fim de todo funil ficam três colunas fixas, as **colunas de desfecho**: **"Ganho"**, **"Perda"** e **"Desqualificado"**. É para lá que o negócio vai quando é finalizado.

O funil também abre no celular e no tablet: veja [No celular e no tablet](https://docs.convergefy.com.br/kb/funis-celular.md).

Os negócios e os desfechos têm página própria: em [Negócios](https://docs.convergefy.com.br/kb/funis-negocios.md) ficam criar, mover, exportar, excluir em massa, buscar e filtrar; em [Ganho, perda e desqualificado](https://docs.convergefy.com.br/kb/funis-desfechos.md), finalizar, trocar o desfecho e reabrir.

### Algo deu errado?

Procure o que você está vendo e siga a coluna da direita. O detalhe de cada caso está mais abaixo.

| O que você vê                                                                                                           | O que fazer                                                                                              |
| ----------------------------------------------------------------------------------------------------------------------- | -------------------------------------------------------------------------------------------------------- |
| Um botão não aparece                                                                                                    | Falta o nível na área Funis (veja a tabela abaixo). Peça a um Administrador.                             |
| "Excluir" da coluna desativado                                                                                          | A coluna ainda tem cartão à vista. Esvazie a coluna, movendo ou removendo os cartões.                    |
| "Esta coluna tem {N} negócios finalizados. Mude para Todos e limpe os filtros para vê-los e movê-los antes de excluir." | Mude para a aba "Todos", limpe os filtros, mova ou exclua esses negócios e tente de novo.                |
| "O funil precisa de ao menos uma coluna."                                                                               | A última etapa não se exclui. Para sumir com o funil, exclua o funil inteiro.                            |
| "As colunas Ganho, Perda e Desqualificado são fixas."                                                                   | As colunas de desfecho não podem ser renomeadas, trocadas de cor, reordenadas nem excluídas.             |
| Um funil restrito não aparece na lista                                                                                  | Você não está na lista de membros dele. Quem administra o funil pode incluir você em "Membros do funil". |

### Primeiro uso

1. **Criar o funil** — Quem tem Administrar em Funis cria o funil e as etapas (veja "Criar um funil" e "Criar etapas (colunas)").
2. **Criar um negócio** — Quem tem Operar em Funis clica em "Novo Negócio" ou no "+" de uma coluna (veja "[Criar um negócio](https://docs.convergefy.com.br/kb/funis-negocios.md)").
3. **Mover o cartão** — Arraste o cartão de uma coluna para outra.
4. **Fechar o negócio** — Marque como "Ganho", "Perda" ou "Desqualificar". Se errar, dá para reabrir (veja "[Ganhar ou perder um negócio](https://docs.convergefy.com.br/kb/funis-desfechos.md)").

Você chega por **barra lateral → Funis**. Todos veem funis, etapas e negócios; o que cada pessoa faz depende do nível dela na área Funis (aba "Acesso" do membro, ver [Equipe e permissões](https://docs.convergefy.com.br/kb/equipe-permissoes.md)):

| O que você quer fazer                                                                                       | Nível necessário                         |
| ----------------------------------------------------------------------------------------------------------- | ---------------------------------------- |
| Ver o quadro, filtrar, abrir a conversa pelo cartão e usar "Exportar negócios"                              | **Ver** (todo membro)                    |
| "Novo Negócio" e o "+" da coluna, arrastar o cartão, o menu (⋮) do cartão, editar produto e valor no cartão | **Operar** em Funis                      |
| "Mover negócios", "Finalizar negócios" e "Excluir negócios" (menu da coluna)                                | **Operar** em Funis                      |
| "Novo Funil", renomear, reordenar e excluir funil, e "Membros do funil"                                     | **Administrar** em Funis (inclui Operar) |
| "Nova coluna", cor, nome, ordem e exclusão de etapa ("Excluir" da coluna)                                   | **Administrar** em Funis (inclui Operar) |
| "Disparar em massa" no menu da coluna                                                                       | **Operar** em Disparo em massa           |
| "+ Tag" no cartão                                                                                           | **Editar** em Contatos                   |

Sem o nível, o botão não aparece (e sem Operar o cartão não arrasta).

## Criar um funil

1. **Abrir o criador** — Exige Administrar em Funis. Clique em **"Criar primeiro funil"** (tela vazia) ou em **"Novo Funil"** (embaixo da lista). Também serve o item "Novo funil" do menu "Trocar de funil".
2. **Dar um nome** — No painel lateral "Novo funil", informe o "Nome do funil" (_"Ex.: Vendas, SDR, Pós-venda"_).
3. **Escolher quem vê (opcional)** — O interruptor "Todos os membros veem este funil" vem ligado (o padrão). Desligue para restringir: aparecem "Adicionar membro", "Selecionar todos" / "Desmarcar todos" e a contagem (_"1 membro marcado."_). Sem ninguém marcado, _"só os admins veem este funil"_.
4. **Confirmar** — Clique em **"Criar funil"**. Aparece "Funil criado." e o funil abre já com uma etapa chamada "Novo" (cinza). Se um membro marcado já saiu da empresa, ele é desmarcado e o aviso diz _"Um membro marcado não faz mais parte da empresa e foi desmarcado. Revise a lista e tente de novo."_

> **Funil restrito: o que a restrição esconde**
>
> A restrição vale só para a lista da tela de Funis: quem não está nela não vê o funil ali, mas ainda o abre pelo link e o encontra nas automações, no Chat e nas campanhas.
>
> Só o administrador da empresa vê todos os funis restritos; o nível Administrar em Funis não basta. Quem tem Administrar em Funis vê um cadeado nos funis restritos (dica: _"Visível só para os membros escolhidos"_).
>
> Para mudar depois: engrenagem do funil → "Membros do funil". Desligar a restrição não apaga a lista: ao religar, os mesmos membros voltam.

## Trocar, organizar e excluir funis

Os funis ficam na lista de funis, à esquerda do quadro (nomes longos aparecem cortados; passe o mouse para ver inteiro).

> **Excluir um funil leva junto etapas e negócios**
>
> A confirmação "Excluir funil?" conta o que será perdido: _"O funil {nome} será excluído com sua 1 etapa e nenhum negócio. Esta ação não pode ser desfeita."_ Com cartões, a frase traz o número de etapas e de negócios (enquanto carrega, diz _"…e todos os negócios dentro dele"_).
>
> Não há trava de "último funil": dá para excluir todos e ficar com a tela vazia.

- **Trocar de funil** — Clique na setinha ao lado do nome do funil aberto ("Trocar de funil").
- **Recolher a lista** — "Recolher lista de funis", no topo da lista, libera a tela para o quadro; para voltar, "Mostrar lista de funis", ao lado do nome do funil. A escolha é só sua.
- **Renomear** — Clique no nome do funil (ou no lápis, "Editar nome do funil") e digite. Exige Administrar.
- **Reordenar** — Com Administrar, arraste a alça que aparece à esquerda do funil ao passar o mouse. A ordem é salva sozinha e vale para toda a empresa.
- **Excluir** — Com Administrar, a lixeira que aparece sobre o funil na lista, ou o ícone "Excluir funil" no canto direito do cabeçalho.

## Exibição e resumo do funil

A engrenagem do cabeçalho ("Configurações do funil") reúne as opções de exibição e o resumo.

**Opções da engrenagem e resumo do funil**

- **Resumo do funil** — Liga e desliga a faixa de resumo abaixo dos filtros. _"A exibição fica salva só para você."_
- **Faixa da etapa nos cards** — Liga e desliga a faixa colorida à esquerda de cada cartão.
- **Ações ao arrastar** — Onde aparece a barra de ações ao arrastar um cartão: "Em cima" ou "Embaixo" (o padrão). Vale para todos os funis. Ver [Arrastar até a barra de ações](https://docs.convergefy.com.br/kb/funis-desfechos.md).
- **Membros do funil** — Quem vê este funil (ver "Criar um funil"). Só com Administrar em Funis.

O resumo conta os negócios do funil com os filtros ligados (ver [Buscar e filtrar](https://docs.convergefy.com.br/kb/funis-negocios.md)):

- **Entraram** — Quantos negócios entraram, com o período dos filtros (_"Criados · 30 dias"_, _"Finalizados · 01/10 a 27/10"_) ou "Todo o período".
- **Em aberto, Ganhos, Perdas e Desqualificados** — Quantidade, parte do total (%) e soma dos valores em reais.
- **Taxa de ganho** — Em gráfico de rosca (um anel), com um texto como _"16 de 33"_ (16 ganhos, numa base de 33 negócios): os ganhos sobre os negócios que entraram, sem contar os desqualificados. O ícone de ajuda ao lado, "Como a taxa de ganho é calculada", explica a conta.

Desqualificado não conta na base da taxa porque nunca teve chance de virar venda. Exemplo: entraram 33 negócios, 5 foram desqualificados e 14 foram ganhos. A base é 33 menos 5, ou 28, e a taxa é 14 de 28 (50%), o que a tela mostra como _"14 de 28"_.

Clicar num número leva à aba correspondente: "Entraram" abre "Todos"; os outros abrem "Abertos", "Ganhos", "Perdas" e "Desqualificados".

## Criar etapas (colunas)

Todas as ações de etapa exigem Administrar em Funis. Clique em **"Nova coluna"** (no cabeçalho ou no botão tracejado no fim do quadro; "Criar primeira etapa" se o funil não tiver nenhuma), informe o nome (ex.: _Contato, Qualificação, Proposta_), escolha uma cor se quiser e confirme em **"Criar coluna"**. A coluna nova entra sempre antes das colunas de desfecho.

O cabeçalho da coluna tem a cor (clique para trocar), o nome (clique para editar) e três botões: "+" (novo negócio nesta etapa), recolher e o menu (⋮). Embaixo ficam o valor total e a quantidade de negócios; com a busca ligada, contam só o que casou.

Se a etapa envia um evento de conversão ao anúncio, o cabeçalho mostra um ícone de mira ao lado da quantidade. Passe o mouse (ou toque) para ver o balão: o nome da coluna, _"Ao entrar nesta coluna, envia:"_ e uma linha por evento, com "Meta" ou "Google" e o nome do evento. Todo membro com acesso ao funil vê a mira; sem evento configurado, ela não aparece. Como configurar: [Configurar o rastreamento](https://docs.convergefy.com.br/kb/meta-ads-configurar.md).

### Colunas de desfecho

Todo funil tem, sempre no fim, três colunas fixas: **"Ganho"** (verde), **"Perda"** (vermelha) e **"Desqualificado"** (cinza). Elas guardam os negócios finalizados e não se editam: não dá para renomear, trocar a cor, reordenar nem excluir (_"As colunas Ganho, Perda e Desqualificado são fixas."_). Nelas não há "+" (novo negócio) nem "Finalizar negócios". A regra do funil precisar de ao menos uma coluna conta só as etapas comuns.

Funis antigos: negócios finalizados antes de as colunas de desfecho existirem continuam na etapa onde estavam, com a faixa "Ganho", "Perda" ou "Desqualificado" no cartão. Eles aparecem nas abas de status normalmente.

### Recolher colunas

**Como recolher e expandir colunas**

"Recolher coluna" deixa a coluna estreita (cor, quantidade e nome na vertical). Clique nela para abrir. As recolhidas ficam salvas por funil e só para você. À direita dos filtros, um atalho alterna entre "Recolher colunas vazias" (considerando aba, filtros e busca) e, com alguma recolhida, "Expandir todas as colunas".

### Ações da coluna

O menu (⋮), "Ações da coluna {nome}", reúne as ações sobre os negócios da etapa. Cada item só aparece com o nível da tabela do início; só "Exportar negócios" é de todos. Se uma ação em massa falhar, o aviso é _"Não foi possível excluir os negócios."_, _"Não foi possível mover os negócios."_ ou _"Não foi possível finalizar os negócios."_: tente de novo.

> **A aba e os filtros valem para as ações da coluna**
>
> "Exportar negócios", "Mover negócios", "Finalizar negócios" e "Excluir negócios" atingem só os negócios que aparecem com a aba de status e os filtros ligados (ver [Buscar e filtrar](https://docs.convergefy.com.br/kb/funis-negocios.md)). Na aba "Abertos", a de abertura do funil, os finalizados ficam de fora. A busca só limita o "Exportar negócios"; nas outras três ela não limita, e as janelas avisam.

> **Mover e finalizar em massa disparam as mesmas automações**
>
> "Mover negócios" e "Finalizar negócios" acionam, para cada negócio, as mesmas automações da ação em um negócio só. Mover também envia as mesmas conversões ao anúncio, se o [Rastreamento](https://docs.convergefy.com.br/kb/meta-ads.md) mapear a etapa de destino. As automações que enviam mensagem saem todas de uma vez, sem espaçamento: se quiser ritmo entre os envios, ponha um passo de espera na própria automação.

- **Disparar em massa** — Manda uma campanha para os negócios abertos da coluna inteira (numa coluna de desfecho, para os negócios dela), sem os filtros da tela (por isso fica disponível mesmo com a coluna aparentemente vazia). Ver [Disparo em massa](https://docs.convergefy.com.br/kb/disparo-em-massa.md).
- **Mover negócios** — Leva os negócios da coluna para outra etapa, deste ou de outro funil. A lista de destino não oferece as colunas de desfecho. Numa coluna comum, os negócios finalizados também vão e continuam finalizados. Numa coluna de desfecho, a janela traz a opção "Reabrir os negócios finalizados" (vem marcada): com ela, os negócios voltam a ficar em aberto na etapa de destino; sem ela, continuam finalizados.
- **Finalizar negócios** — Só em coluna comum. Abre "Finalizar negócios da coluna", que pergunta se os negócios em aberto da coluna viram ganho, perda ou desqualificado, com os botões "Marcar como ganho", "Marcar como perda" e "Desqualificar". Os que já estavam finalizados continuam como estão. Só nas abas "Abertos" e "Todos". Não pergunta o valor da venda (só o "Ganho" de um cartão pergunta).
- **Excluir negócios** — Apaga os negócios da coluna de uma vez (ver [Excluir todos os negócios de uma coluna](https://docs.convergefy.com.br/kb/funis-negocios.md)). Desativado se a coluna não tem negócio com a aba e os filtros atuais.
- **Excluir** — Remove a coluna. Desativado enquanto houver cartão à vista. As colunas de desfecho não têm esta opção.

### Mudar a ordem das etapas

O cabeçalho inteiro da coluna é a alça: arraste para a esquerda ou a direita. Clicar no nome, na cor ou no menu continua normal. A ordem é salva sozinha.

Só as etapas comuns mudam de lugar: as colunas de desfecho ficam paradas no fim.

Com mais colunas do que cabem na tela, arraste até a borda e o quadro rola sozinho. Sem arrastar, o mesmo vale com o mouse parado numa borda (faixa de uns 60 px): o quadro rola para aquele lado, mais depressa quanto mais perto da borda, com uma seta ‹ ou ›. Só com mouse, não com toque.

> **Quando não dá para excluir uma etapa**
>
> Uma etapa só é excluída quando não tem nenhum negócio, nem aberto nem finalizado. Na prática, são três casos:
>
> - **Há cartões à vista na coluna:** "Excluir" fica desativado. Mova ou remova os cartões antes.
> - **A coluna parece vazia, mas não está:** a busca, os filtros ou a aba "Abertos" escondem negócios. A exclusão é recusada e a mensagem diz o que fazer (_"Esta coluna tem {N} negócios finalizados. Mude para Todos…"_ ou _"Só dá para excluir uma coluna sem negócios. Limpe a busca e os filtros…"_).
> - **É a última etapa do funil:** a exclusão é recusada mesmo com a coluna vazia (_"O funil precisa de ao menos uma coluna."_). Para se livrar dela, exclua o funil inteiro.

A confirmação de excluir etapa pergunta _"Deseja remover a coluna {nome}?"_. Confirme em "Remover" ou desista em "Cancelar".

## Telas vazias

- **Nenhum funil ainda** (gray) — _"Crie seu primeiro funil para começar a gerenciar seus negócios"_ (sem Administrar: _"Os funis criados na empresa aparecem aqui"_). Como resolver: crie seu primeiro funil.
- **Nenhuma etapa ainda** (gray) — _"Crie sua primeira etapa para começar a organizar negócios"_ (sem Administrar: _"As etapas deste funil aparecem aqui"_). Como resolver: crie a primeira etapa.

## Avisos de confirmação

**Textos que aparecem quando dá certo**

- _"Funil criado."_, _"Coluna criada com sucesso"_, _"Coluna removida com sucesso"_.
- Ações em massa da coluna, que rodam em segundo plano: _"Movendo {N} negócios."_, _"Marcando {N} negócios como ganhos."_ (ou _"como perda"_, _"como desqualificados"_) e _"{N} negócios excluídos."_ Se nada se aplica: _"Nenhum negócio desta coluna pode ir para o destino."_ ou _"Nenhum negócio em aberto nesta coluna."_

## Erros e avisos esperados

- “Não foi possível criar o funil.” — falha ao criar o funil. Resolver: confira a internet e tente de novo.
- “Não foi possível criar a coluna.” — falha ao criar a etapa. Resolver: tente de novo.
- “Não foi possível reordenar os funis.” — falha ao salvar a ordem dos funis. Resolver: arraste de novo; a lista volta à ordem anterior.
- “O funil precisa de ao menos uma coluna.” — você tentou excluir a última etapa do funil. Resolver: para sumir com o funil, exclua o funil inteiro.
- “Só dá para excluir uma coluna sem negócios. Limpe a busca e os filtros para ver os negócios dela.” — a coluna tem negócios escondidos pela busca ou pelos filtros. Resolver: limpe a busca e os filtros, mova ou exclua os negócios e tente de novo.
- “Não foi possível remover a coluna.” — falha geral ao excluir a etapa. Resolver: tente de novo; se persistir, recarregue a página.
- “Esta coluna tem {N} negócios finalizados. Mude para Todos e limpe os filtros para vê-los e movê-los antes de excluir.” — a coluna só tem negócios finalizados, escondidos pela aba Abertos. Resolver: mude para a aba Todos, limpe os filtros, mova ou exclua esses negócios e tente de novo.
- “Não foi possível reordenar as colunas.” — falha ao salvar a nova ordem das etapas. Resolver: arraste de novo; a ordem anterior volta sozinha.
- “As colunas Ganho, Perda e Desqualificado são fixas.” — você tentou alterar uma coluna de desfecho. Resolver: as colunas de desfecho não se renomeiam, não mudam de cor, não se reordenam e não se excluem. Use as etapas comuns para organizar o funil.
