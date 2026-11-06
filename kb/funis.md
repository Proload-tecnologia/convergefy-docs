# Funis e CRM

O Funil é o quadro Kanban de vendas da empresa: colunas (etapas) lado a lado e cartões (negócios) que avançam até fechar. Mostra em que ponto está cada oportunidade.

Na Central de Ajuda: https://docs.convergefy.com.br/#/funis

## Em resumo

O **Funil** é o seu quadro de vendas no estilo Kanban (colunas lado a lado, cartões que avançam). As colunas são as **etapas** (ex.: _Contato_, _Qualificação_, _Proposta_). Cada **negócio** é um cartão ligado a um contato, com título, valor, produto e observações, que você arrasta de etapa em etapa. Uma empresa pode ter vários funis (ex.: _Vendas_, _SDR_, _Pós-Venda_).

### Algo deu errado?

Procure o que você está vendo e siga a coluna da direita. O detalhe de cada caso está mais abaixo.

| O que você vê                                                                                                            | O que fazer                                                                                                                         |
| ------------------------------------------------------------------------------------------------------------------------ | ----------------------------------------------------------------------------------------------------------------------------------- |
| "Abra no desktop"                                                                                                        | O quadro só abre em tela grande. Use um computador ou aumente a janela.                                                             |
| Um botão não aparece                                                                                                     | Falta o nível na área Funis (veja a tabela abaixo). Peça a um Administrador.                                                        |
| Não acho um negócio                                                                                                      | A busca só alcança os cartões já carregados (20 por vez, ao rolar). Role a coluna até o fim e confira a aba de status e os filtros. |
| "Excluir" da coluna desativado                                                                                           | A coluna ainda tem cartão à vista. Esvazie a coluna, movendo ou removendo os cartões.                                               |
| "Esta coluna tem {N} negócios finalizados. Mude para Todos e limpe os filtros para vê-los e movê-los antes de excluir."  | Mude para a aba "Todos", limpe os filtros, mova ou exclua esses negócios e tente de novo.                                           |
| "O funil precisa de ao menos uma coluna."                                                                                | A última etapa não se exclui. Para sumir com o funil, exclua o funil inteiro.                                                       |
| "Este negócio já foi finalizado."                                                                                        | Atualize o quadro: alguém já o marcou como Ganho ou Perda.                                                                          |
| "Negócio ganho ou perdido não pode ser editado."                                                                         | Negócio finalizado só pode ser movido ou excluído.                                                                                  |
| "A coluna mudou enquanto você arrastava. Arraste o negócio de novo."                                                     | Solte o cartão de novo na posição desejada.                                                                                         |
| "Não foi possível mover o negócio."                                                                                      | Tente de novo e confirme que a etapa de destino ainda existe. Num arraste, o cartão volta sozinho à origem.                         |
| "Todos os atendimentos deste contato estão sendo conduzidos por outros atendentes. Você não tem acesso para abrir aqui." | Peça ao atendente responsável para liberar, ou abra por outro caminho.                                                              |
| Um funil restrito não aparece na lista                                                                                   | Você não está na lista de membros dele. Quem administra o funil pode incluir você em "Membros do funil".                            |

### Primeiro uso

1. **Criar o funil** — Quem tem Administrar em Funis cria o funil e as etapas (veja "Criar um funil" e "Criar etapas (colunas)").
2. **Criar um negócio** — Quem tem Operar em Funis clica em "Novo Negócio" ou no "+" de uma coluna (veja "Criar um negócio").
3. **Mover o cartão** — Arraste o cartão de uma coluna para outra.
4. **Fechar o negócio** — Marque como Ganho ou Perda. Atenção: isso não tem volta (veja "Ganhar ou perder um negócio").

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

