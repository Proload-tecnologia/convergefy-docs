# Funis e CRM: Negócios

Tudo o que se faz com os negócios (os cartões do Funil): criar, mover de etapa ou de funil, exportar e excluir os de uma coluna, e buscar, filtrar e abrir a conversa do contato.

Na Central de Ajuda: https://docs.convergefy.com.br/#/funis-negocios

## Em resumo

Um **negócio** é o cartão do funil: uma oportunidade de venda ligada a um contato. Esta página reúne o que se faz com ele: criar, mover de etapa ou de funil, exportar e excluir os de uma coluna, e buscar, filtrar e abrir a conversa. Criar, mover e excluir exigem **Operar** em Funis; ver, filtrar e exportar são de todos (a tabela de níveis está em [Funis e CRM](https://docs.convergefy.com.br/kb/funis.md)). Para finalizar um negócio como ganho, perda ou desqualificado, veja [Ganho, perda e desqualificado](https://docs.convergefy.com.br/kb/funis-desfechos.md).

Atenção: "Excluir negócios", no menu (⋮) da coluna, apaga os negócios de vez, sem lixeira e sem desfazer (veja "Excluir todos os negócios de uma coluna").

### Algo deu errado?

Procure o que você está vendo e siga a coluna da direita. O detalhe de cada caso está mais abaixo.

| O que você vê                                                                                                            | O que fazer                                                                                                                         |
| ------------------------------------------------------------------------------------------------------------------------ | ----------------------------------------------------------------------------------------------------------------------------------- |
| Não acho um negócio                                                                                                      | A busca só alcança os cartões já carregados (20 por vez, ao rolar). Role a coluna até o fim e confira a aba de status e os filtros. |
| "A coluna mudou enquanto você arrastava. Arraste o negócio de novo."                                                     | Solte o cartão de novo na posição desejada.                                                                                         |
| "Não foi possível mover o negócio."                                                                                      | Tente de novo e confirme que a etapa de destino ainda existe. Num arraste, o cartão volta sozinho à origem.                         |
| "Todos os atendimentos deste contato estão sendo conduzidos por outros atendentes. Você não tem acesso para abrir aqui." | Peça ao atendente responsável para liberar, ou abra por outro caminho.                                                              |
| "Novo Negócio" e o "+" da coluna não aparecem                                                                            | Falta o nível Operar em Funis. Peça a um Administrador.                                                                             |
| "Valor não pode ser negativo"                                                                                            | Informe zero ou mais no campo "Valor (R$)".                                                                                         |
| "Não foi possível carregar a conversa."                                                                                  | Tente de novo; se persistir, recarregue a página.                                                                                   |
| Nenhum negócio aparece na coluna                                                                                         | Confira a aba de status, a busca e os filtros (veja "Telas vazias").                                                                |

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
- **Produto e valor** — Com o nível Operar, clique no produto ou no valor para editar ali mesmo, sem abrir o formulário. Vale também para negócio finalizado. Como funciona: [Editar rápido pelo cartão do negócio](https://docs.convergefy.com.br/kb/produtos.md).
- **Tags** — As tags do contato numa linha; as que não cabem viram "+N". O "+ Tag" abre a lista para marcar ou criar tags.
- **Rodapé** — Em aberto: data de criação (dia/mês; o ano aparece ao passar o mouse: _"Criado em …"_) e avatar de quem criou. Sem pessoa (automação ou agente de IA), o ícone de Automação (_"Criado por Automação"_); se quem criou saiu da empresa, _"Criado por membro removido"_. Finalizado: faixa verde "Ganho", vermelha "Perda" ou cinza "Desqualificado", com a data de finalização (_"Finalizado em …"_). Em perda e desqualificado, o nome do contato fica em cinza.
- **Opções do negócio (⋮)** — Ao passar o mouse, só com Operar: "Ganho", "Perda", "Desqualificar", "Editar", "Mover negócio" e "Excluir". Em negócio finalizado, o desfecho atual aparece marcado e desativado, os outros dois servem para trocar de desfecho, e entra o item "Reabrir".

## Mover um negócio de etapa ou de funil

Arraste o cartão para outra coluna: o negócio muda de etapa na hora e para todos que veem o funil (ver [Tempo real](https://docs.convergefy.com.br/kb/tempo-real.md)). Para trocar de funil, use o menu "Opções do negócio" (⋮) → "Mover negócio". Negócio finalizado também se move e continua finalizado. A lista de destino não oferece as colunas de desfecho: para finalizar, use o menu do cartão ou a barra de ações.

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

## Buscar, filtrar e abrir a conversa

Abaixo do nome do funil ficam a busca "Buscar negócios...", as abas de status e um botão por filtro.

A busca compara nome e telefone do contato (não o título do negócio) e só alcança os cartões já carregados: a coluna carrega 20 negócios por vez, ao rolar. Em colunas longas, role até o fim antes de concluir que o negócio não existe.

As abas de status escolhem quais negócios o quadro mostra, cada uma com a quantidade:

- **Todos** — Abertos e finalizados.
- **Abertos** — Só os em andamento. É a aba padrão: depois, o funil volta na última aba que você escolheu nesta sessão do navegador. Cada coluna de desfecho vira um resumo tracejado (veja abaixo).
- **Ganhos** — Só os marcados como ganho.
- **Perdas** — Só os marcados como perda.
- **Desqualificados** — Só os marcados como desqualificados.

Na aba "Abertos", em vez dos cartões finalizados, cada coluna de desfecho mostra um resumo tracejado: a quantidade (_"{N} negócios"_), o aviso _"Solte aqui para marcar como ganho"_ (ou "perda", "desqualificado") e o link **"Ver na aba Ganhos"** (ou "Perdas", "Desqualificados"). Dá para soltar um cartão aberto direto nesse resumo para finalizá-lo, e o link leva à aba com os cartões.

A aba escolhida fica guardada para aquele funil enquanto a aba do navegador estiver aberta; depois, ele volta a abrir em "Abertos". Os números das abas seguem os filtros.

Cada filtro tem o seu botão, nesta ordem, e podem ser combinados:

- **Período** — Escolha a data que vale: "Criado em" ou "Finalizado em" (quando foi marcado como ganho, perda ou desqualificado). Depois, "Hoje", "Ontem", "7 dias", "30 dias" ou um intervalo no calendário. Com "Finalizado em", a aba "Abertos" fica zerada, pois negócio aberto não foi finalizado.
- **Criado por** — Um ou mais atendentes. No topo da lista fica "Automação", para negócios criados sem pessoa (automação ou agente de IA).
- **Tags** — Uma ou mais tags do contato: aparece o negócio cujo contato tem qualquer uma.
- **Origem** — De onde o contato veio pela última vez: Meta Ads, Google Ads, Outras origens ou Não rastreados. Uma por vez.

A escolha vale ao fechar o botão. Ligado, ele fica preenchido (desligado é tracejado) e mostra o que está escolhido (_"Período finalizados, 30 dias"_, _"Criado por Ana +2"_), com um "x" para limpar só aquele filtro. "Limpar filtros" desliga todos (a aba de status fica como está). Contadores e valores das colunas, o resumo e os números das abas contam só o que casa com os filtros.

Filtros e aba ficam no endereço da página: recarregar, voltar ou mandar o link a um colega abre o funil do mesmo jeito.

Clique num cartão para abrir a conversa do contato sem sair do CRM. Se o atendimento estiver com outra pessoa, aparece um aviso de acesso (ver [Atendimento / Chat](https://docs.convergefy.com.br/kb/chat.md)).

## Telas vazias

- **Nenhum negócio nesta coluna** (gray) — A etapa não tem cartões (aba "Todos"). Como resolver: adicione um negócio à coluna.
- **Nenhum negócio aberto nesta coluna** (gray) — Na aba "Abertos" não há negócio em andamento. Nas outras abas: _"Nenhum negócio ganho nesta coluna"_, _"Nenhum negócio perdido nesta coluna"_ e _"Nenhum negócio desqualificado nesta coluna"_. Como resolver: mude de aba para ver os finalizados.
- **Nenhum negócio com estes filtros** (gray) — A coluna tem negócios, mas nenhum casa com a busca ou os filtros. Como resolver: mude ou limpe os filtros e a busca.

## Avisos de confirmação

**Textos que aparecem quando dá certo**

- _"Negócio criado com sucesso"_, _"Negócio removido com sucesso"_.
- _"Negócio movido."_ (mesmo funil) e _"Negócio movido para o funil."_ (outro funil).

## Erros e avisos esperados

- “Valor não pode ser negativo” — valor inválido no negócio. Resolver: informe zero ou mais.
- “Remover negócio?” — confirmação ao excluir: _"O negócio "{título}" será removido permanentemente. Esta ação não pode ser desfeita."_ Resolver: confirme só se tiver certeza: é permanente.
- “Não foi possível mover o negócio.” — falha ao mover o negócio (arraste ou janela "Mover negócio"). Resolver: tente de novo e confirme que a etapa de destino ainda existe. Num arraste, o cartão volta sozinho à origem.
- “A coluna mudou enquanto você arrastava. Arraste o negócio de novo.” — outra pessoa alterou a coluna de destino durante o seu arraste. Resolver: solte o cartão de novo na posição desejada.
- “Todos os atendimentos deste contato estão sendo conduzidos por outros atendentes. Você não tem acesso para abrir aqui.” — o atendimento do contato está com outras pessoas. Resolver: peça ao atendente responsável para liberar, ou abra por outro caminho.
- “Não foi possível carregar a conversa.” — falha ao abrir a conversa pelo cartão (carregando, aparece um indicador girando). Resolver: tente de novo; se persistir, recarregue a página.
