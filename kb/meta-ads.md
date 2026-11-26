# Rastreamento

O Rastreamento liga seu funil de vendas aos anúncios do Facebook, Instagram e Google. Quando um negócio avança (ex.: fecha uma compra), a Convergefy avisa a plataforma de anúncios, e as campanhas aprendem a trazer clientes parecidos. Também mostra de onde cada contato veio.

Na Central de Ajuda: https://docs.convergefy.com.br/#/meta-ads

## Em resumo

O Rastreamento conecta o CRM aos anúncios da **Meta** (Facebook e Instagram) e do **Google Ads**. Você agrupa colunas dos seus funis em **etapas de conversão** (ex.: "Compra") e escolhe o evento que cada uma envia. Quando um negócio entra numa dessas colunas, a Convergefy envia esse resultado, a **conversão**, à plataforma. Os anúncios passam a buscar pessoas parecidas com quem comprou.

O envio é de servidor para servidor, direto à Meta e ao Google, sem depender de cookie no navegador do cliente. Na Meta isso se chama API de Conversões.

### Algo deu errado?

Procure o que você está vendo e siga a coluna da direita. O detalhe de cada caso está mais abaixo, ou nos guias [Configurar](https://docs.convergefy.com.br/kb/meta-ads-configurar.md), [Acompanhar](https://docs.convergefy.com.br/kb/meta-ads-acompanhar.md) e [Dashboard](https://docs.convergefy.com.br/kb/meta-ads-dashboard.md).

| O que você vê                                                                     | O que fazer                                                                                                                                                                                                                                           |
| --------------------------------------------------------------------------------- | ----------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------- |
| O item "Rastreamento" não aparece na barra lateral                                | O seu nível é "Nenhum" (modelo Básico). Peça a um Administrador o nível Ver ou Administrar na aba "Acesso" do membro.                                                                                                                                 |
| Os botões de alteração sumiram e "Gerenciar" virou "Ver detalhes"                 | Você tem o nível Ver, só leitura. Para conectar contas, cadastrar pixels ou salvar o Funil de conversão, é preciso o nível Administrar.                                                                                                               |
| Em "Origem do contato", campanha, conjunto ou anúncio aparecem só como ID         | É normal logo após o clique. A Convergefy busca o nome na plataforma e até lá mostra o ID. Na Meta, precisa haver uma conta do Facebook conectada que enxergue o anúncio. No Google, é preciso ter conectado o Google e escolhido a conta de anúncio. |
| Uma conta do Google Ads não aparece na lista                                      | Veja a nota "Conta do Google que não aparece na lista", mais abaixo.                                                                                                                                                                                  |
| Uma etapa do Funil de conversão mostra "Falta o evento" ou "Falta escolher funil" | Ela ainda não envia nada. Escolha o evento e a coluna do funil em "Enviar como" e "Onde acontece". Veja [Passo 2: Funil de conversão](https://docs.convergefy.com.br/kb/meta-ads-configurar.md).                               |
| Resultado inesperado nas conversões                                               | Confira "Eventos" (detalhe e payloads, o conteúdo técnico do envio) e "Contas de Anúncio", ou procure o suporte.                                                                                                                                      |

> **Quem vê e quem altera**
>
> O nível de acesso ao Rastreamento é definido na aba "Acesso" do membro. Ver [Equipe e permissões](https://docs.convergefy.com.br/kb/equipe-permissoes.md).
>
> - Nível "Nenhum" (modelo Básico): a área não aparece.
> - Ver: dashboard, eventos, Funil de conversão e links, só para leitura.
> - Administrar: também conecta Meta e Google, cadastra pixels, salva o Funil de conversão, cria links e busca respostas de formulário da Meta.
>
> Sem Administrar, os botões de alteração somem ("Gerenciar" vira "Ver detalhes"). O item da barra lateral se chama "Rastreamento" ("Rastreio" no celular).

**Conceitos rápidos**

- **Pixel (Meta)** — O destino das suas conversões na Meta. Os pixels que você compartilha ao conectar a conta entram sozinhos na lista.
- **Token de acesso** — Chave própria de um pixel para o envio. Opcional: sem token, o pixel envia pela conta do Facebook conectada.
- **Pixel de CRM** — Pixel marcado como "de CRM" na Meta, usado em campanhas de formulário otimizadas para leads de CRM (Conversion Leads). Na Convergefy a marcação só informa: todos os pixels recebem as conversões do funil e os leads dos formulários dos anúncios.
- **Ação de conversão (Google)** — O equivalente do pixel no Google Ads. Você a cria no Google Ads e a escolhe na Convergefy.
- **Evento de conversão** — O resultado informado. Na Meta, o nome oficial do evento (ex.: Purchase). No Google, a ação de conversão escolhida.
- **Etapa de conversão** — Um grupo que você cria no Funil de conversão, com nome livre, reunindo uma ou mais colunas de um ou mais funis. Cada etapa escolhe o evento da Meta e/ou a ação do Google que é enviado quando um negócio entra numa dessas colunas. Não é a coluna do funil de vendas.
- **Identificador de clique** — Código que a plataforma cola no link do anúncio e que liga o contato ao anúncio clicado. Na Meta, ctwa\_clid (anúncio que abre o WhatsApp). No Google, GCLID, GBRAID e WBRAID.
- **UTM** — Parâmetros no fim de um link (utm\_source, utm\_medium, utm\_campaign, utm\_content, utm\_term) que dizem de qual campanha ou canal veio o clique.
- **Origem** — O anúncio ou link que trouxe o contato. Vale sempre o clique mais recente.
- **Conjunto / Grupo de anúncios** — O nível entre a campanha e o anúncio. Na Meta chama "Conjunto", no Google "Grupo de anúncios".

## Onde fica e como se organiza

Na barra lateral, abra **Rastreamento** (_"Conversões para anúncios"_). São cinco telas, no menu do próprio Rastreamento:

| Seção         | Telas                                                  | Para quê                                                       |
| ------------- | ------------------------------------------------------ | -------------------------------------------------------------- |
| MONITORAMENTO | Dashboard, Eventos                                     | Ver o que foi enviado e o desempenho.                          |
| CONFIGURAÇÕES | Link rastreável, Funil de conversão, Contas de Anúncio | Criar links, conectar contas e definir o que cada etapa envia. |

O botão **"Recolher menu do Rastreamento"**, no topo do menu, libera espaço para a tela. Com o menu recolhido, o cabeçalho da página mostra **"Abrir menu do Rastreamento"** (só em tela média para cima). A escolha fica salva para o seu usuário.

> **Ordem recomendada**
>
> Comece por "Contas de Anúncio", depois o "Funil de conversão". Só então "Dashboard" e "Eventos" mostram dados. O "Link rastreável" é independente e tem [guia próprio](https://docs.convergefy.com.br/kb/links-rastreaveis.md).

## Origem do anúncio (de onde o contato veio)

Quando alguém clica num anúncio do Facebook/Instagram ou do Google e abre o WhatsApp, a plataforma manda junto de qual anúncio a conversa veio. A Convergefy guarda isso e mostra em três lugares:

- "Origem do contato", no painel do contato no Chat;
- a aba "Rastreio" do contato (ver [Contatos](https://docs.convergefy.com.br/kb/contatos.md));
- "Informações de Rastreio", no painel de contatos do Dashboard.

A seção abre com um resumo: a plataforma (Meta Ads, Google Ads ou Outra origem) com o horário do clique, o anúncio em destaque e, embaixo, campanha › conjunto (campanha › grupo de anúncios no Google). Numa "Outra origem", o destaque é utm\_source / utm\_medium e a campanha vai embaixo.

"Detalhes da origem" abre a lista completa, com os campos que existirem:

- **Anúncio, Conjunto (ou Grupo de anúncios), Campanha** — O nome de cada nível. "Conjunto" na Meta, "Grupo de anúncios" no Google.
- **Conta** — O nome e o ID da conta de anúncios. É o único ID mostrado ao lado do nome, porque é o que se cola no gerenciador de anúncios para achar o anunciante.
- **Identificadores de clique** — Na Meta, "Clique (ctwa\_clid)". No Google, GCLID, GBRAID e WBRAID.
- **UTMs** — utm\_source, utm\_medium, utm\_campaign, utm\_content e utm\_term, quando o link tiver.
- **Clique em** — Data e hora do clique.

O ID de anúncio, conjunto/grupo e campanha só aparece no lugar do nome, enquanto o nome não chega. Às vezes o WhatsApp avisa que a conversa veio de um anúncio da Meta sem dizer qual: a origem fica "Meta Ads", com o horário do clique, mas sem anúncio, conjunto nem campanha. Uma "Outra origem" (sem anúncio, só link de campanha) traz apenas as UTMs e o horário.

### Formulários de anúncio

Quem respondeu a um formulário da Meta ganha, na "Origem do contato", a linha fechada "Formulário · ‹nome›", com a quantidade de respostas e a data.

- Se a origem atual é o formulário, ele fica logo abaixo do resumo. Os demais vão para "Formulários anteriores".
- Sem outra origem, aparece _"Origem não rastreada. O contato respondeu a um formulário de anúncio."_
- No Chat, o formulário também aparece como um cartão na data do envio, com as respostas (as três primeiras e "Ver todas as N respostas").
- Na lista de conversas e no card do funil, quem chegou por formulário tem a etiqueta "Form".

> **Os nomes podem demorar a aparecer**
>
> Logo após o clique, às vezes só o ID está disponível. A Convergefy busca o nome da campanha, do conjunto/grupo e do anúncio na plataforma, e até lá mostra o ID. Para isso:
>
> - Meta: é preciso ter uma conta do Facebook conectada que enxergue o anúncio.
> - Google: é preciso ter conectado o Google e escolhido a conta de anúncio. A busca olha os cliques dos últimos 3 dias.

## Limitações conhecidas

> Todos os pixels recebem as mesmas conversões: não dá para mandar uma etapa a um pixel e outra etapa a outro. Os contatos que vieram de formulário de anúncio também vão a todos, só que como evento de CRM ([veja em Configurar](https://docs.convergefy.com.br/kb/meta-ads-configurar.md)). Com resultado inesperado, confira "Eventos" (detalhe e payloads) e "Contas de Anúncio", ou procure o suporte.

> **Conta do Google que não aparece na lista**
>
> A lista traz as contas de cliente. Contas gerenciadoras (MCC, que administram outras contas) não aparecem, só as contas de cliente ligadas a elas. Contas sem permissão para o login conectado ou não ativas (cadastro incompleto, suspensa ou desativada) não podem ser escolhidas. Elas não somem em silêncio: no fim da lista aparece "N contas não puderam ser lidas", com o número e o motivo, por exemplo _"Sem acesso a esta conta no Google Ads. Verifique as permissões ou reconecte."_ Resolva no Google Ads e use "Atualizar lista".