> **O Funil só abre em tela grande**
>
> Em telas estreitas (celular e janelas pequenas) o quadro não aparece. A tela mostra "Abra no desktop" e _"O funil requer uma tela maior para funcionar corretamente."_ _Por quê:_ arrastar cartões e colunas não cabe no celular. Use um computador ou aumente a janela.

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
- **Ações ao arrastar** — Onde aparece a barra de ações ao arrastar um cartão: "Em cima" ou "Embaixo" (o padrão). Vale para todos os funis. Ver [Arrastar até a barra de ações](https://docs.convergefy.com.br/kb/funis.md).
- **Membros do funil** — Quem vê este funil (ver "Criar um funil"). Só com Administrar em Funis.

O resumo conta os negócios do funil com os filtros ligados (ver [Buscar e filtrar](https://docs.convergefy.com.br/kb/funis.md)):

- **Entraram** — Quantos negócios entraram, com o período dos filtros (_"Criados · 30 dias"_, _"Finalizados · 01/10 a 27/10"_) ou "Todo o período".
- **Em aberto, Ganhos e Perdas** — Quantidade, parte do total (%) e soma dos valores em reais.
- **Taxa de ganho** — Ganhos sobre tudo o que entrou (abertos, ganhos e perdidos), em gráfico de rosca (um anel): _"14 de 31 que entraram"_.

Clicar num número leva à aba correspondente: "Entraram" abre "Todos"; os outros abrem "Abertos", "Ganhos" e "Perdas".

## Criar etapas (colunas)

Todas as ações de etapa exigem Administrar em Funis. Clique em **"Nova coluna"** (no cabeçalho ou depois da última coluna; "Criar primeira etapa" se o funil não tiver nenhuma), informe o nome (ex.: _Contato, Qualificação, Proposta_), escolha uma cor se quiser e confirme em **"Criar coluna"**.

O cabeçalho da coluna tem a cor (clique para trocar), o nome (clique para editar) e três botões: "+" (novo negócio nesta etapa), recolher e o menu (⋮). Embaixo ficam o valor total e a quantidade de negócios; com a busca ligada, contam só o que casou.

### Recolher colunas

**Como recolher e expandir colunas**

"Recolher coluna" deixa a coluna estreita (cor, quantidade e nome na vertical). Clique nela para abrir. As recolhidas ficam salvas por funil e só para você. À direita dos filtros, um atalho alterna entre "Recolher colunas vazias" (considerando aba, filtros e busca) e, com alguma recolhida, "Expandir todas as colunas".

### Ações da coluna

O menu (⋮), "Ações da coluna {nome}", reúne as ações sobre os negócios da etapa. Cada item só aparece com o nível da tabela do início; só "Exportar negócios" é de todos. Se uma ação em massa falhar, o aviso é _"Não foi possível excluir os negócios."_, _"Não foi possível mover os negócios."_ ou _"Não foi possível finalizar os negócios."_: tente de novo.

> **A aba e os filtros valem para as ações da coluna**
>
> "Exportar negócios", "Mover negócios", "Finalizar negócios" e "Excluir negócios" atingem só os negócios que aparecem com a aba de status e os filtros ligados (ver [Buscar e filtrar](https://docs.convergefy.com.br/kb/funis.md)). Na aba "Abertos", a de abertura do funil, ganhos e perdidos ficam de fora. A busca só limita o "Exportar negócios"; nas outras três ela não limita, e as janelas avisam.

> **Mover e finalizar em massa disparam as mesmas automações**
>
> "Mover negócios" e "Finalizar negócios" acionam, para cada negócio, as mesmas automações da ação em um negócio só. Mover também envia as mesmas conversões ao anúncio, se o [Rastreamento](https://docs.convergefy.com.br/kb/meta-ads.md) mapear a etapa de destino. As automações que enviam mensagem saem todas de uma vez, sem espaçamento: se quiser ritmo entre os envios, ponha um passo de espera na própria automação.

- **Disparar em massa** — Manda uma campanha para os negócios abertos da coluna inteira, sem os filtros da tela (por isso fica disponível mesmo com a coluna aparentemente vazia). Ver [Disparo em massa](https://docs.convergefy.com.br/kb/disparo-em-massa.md).
- **Mover negócios** — Leva os negócios da coluna para outra etapa, deste ou de outro funil. Os finalizados também vão e continuam Ganho ou Perda.
- **Finalizar negócios** — Marca os negócios abertos como ganhos ("Marcar como ganhos") ou perdidos ("Marcar como perdidos"). Só nas abas "Abertos" e "Todos". Não pergunta o valor da venda (só o "Ganho" de um cartão pergunta).
- **Excluir negócios** — Apaga os negócios da coluna de uma vez (abaixo). Desativado se a coluna não tem negócio com a aba e os filtros atuais.
- **Excluir** — Remove a coluna. Desativado enquanto houver cartão à vista.

### Mudar a ordem das etapas

O cabeçalho inteiro da coluna é a alça: arraste para a esquerda ou a direita. Clicar no nome, na cor ou no menu continua normal. A ordem é salva sozinha.

Com mais colunas do que cabem na tela, arraste até a borda e o quadro rola sozinho. Sem arrastar, o mesmo vale com o mouse parado numa borda (faixa de uns 60 px): o quadro rola para aquele lado, mais depressa quanto mais perto da borda, com uma seta ‹ ou ›. Só com mouse, não com toque.

> **Quando não dá para excluir uma etapa**
>
> Uma etapa só é excluída quando não tem nenhum negócio, nem aberto nem finalizado. Na prática, são três casos:
>
> - **Há cartões à vista na coluna:** "Excluir" fica desativado. Mova ou remova os cartões antes.
> - **A coluna parece vazia, mas não está:** a busca, os filtros ou a aba "Abertos" escondem negócios. A exclusão é recusada e a mensagem diz o que fazer (_"Esta coluna tem {N} negócios finalizados. Mude para Todos…"_ ou _"Só dá para excluir uma coluna sem negócios. Limpe a busca e os filtros…"_).
> - **É a última etapa do funil:** a exclusão é recusada mesmo com a coluna vazia (_"O funil precisa de ao menos uma coluna."_). Para se livrar dela, exclua o funil inteiro.

A confirmação de excluir etapa pergunta _"Deseja remover a coluna {nome}?"_. Confirme em "Remover" ou desista em "Cancelar".

## Criar um negócio

1. **Abrir o criador de negócio** — Exige Operar em Funis. Clique em **"Novo Negócio"** (cabeçalho) ou no **"+"** de uma coluna: abre o painel lateral "Novo negócio" (ao editar, "Editar negócio"). Pelo "+", o negócio já nasce naquela etapa. Pelo "Novo Negócio", o campo "Etapa" vem com a primeira do funil (dá para trocar).
2. **Preencher os dados** — * **Lead \*** — Obrigatório. Selecione o cliente (_"Buscar lead pelo nome ou telefone..."_). A tela diz "lead", que é o mesmo que contato. Se o negócio nasce de uma conversa, o contato já vem preenchido. Ao editar, vira só leitura e se chama "Contato".
   * **Observações** — Anotações livres (_"Anotações sobre este negócio..."_).
   * **Produto cadastrado** — Escolhe um produto cadastrado e copia nome e valor para os campos abaixo, que seguem editáveis (ver [Produtos](https://docs.convergefy.com.br/kb/produtos.md)).
   * **Nome do produto** — _"Ex: Plano Mensal"_. Texto livre.
   * **Valor (R$)** — O valor em reais (_0,00_). Dá para ajustar depois no cartão; ao marcar Ganho, ele é confirmado de novo.
3. **Confirmar** — Clique em **"Criar negócio"** (ou "Salvar", ao editar).

**O que o cartão do negócio mostra**

Todo cartão tem as mesmas quatro linhas. A faixa colorida à esquerda é a cor da etapa.

- **Contato** — Avatar e nome do contato (ou o título, se não tiver nome). Contato vindo de anúncio leva o selo da origem (Meta, Google ou outra) no avatar e, se veio por formulário de anúncio, a etiqueta "Form" antes do nome.
- **Produto e valor** — Com o negócio em aberto e o nível Operar, clique no produto ou no valor para editar ali mesmo, sem abrir o formulário. Como funciona: [Editar rápido pelo cartão do negócio](https://docs.convergefy.com.br/kb/produtos.md).
- **Tags** — As tags do contato numa linha; as que não cabem viram "+N". O "+ Tag" abre a lista para marcar ou criar tags.
- **Rodapé** — Em aberto: data de criação (dia/mês; o ano aparece ao passar o mouse: _"Criado em …"_) e avatar de quem criou. Sem pessoa (automação ou agente de IA), o ícone de Automação (_"Criado por Automação"_); se quem criou saiu da empresa, _"Criado por membro removido"_. Ganho ou perdido: faixa verde "Ganho" ou vermelha "Perda" com a data de finalização (_"Finalizado em …"_).
- **Opções do negócio (⋮)** — Ao passar o mouse, só com Operar: "Ganho", "Perda", "Editar", "Mover negócio", "Excluir". Em negócio finalizado, só os dois últimos.

## Mover um negócio de etapa ou de funil

Arraste o cartão para outra coluna: o negócio muda de etapa na hora e para todos que veem o funil (ver [Tempo real](https://docs.convergefy.com.br/kb/tempo-real.md)). Para trocar de funil, use o menu "Opções do negócio" (⋮) → "Mover negócio". Negócio finalizado também se move e continua Ganho ou Perda.

> **Mover pode disparar automações e conversões**
>
> Ao cair na etapa de destino (ou ser criado nela), o negócio pode iniciar automações ligadas a ela e enviar um evento de conversão ao anúncio, se o [Rastreamento](https://docs.convergefy.com.br/kb/meta-ads.md) mapear essa etapa.

1. **Abrir** — Abre a janela "Mover negócio" (_"Escolha o funil e a etapa de destino."_).
2. **Escolher funil e etapa** — "Funil" e "Etapa" ficam lado a lado. O funil e a etapa de agora continuam na lista com o selo "Atual" (a etapa atual não pode ser escolhida). Um resumo embaixo mostra de onde sai e para onde vai. Com seis funis ou mais, aparece a busca "Buscar funil...".
3. **Confirmar** — Clique em **"Mover"** (mostra _"Movendo..."_) ou desista em "Cancelar".

> **Dá para mover sem sair da conversa**
>
> No [Chat](https://docs.convergefy.com.br/kb/chat.md), a seção "Negócios" do painel do contato tem "Avançar para ‹próxima etapa›", que move o negócio na hora (a seta volta uma etapa). Na última etapa, vira "Concluir como Ganho". No computador, clicar na trilha de etapas move direto para a etapa clicada.

## Exportar os negócios de uma coluna

No menu (⋮) da coluna, **"Exportar negócios"** abre "Exportar negócios de {nome da coluna}", onde você escolhe o que entra no arquivo: Negócio, Contato, Origem do contato e Campos personalizados do contato. Tudo vem marcado, e a escolha fica lembrada.

O arquivo sai em CSV, gerado no seu computador: _"Você pode continuar usando o sistema, mas fechar a aba recomeça a exportação do zero."_ Enquanto roda, o item do menu vira "Exportando N%". No fim aparece _"{N} negócios exportados."_, com "Baixar novamente". Com a busca ligada, sai só o que casa com ela, inclusive o que a coluna ainda não carregou.

## Excluir todos os negócios de uma coluna

> **Isso não tem desfazer**
>
> Os negócios são apagados de vez, sem lixeira. Os contatos não são tocados e a coluna continua, vazia.

No menu (⋮) da coluna, **"Excluir negócios"** apaga os cartões de uma vez. A janela "Excluir negócios da coluna" diz _"Excluir os {N} negócios da coluna {nome}? Esta ação não pode ser desfeita."_ (na aba "Abertos": _"Excluir os {N} negócios abertos da coluna…"_).

## Ganhar ou perder um negócio

> **Ganho e Perda são irreversíveis**
>
> Marcar Ganho ou Perda fecha o negócio para o histórico de resultados e não pode ser desfeito: ele não volta a ficar em aberto. Confira o produto antes e o valor em "Valor da venda", a última chance de acertá-lo.
>
> Depois de fechado:
>
> - **não dá mais para editar** título, notas, produto, valor e responsável, nem marcar outro desfecho;
> - **continua possível** mover o negócio de etapa ou de funil ("Mover negócio") e excluí-lo ("Excluir");
> - ele sai da aba "Abertos" e passa a aparecer em "Ganhos" ou "Perdas".
>
> _Por quê:_ esses números alimentam o histórico de vendas, e editá-los depois de fechado corromperia o resultado.

Você fecha uma oportunidade pelo menu "Opções do negócio" (⋮) ou arrastando o cartão até a barra de ações (ver abaixo). Os dois caminhos abrem a mesma confirmação:

- **Ganho** — Abre "Marcar como Ganho?" (_"Depois de marcado, o negócio não volta a ficar em aberto."_) com o campo "Valor da venda", preenchido com o valor atual e opcional: _"Confira o valor fechado. Ele entra no total do funil e do contato."_ Em branco, o valor não muda. Confirme em **"Marcar como Ganho"**. O rodapé vira a faixa verde "Ganho".
- **Perda** — Abre "Marcar como Perda?" com o mesmo aviso, sem valor. Confirme em **"Marcar como Perda"**. O rodapé vira a faixa vermelha "Perda".

Marcar também pode iniciar automações de negócio finalizado.

### Arrastar até a barra de ações

1. **Segurar o cartão** — Segure um cartão em aberto e comece a arrastar. Aparece uma barra de ações. Ela tem, numa caixa, "Ganho" (_"Marcar como ganho"_) e "Perda" (_"Marcar como perda"_). Soltos dos lados ficam dois círculos só com ícone: o X à esquerda e a lixeira à direita. Com o cartão em cima, eles dizem _"Solte para cancelar"_ e _"Solte para excluir"_.
2. **Soltar no destino** — Leve o cartão até um destino: ele ganha borda contínua e a cor dele (verde no Ganho, vermelho na Perda e na lixeira), e o cartão encolhe junto do ponteiro. Solte ali.
3. **Confirmar** — Abre a mesma janela do menu: "Marcar como Ganho?" (com o "Valor da venda"), "Marcar como Perda?" ou, na lixeira, "Remover negócio?". Em "Cancelar", o cartão continua aberto na etapa onde estava. Solto no X, não abre janela: o arraste é desfeito e o cartão volta para onde estava.

A barra fica rente à base das colunas; em "Ações ao arrastar" (engrenagem) dá para pôr "Em cima".

**Quando a barra não aparece**

- Cartão já finalizado (abas "Ganhos" e "Perdas"): não tem mais desfecho a marcar.
- Arraste de coluna: a barra é só para cartões.
- Sem Operar em Funis: o cartão nem arrasta.

Soltar fora da barra continua movendo o negócio entre etapas. Esc no meio do arraste cancela tudo e a barra some.

## Buscar, filtrar e abrir a conversa

Abaixo do nome do funil ficam a busca "Buscar negócios...", as abas de status e um botão por filtro.

A busca compara nome e telefone do contato (não o título do negócio) e só alcança os cartões já carregados: a coluna carrega 20 negócios por vez, ao rolar. Em colunas longas, role até o fim antes de concluir que o negócio não existe.

As abas de status escolhem quais negócios o quadro mostra, cada uma com a quantidade:

- **Todos** — Abertos e finalizados.
- **Abertos** — Só os em andamento. É a aba em que o funil abre: ganhos e perdidos continuam nas colunas, mas saem da frente.
- **Ganhos** — Só os marcados como ganho.
- **Perdas** — Só os marcados como perda.

A aba escolhida fica guardada para aquele funil enquanto a aba do navegador estiver aberta; depois, ele volta a abrir em "Abertos". Os números das abas seguem os filtros.

Cada filtro tem o seu botão, nesta ordem, e podem ser combinados:

- **Período** — Escolha a data que vale: "Criado em" ou "Finalizado em" (quando virou ganho ou perdido). Depois, "Hoje", "Ontem", "7 dias", "30 dias" ou um intervalo no calendário. Com "Finalizado em", a aba "Abertos" fica zerada, pois negócio aberto não foi finalizado.
- **Criado por** — Um ou mais atendentes. No topo da lista fica "Automação", para negócios criados sem pessoa (automação ou agente de IA).
- **Tags** — Uma ou mais tags do contato: aparece o negócio cujo contato tem qualquer uma.
- **Origem** — De onde o contato veio pela última vez: Meta Ads, Google Ads, Outras origens ou Não rastreados. Uma por vez.

A escolha vale ao fechar o botão. Ligado, ele fica preenchido (desligado é tracejado) e mostra o que está escolhido (_"Período finalizados, 30 dias"_, _"Criado por Ana +2"_), com um "x" para limpar só aquele filtro. "Limpar filtros" desliga todos (a aba de status fica como está). Contadores e valores das colunas, o resumo e os números das abas contam só o que casa com os filtros.

Filtros e aba ficam no endereço da página: recarregar, voltar ou mandar o link a um colega abre o funil do mesmo jeito.

Clique num cartão para abrir a conversa do contato sem sair do CRM. Se o atendimento estiver com outra pessoa, aparece um aviso de acesso (ver [Atendimento / Chat](https://docs.convergefy.com.br/kb/chat.md)).

## Telas vazias

- **Nenhum funil ainda** (gray) — _"Crie seu primeiro funil para começar a gerenciar seus negócios"_ (sem Administrar: _"Os funis criados na empresa aparecem aqui"_). Como resolver: crie seu primeiro funil.
- **Nenhuma etapa ainda** (gray) — _"Crie sua primeira etapa para começar a organizar negócios"_ (sem Administrar: _"As etapas deste funil aparecem aqui"_). Como resolver: crie a primeira etapa.
- **Nenhum negócio nesta coluna** (gray) — A etapa não tem cartões (aba "Todos"). Como resolver: adicione um negócio à coluna.
- **Nenhum negócio aberto nesta coluna** (gray) — Na aba "Abertos" não há negócio em andamento. Nas outras abas: _"Nenhum negócio ganho nesta coluna"_ e _"Nenhum negócio perdido nesta coluna"_. Como resolver: mude de aba para ver os ganhos e perdidos.
- **Nenhum negócio com estes filtros** (gray) — A coluna tem negócios, mas nenhum casa com a busca ou os filtros. Como resolver: mude ou limpe os filtros e a busca.

## Avisos de confirmação

**Textos que aparecem quando dá certo**

- _"Funil criado."_, _"Coluna criada com sucesso"_, _"Coluna removida com sucesso"_, _"Negócio criado com sucesso"_, _"Negócio removido com sucesso"_.
- _"Negócio movido."_ (mesmo funil) e _"Negócio movido para o funil."_ (outro funil).
- Ações em massa da coluna, que rodam em segundo plano: _"Movendo {N} negócios."_, _"Marcando {N} negócios como ganhos."_ (ou _"perdidos"_) e _"{N} negócios excluídos."_ Se nada se aplica: _"Nenhum negócio desta coluna pode ir para o destino."_ ou _"Nenhum negócio em aberto nesta coluna."_

## Erros e avisos esperados

- “Não foi possível criar o funil.” — falha ao criar o funil. Resolver: confira a internet e tente de novo.
- “Não foi possível criar a coluna.” — falha ao criar a etapa. Resolver: tente de novo.
- “Não foi possível reordenar os funis.” — falha ao salvar a ordem dos funis. Resolver: arraste de novo; a lista volta à ordem anterior.
- “O funil precisa de ao menos uma coluna.” — você tentou excluir a última etapa do funil. Resolver: para sumir com o funil, exclua o funil inteiro.
- “Só dá para excluir uma coluna sem negócios. Limpe a busca e os filtros para ver os negócios dela.” — a coluna tem negócios escondidos pela busca ou pelos filtros. Resolver: limpe a busca e os filtros, mova ou exclua os negócios e tente de novo.
- “Não foi possível remover a coluna.” — falha geral ao excluir a etapa. Resolver: tente de novo; se persistir, recarregue a página.
- “Esta coluna tem {N} negócios finalizados. Mude para Todos e limpe os filtros para vê-los e movê-los antes de excluir.” — a coluna só tem ganhos ou perdas, escondidos pela aba Abertos. Resolver: mude para a aba Todos, limpe os filtros, mova ou exclua esses negócios e tente de novo.
- “Valor não pode ser negativo” — valor inválido no negócio. Resolver: informe zero ou mais.
- “Remover negócio?” — confirmação ao excluir: _"O negócio "{título}" será removido permanentemente. Esta ação não pode ser desfeita."_ Resolver: confirme só se tiver certeza: é permanente.
- “Não foi possível mover o negócio.” — falha ao mover o negócio (arraste ou janela "Mover negócio"). Resolver: tente de novo e confirme que a etapa de destino ainda existe. Num arraste, o cartão volta sozinho à origem.
- “A coluna mudou enquanto você arrastava. Arraste o negócio de novo.” — outra pessoa alterou a coluna de destino durante o seu arraste. Resolver: solte o cartão de novo na posição desejada.
- “Não foi possível reordenar as colunas.” — falha ao salvar a nova ordem das etapas. Resolver: arraste de novo; a ordem anterior volta sozinha.
- “Este negócio já foi finalizado.” — você tentou finalizar um negócio já finalizado. Resolver: atualize o quadro: alguém já o marcou como Ganho ou Perda.
- “Não foi possível finalizar o negócio.” — falha ao marcar o negócio como Ganho ou Perda. Resolver: tente de novo; se persistir, recarregue a página.
- “Negócio ganho ou perdido não pode ser editado.” — você tentou mudar produto ou valor de um negócio já marcado como Ganho ou Perda. Resolver: negócio finalizado só pode ser movido ou excluído.
- “Todos os atendimentos deste contato estão sendo conduzidos por outros atendentes. Você não tem acesso para abrir aqui.” — o atendimento do contato está com outras pessoas. Resolver: peça ao atendente responsável para liberar, ou abra por outro caminho.
- “Não foi possível carregar a conversa.” — falha ao abrir a conversa pelo cartão (carregando, aparece um indicador girando). Resolver: tente de novo; se persistir, recarregue a página.
