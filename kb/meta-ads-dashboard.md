# Rastreamento: Dashboard

O resumo do período no Rastreamento: quanto você investiu em anúncios, quantos contatos chegaram, quantos negócios viraram venda e quanto cada campanha rendeu.

Na Central de Ajuda: https://docs.convergefy.com.br/#/meta-ads-dashboard

## Em resumo

O Dashboard junta, num período escolhido, o que veio dos anúncios e o que aconteceu no seu funil de vendas. Ele tem dois formatos:

- **Com anúncios**: quando a Meta ou o Google Ads estão conectados em "Contas de Anúncio". Mostra o investimento, o retorno e uma aba para cada plataforma conectada.
- **Só CRM**: sem nenhuma das duas conectadas. Mostra só os negócios e as vendas, e uma aba "Campanhas" que convida a conectar.

Os números vêm do histórico do seu funil e das plataformas de anúncio. O que cada um conta está em [Como os números são contados](https://docs.convergefy.com.br/kb/meta-ads-dashboard.md).

### Algo deu errado?

Procure o que você está vendo e siga a coluna da direita. O detalhe de cada caso está mais abaixo.

| O que você vê                                                                 | O que fazer                                                                                                                                                                                                                                                            |
| ----------------------------------------------------------------------------- | ---------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------- |
| Vendas, faturamento ou etapas zerados em datas antigas                        | É esperado antes de 12/11/2026, quando o histórico de colunas começou a ser gravado. Os eventos enviados antes dessa data continuam em "Eventos". Veja [Data de início do histórico](https://docs.convergefy.com.br/kb/meta-ads-dashboard.md). |
| "Investido" mostra "—" com um selo âmbar                                      | Abra o selo: ele lista as contas que ficaram de fora e o que fazer ("Tentar de novo" ou "Reconectar"). Veja [Avisos do investimento](https://docs.convergefy.com.br/kb/meta-ads-dashboard.md).                                                      |
| _"A conexão com a Meta expirou."_ (ou com o Google) na aba da plataforma      | Clique em **"Reconectar"**. A conexão abre por cima do Dashboard.                                                                                                                                                                                                      |
| _"A Meta limitou as consultas desta conta. Tente de novo em alguns minutos."_ | Espere alguns minutos e atualize. Não há o que corrigir na conta.                                                                                                                                                                                                      |
| "Atualizar" não mostra contatos, envios ou investimento novos                 | Esses números ficam guardados por até 15 minutos. Vendas e faturamento aparecem na hora. Salvar o Funil de conversão limpa a memória dos contatos e dos envios.                                                                                                        |
| Datas desabilitadas no calendário (_"Intervalo máximo de 90 dias."_)          | Escolha um intervalo de até 90 dias.                                                                                                                                                                                                                                   |
| Os números não batem com os painéis da Meta ou do Google                      | É esperado. Cada plataforma atribui a conversão com janelas próprias, e a Meta conta conversas, não contatos.                                                                                                                                                          |
| O total do painel de contatos é menor que o número clicado                    | É esperado: o painel lista contatos, um por contato, e o número conta negócios.                                                                                                                                                                                        |

## Topo da tela

- **Período** — Presets ("Hoje", "Ontem", "Esta semana", "Última semana", "Este mês", "Último mês") ou um intervalo no calendário, com **"Aplicar"**. A tela abre em "Hoje". No computador, o campo mostra ao lado a comparação: _"vs. ontem"_ para "Hoje" e _"vs. anterior"_ nos demais.
- **Etapas** — As etapas do seu Funil de conversão, por exemplo _"Contato › Qualificado › Venda · 2 funis"_. Clique para abrir **"De onde vem cada etapa"**. Na versão só CRM, o lugar dele fica com **"Configurar eventos de conversão"** (no celular, **"Eventos"**), que leva ao Funil de conversão.
- **Atualizar** — No computador, mostra há quanto tempo os números foram buscados (_"agora"_, _"há 12 min"_). No celular e no tablet, fica só o ícone. Clique para buscar de novo.
- **Exportar** — Baixa um arquivo CSV com os números da aba aberta. Fica desligado enquanto os números carregam. No celular e no tablet, fica só o ícone.

Abaixo ficam as abas: **"Visão geral"** e uma aba por plataforma conectada, **"Meta Ads"** e **"Google Ads"**, cada uma com o número de contatos daquela origem no período. Plataforma não conectada vira o botão **"Conectar Meta Ads"** ou **"Conectar Google Ads"**. O da Meta abre a conexão por cima do Dashboard. O do Google passa antes pela tela de autorização do Google e volta ao Dashboard com a conexão aberta. Esse botão só aparece para quem tem o nível Administrar no Rastreamento.

> **Limites do período e da atualização**
>
> O intervalo vai até 90 dias: as datas além disso ficam desabilitadas, com o aviso _"Intervalo máximo de 90 dias."_ Contatos, envios e investimento ficam guardados por até 15 minutos, então "Atualizar" pode demorar a mostrar o que é novo. Vendas, faturamento e "Em negociação" aparecem na hora. Salvar o Funil de conversão limpa na hora a memória dos contatos e dos envios, mas não a do investimento.

## Como os números são contados

O Dashboard usa três tipos de contagem. Cada card diz qual é a sua.

- **Contato** — Uma pessoa que chegou no período (o contato foi criado nesses dias). A origem é a do último clique em anúncio ou link rastreável. Por isso a origem de um contato pode mudar com o tempo, se ele clicar depois em outro anúncio.
- **Negócio que entrou numa coluna** — Cada vez que um negócio entra numa coluna do funil, isso fica no histórico com a data. Vendas, faturamento, desqualificados, as etapas do "Seu funil" e as das abas Meta Ads e Google Ads contam por esse histórico. O mesmo negócio conta uma vez em cada etapa.
- **Evento enviado** — Uma conversão aceita pela Meta ou pelo Google, como as listadas em "Eventos". Envio com status "Falhou" não conta. As colunas "Meta × Convergefy" da aba Meta Ads contam assim.

### Data de início do histórico

O histórico de colunas começou a ser gravado em **12/11/2026**. Tudo o que depende dele aparece zerado em datas anteriores: vendas, ganhos, faturamento, novos negócios, desqualificados, as etapas do "Seu funil" e das abas de plataforma, o diálogo "De onde vem cada etapa" e o card de um funil escolhido. Isso não muda com o tempo.

Contatos, origens, investimento e eventos enviados não dependem do histórico e aparecem normalmente em qualquer data. Os eventos enviados antes de 12/11/2026 continuam na tela "Eventos" e na coluna "Meta × Convergefy" da aba Meta Ads.

### Comparação com o período anterior

O chip ao lado do número (ex.: _"↑ 12%"_) compara com o período anterior de mesma duração, logo antes do escolhido. Passe o mouse para ler _"Comparado ao período anterior"_. Verde é subida, vermelho é queda e cinza é variação menor que 0,5%. O "Investido" fica sempre cinza: gastar mais não é bom nem ruim por si só.

O chip some quando o período anterior está zerado e quando há filtro de origem. Se o período anterior começa antes de 12/11/2026, ele está incompleto e a variação parece maior do que foi.

## Visão geral com anúncios

No topo, uma saudação e uma frase com o resumo, por exemplo _"Neste mês, você investiu R$ 3.200,00 e recebeu 120 contatos. Deles, 8 viraram venda e somaram R$ 14,2 mil."_ À direita, dois filtros, com **"Limpar"** quando algum está ativo:

- **Funil** — "Todos os funis" ou um funil só. Veja [Um funil escolhido](https://docs.convergefy.com.br/kb/meta-ads-dashboard.md).
- **Origem** — "Todas as origens", "Só anúncios (Meta + Google)", "Meta Ads", "Google Ads", "Outras origens" ou "Não rastreados". Recorta os números da tela. No card "De onde vêm seus contatos", as outras origens continuam à mostra, só que apagadas. Com uma origem sem anúncio, o "Investido" mostra _"Essa origem não tem custo"_.

### Os quatro números

- **Investido** — O gasto lido na Meta e no Google no período, em reais. Embaixo, de onde veio (_"em anúncios do Meta e Google"_) ou o que ficou de fora (_"sem o Google"_). Mostra "—" quando não há investimento ou nenhuma plataforma respondeu.
- **Em negociação** — O valor dos negócios em aberto **agora**, não no período (_"20 negócios em aberto"_). Não tem comparação.
- **Vendas** — Negócios que entraram em Ganho no período e continuam lá. Embaixo, o custo por venda (gasto ÷ vendas) ou _"Ganhos no período"_.
- **Faturamento** — A soma do valor desses negócios ganhos, com o ticket médio embaixo.

Se um número não carregar, o card mostra "—" e _"Não foi possível carregar"_, para não confundir com zero.

### Seu funil

O card **"Seu funil"** desenha as etapas do Funil de conversão, na mesma ordem (veja [Configurar](https://docs.convergefy.com.br/kb/meta-ads-configurar.md)):

- no topo, a faixa **"Contatos"** (_"Chegaram no período"_), com o filtro de origem aplicado;
- uma faixa por etapa, com o número de negócios que entraram numa coluna dela no período. Embaixo, o custo por etapa quando há investimento;
- entre as faixas, a taxa de avanço (_"NN% avançam"_). Passe o mouse para ler _"Dos que chegaram em {A}, quantos chegaram em {B}"_;
- no rodapé, _"De cada 100 que entram em Contatos, {N} chegam em {última etapa}."_

A etapa que envia evento tem um ícone de mira. Passe o mouse para ver o que ela envia. O link **"Como é calculado"** abre o diálogo "De onde vem cada etapa". Sem etapas montadas, o card mostra _"Monte as etapas em Funil de conversão para ver seu funil aqui."_ Com a origem em "Outras origens" ou "Não rastreados", o card some, porque não há conversão de anúncio a mostrar.

**O que o número de cada etapa conta**

- Os negócios que entraram, no período, numa coluna que pertence à etapa (você escolhe as colunas em "Onde acontece", no Funil de conversão). É a mesma conta do diálogo "De onde vem cada etapa", somando os funis.
- O mesmo negócio vale 1 por etapa, mesmo que entre na coluna mais de uma vez.
- Não depende de evento enviado: a etapa conta mesmo sem a Meta ou o Google conectados, ou sem evento escolhido.
- Com o filtro de origem, só contam os negócios de contatos daquela origem.

### Um funil escolhido

Com um funil no filtro, o card "Seu funil" vira **"Funil {nome}"**, com o link **"Abrir funil"** para o quadro. Cada faixa é uma coluna do funil e conta os negócios em aberto que entraram nela no período. Embaixo, quantos estão na coluna agora e, em média, quantos dias os negócios ficaram nela antes de sair. A última coluna mostra o valor vendido.

O rodapé aponta a maior queda entre duas colunas e traz os chips de ganhos, perdidos e desqualificados. Funil sem colunas mostra _"Este funil ainda não tem etapas."_

O resto da tela também muda:

- "Vendas", "Faturamento" e "Em negociação" passam a valer só para esse funil.
- O "contatos" da frase do topo passa a contar os negócios que entraram na primeira coluna do funil.
- O "Investido" continua sendo o de todas as campanhas. Por isso o custo por venda e o retorno comparam o gasto total com as vendas de um funil só.

### Retorno dos anúncios

O card **"Retorno dos anúncios"** mostra o ROAS (quanto voltou em venda para cada real investido): verde a partir de 1x, vermelho abaixo. Embaixo, "Lucro sobre anúncios", o custo da primeira etapa (ex.: "Custo por qualificado"), "Ticket médio" e "Tempo até a venda" (média de dias da criação do negócio até o Ganho).

O retorno e o lucro usam só as vendas de contatos que vieram da Meta ou do Google. O card "Faturamento" soma todas as origens, então os dois podem diferir. Quando não há como calcular, o card explica:

- _"Sem investimento no período."_: não houve gasto em anúncios.
- _"Sem o investimento, não dá para calcular o retorno."_: a Meta ou o Google não responderam. Veja [Avisos do investimento](https://docs.convergefy.com.br/kb/meta-ads-dashboard.md).
- _"Escolha uma origem com anúncios para ver o retorno."_: a origem está em "Outras origens" ou "Não rastreados".

### De onde vêm seus contatos

O card **"De onde vêm seus contatos"** divide os contatos do período em quatro origens, com número e percentual:

- **Meta Ads** — Vieram de um anúncio do Facebook ou do Instagram. Embaixo, o custo por contato.
- **Google Ads** — Vieram de um anúncio do Google. Embaixo, o custo por contato.
- **Outras origens** — Chegaram por um link rastreável sem anúncio da Meta ou do Google (_"orgânico e indicação"_).
- **Não rastreados** — Sem origem conhecida (_"sem link rastreável"_).

Clique numa origem para listar os contatos dela, ou em **"Ver contatos"** para todos. **"Ver por dia"** abre um gráfico de barras com os contatos ao longo do período (por hora, quando o período é de um dia só), uma cor por origem. Quando mais da metade chega sem rastreio, o card sugere usar o [link rastreável](https://docs.convergefy.com.br/kb/links-rastreaveis.md) nos anúncios.

## Visão geral só CRM

Sem Meta nem Google conectados, a Visão geral mostra só o funil de vendas, com o filtro de funil:

- **Novos negócios** — Negócios criados no período (_"entraram nos funis"_).
- **Em negociação** — O valor dos negócios em aberto agora.
- **Ganhos** — Negócios ganhos no período, com o percentual sobre os novos negócios.
- **Faturamento** — A soma do valor dos ganhos.

Abaixo, um funil com três faixas ("Contatos", "Negociação" e "Ganho"), somando todos os funis, e o card **"Resultado das vendas"**: a taxa de conversão (_"De cada 100 negócios que entram, {N} viram venda."_), "Ticket médio", "Tempo até a venda", "Perdidos" e "Desqualificados". Nessa versão os cards não têm comparação.

A aba **"Campanhas"** mostra _"Veja quanto custa cada venda"_ e os botões **"Conectar Meta Ads"** e **"Conectar Google Ads"** (_"Leva cerca de 2 minutos. Seus dados do CRM continuam iguais."_). Sem o nível Administrar, aparece _"Peça para quem administra a empresa conectar a conta de anúncios."_

## Abas Meta Ads e Google Ads

Cada aba mostra os anúncios de uma conta da plataforma cruzados com o seu funil. A aba só mostra: pausar, editar ou mudar orçamento é feito na própria plataforma.

1. **Escolher a conta** — No topo, **"Conta:"** mostra a conta de anúncio lida. Clique para trocar ou em **"Conectar outra conta"**. À direita, **"Abrir no Gerenciador"** (Meta) ou **"Abrir no Google Ads"** leva à plataforma.
2. **Ler o resultado** — O card **"Resultado dos anúncios"** traz Investido, Faturamento, Lucro (ou Prejuízo) e ROAS. Ao lado, "Contatos" e um card por etapa do Funil de conversão, cada um com o custo, e "Desqualificados", com a porcentagem dos contatos. Nessas etapas o chip pode mostrar _"novo"_, quando o período anterior estava zerado.
3. **Explorar as campanhas** — A tabela tem três níveis: "Campanhas", "Conjuntos de anúncios" (no Google, "Grupos de anúncios") e "Anúncios". Clique no nome para descer um nível, ou marque linhas e use o botão que aparece, como _"Ver conjuntos de 2"_ ou _"Ver anúncios de 2"_, para ver só o que está dentro delas. No nível de anúncio, o clique abre o detalhe do anúncio.

**Filtros e colunas da tabela**

- Busca _"Pesquisar por nome ou ID"_.
- Status: "Todos os status", "Ativos" ou "Desativados". A tabela abre em "Ativos".
- **"Colunas:"** troca o conjunto de colunas:
  - **Desempenho** (padrão): contatos, etapas, desqualificados, gasto, faturamento, lucro e ROAS, com o custo de cada um.
  - **Veiculação**: impressões, alcance (Meta), frequência (Meta), cliques, CTR, CPC e CPM.
  - **Criativo** (só Meta): taxas de retenção do vídeo, CTR e CPC.
  - **Meta × Convergefy** (só Meta): conversas que a Meta contou, contatos que chegaram à Convergefy, a diferença entre os dois e os eventos enviados em cada etapa.
- Selos de alerta na linha: "Frequência alta", "Aprendizado", "Escalar" (ROAS alto) e "Sem {etapa}" (muitos contatos sem chegar à primeira etapa).
- Clique no título de uma coluna para ordenar.

Os contatos de cada anúncio são os do último clique nele. Clique sem anúncio identificado não entra na tabela.

**Avisos e telas vazias das abas**

- _"Nenhuma conta de anúncio encontrada nesta conexão."_, com **"Conectar conta"**.
- _"Não foi possível consultar a Meta agora."_ (ou o Google), com **"Tentar de novo"**.
- _"A Meta limitou as consultas desta conta. Tente de novo em alguns minutos."_
- _"A conexão com a Meta expirou."_, com **"Reconectar"**, que abre a conexão por cima do Dashboard.
- _"Não foi possível carregar as campanhas."_, com **"Tentar de novo"**.
- _"Nenhum anúncio veiculou neste período."_ Escolha outro período.
- _"Nada encontrado com esses filtros."_, com **"Limpar filtros"**.

## Avisos do investimento

Quando alguma conta fica de fora do investimento, o card "Investido" ganha um selo âmbar com o número de avisos. Clique nele para abrir **"Avisos do investimento"**:

- “Não foi possível consultar o Meta agora. O investimento dele não entrou nos números.” — A plataforma não respondeu. O mesmo vale para o Google. Resolver: clique em “Tentar de novo”.
- “A conexão com o Google expirou. O investimento dele não entrou nos números.” — O acesso à conta venceu. O mesmo vale para a Meta. Resolver: clique em “Reconectar” e refaça a conexão em Contas de Anúncio.
- “Não foi possível consultar a conta {nome}. O investimento dela ficou de fora.” — Só aquela conta não respondeu. Resolver: clique em “Tentar de novo”.
- “A conta {nome} está em outra moeda ({moeda}) e ficou fora do investimento.” — A conta não está em real e a moeda dela não tem cotação. Resolver: nada a fazer: o Banco Central não tem cotação para essa moeda, então não dá para converter para real.

Conta em outra moeda (dólar, euro, libra e outras com cotação no Banco Central) entra convertida para real pela cotação PTAX do último fechamento publicado. O aviso diz a cotação usada, por exemplo _"(1 USD = R$ 5,8102)"_.

## Contatos por trás de um número

Clicar numa faixa do "Seu funil", numa origem ou em "Ver contatos" abre um painel lateral com os contatos daquele número:

| Clique                          | Título do painel                                                                                                                 |
| ------------------------------- | -------------------------------------------------------------------------------------------------------------------------------- |
| "Ver contatos"                  | _"Total de Contatos"_, ou a origem filtrada (ex.: _"Contatos · Meta Ads"_)                                                       |
| Uma origem                      | _"Contatos · Meta Ads"_, _"Contatos · Google Ads"_, _"Contatos · Outras origens"_ ou _"Contatos Não Rastreados"_                 |
| Faixa "Contatos" do "Seu funil" | _"Contatos"_, com _"Contatos que chegaram no período."_                                                                          |
| Faixa de uma etapa              | O nome da etapa, com _"Contatos com negócio em {etapa} no período. Cada contato aparece uma vez, mesmo com mais de um negócio."_ |

O painel lista **contatos**, um por contato, e o número da etapa conta **negócios**. Por isso o total do painel pode ser menor que o número clicado. Dá para buscar por nome ou telefone e filtrar por Departamentos, Atendentes, Status e Tags. Cada contato traz o botão **"Conversas"** e as "Informações de Rastreio" (anúncio, conjunto, campanha e conta). Com a origem em "Só anúncios (Meta + Google)", "Ver contatos" e a faixa "Contatos" do "Seu funil" não abrem lista, porque ela filtra uma origem por vez. As origens Meta Ads e Google Ads continuam abrindo.
