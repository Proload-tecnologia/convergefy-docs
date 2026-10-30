# Agentes de IA

Um agente de IA é um atendente virtual que a sua empresa cria e ensina: ele conversa com o contato dentro de uma automação, responde com o jeito e as informações que você definiu, e reconhece situações da conversa que ramificam o fluxo.

Na Central de Ajuda: https://docs.convergefy.com.br/#/agentes-ia

## Em resumo

Um **agente de IA** é um atendente virtual que a sua empresa monta e treina. Você define quem ele é (personalidade), como atende (instruções), o que ele sabe (base de informações) e as respostas prontas para dúvidas comuns.

Depois de publicado, ele conversa com o contato dentro de uma automação. Também reconhece situações da conversa (ex.: _"interessado em comprar"_), e cada uma vira uma saída, para o seu fluxo seguir caminhos diferentes.

Você chega pelo item "Agentes de IA" da barra lateral. Dentro do editor de [automações](https://docs.convergefy.com.br/kb/automacoes.md), o passo que usa o agente se chama "Agente de automação": é o mesmo agente, visto de dois lugares.

A construção é assistida: o assistente construtor conversa com você e vai preenchendo a configuração. Você não precisa escrever tudo do zero.

> **Duas coisas com nomes parecidos**
>
> O [Assistente](https://docs.convergefy.com.br/kb/assistente.md) (a Letícia) responde as suas dúvidas sobre a plataforma. O agente de IA deste guia atende o seu contato, dentro de uma automação.

### Algo deu errado?

Procure o que você está vendo e siga a coluna da direita. O detalhe de cada caso está mais abaixo.

| O que você vê                                                                       | O que fazer                                                                                                                |
| ----------------------------------------------------------------------------------- | -------------------------------------------------------------------------------------------------------------------------- |
| O agente está publicado, mas não fala com ninguém                                   | Ele só atende dentro de uma automação. Adicione o passo "Agente de automação" e escolha este agente.                       |
| Você editou o agente e o atendimento não mudou                                      | Só o que está publicado vale. Pause o agente e use "Republicar e ativar". A base de informações é a exceção: vale na hora. |
| Botão "Criar com IA" desativado, com "Disponível com uma assinatura ativa."         | Ative ou regularize a assinatura (ver [Cobrança](https://docs.convergefy.com.br/kb/cobranca.md)).                              |
| "Configure ao menos a personalidade ou as instruções antes de publicar."            | Preencha a personalidade ou as instruções e publique de novo.                                                              |
| Fonte da base de informações em "Parcial"                                           | A fonte está disponível, mas veio incompleta. Passe o mouse para ver o motivo e use "Reprocessar".                         |
| Fonte da base de informações em "Erro no processamento"                             | Passe o mouse para ver o erro e use "Reprocessar". Se persistir, troque a fonte.                                           |
| Fonte de URL que veio só com os títulos, sem as respostas (FAQ, abas, "ver mais")   | O conteúdo que só abre ao clicar não é capturado. Cole o texto direto como fonte Texto.                                    |
| "Tipo de arquivo não suportado" ou "Arquivo acima de 50 MB"                         | Exporte em PDF, reduza o arquivo ou cole o conteúdo como fonte Texto.                                                      |
| "Esta chave é reservada pelo sistema."                                              | Escolha outra chave para a saída.                                                                                          |
| "Nenhuma saída de automação publicada. Publique no agente para ramificar por elas." | A saída só é acionada depois de publicar ou republicar o agente.                                                           |
| Automação parou de funcionar depois de excluir um agente                            | Excluir é permanente e derruba os passos "Agente de automação" que o usavam. Não dá para desfazer.                         |

## Como funciona, em 4 passos

O agente não atende sozinho só por existir ou estar publicado. Ele entra em ação dentro de uma automação. O caminho completo é:

1. **Criar e treinar** — Crie o agente e defina personalidade, instruções, base de informações, perguntas e saídas, com a ajuda do assistente construtor ou à mão.
2. **Testar** — Use "Testar" para conversar com ele sem afetar clientes, até ficar do jeito certo.
3. **Publicar** — Publique para deixar o agente disponível. Só o que está publicado vale no atendimento e nas automações.
4. **Usar numa automação** — Adicione o passo "Agente de automação" numa [automação](https://docs.convergefy.com.br/kb/automacoes.md) e escolha este agente. É a automação que entrega a conversa a ele e direciona o fluxo pelas saídas que ele reconhece. Sem isso, este agente não fala com ninguém.

**Conceitos rápidos**

- **Agente** — O atendente virtual que você cria. Tem nome, cor/ícone e uma configuração própria.
- **Assistente construtor** — A IA que te ajuda a montar o agente conversando no chat: sugere personalidade, instruções, perguntas e saídas.
- **Personalidade** — Quem o agente é, como se apresenta e o tom de voz.
- **Instruções** — Como ele conduz o atendimento, o que prioriza e o que nunca faz.
- **Base de informações** — Textos, links e documentos que o agente usa como fonte (cada um é processado automaticamente).
- **Perguntas e Respostas** — Respostas prontas para dúvidas comuns, usadas como referência.
- **Saída de automação (intenção)** — Uma situação que o agente reconhece na conversa (ex.: _Qualificação_, _Vendas_). Cada uma vira um ponto de saída no passo "Agente de automação".
- **Publicar** — Tira uma cópia da configuração atual e ativa o agente. Só o que está publicado vale no atendimento e nas automações.
- **Testar** — Uma conversa de teste, isolada: não fala com o cliente nem dispara automações.

## Onde fica e quem acessa

Na barra lateral, clique em "Agentes de IA". O item aparece para o Administrador e para quem tem o nível Administrar na área "Agentes de IA" do acesso do membro. Para os demais, ele não aparece (ver [Equipe e permissões](https://docs.convergefy.com.br/kb/equipe-permissoes.md)).

Para criar um agente, o acesso precisa estar em dia: assinatura ativa ou período de experiência em andamento. Fora disso, o botão de criar fica desativado com o aviso _"Disponível com uma assinatura ativa."_ (ver [Cobrança](https://docs.convergefy.com.br/kb/cobranca.md)).

Tela "Agentes de IA": _"Crie e gerencie seus agentes de atendimento."_ Cada agente aparece como um cartão com avatar colorido, nome, descrição e um selo de estado. Quando ainda não há nenhum: _"Nenhum agente ainda"_, _"Crie seu primeiro agente de atendimento. A IA te guia na construção."_

**Estado de cada agente**

- **Atendendo** (green) — publicado e ativo, pronto para atender nas automações que o usam.
- **Pausado** (amber) — publicado, mas com o atendimento parado no momento.
- **Rascunho** (gray) — ainda não foi publicado; só existe em construção.

## Criar um agente

1. **Iniciar** — Clique em **"Criar com IA"** (ícone ✨). Abre a tela "Novo agente": _"Converse com o assistente para criar seu atendente."_
2. **Conversar com o construtor** — O assistente se apresenta e conduz por passos: nome → jeito de falar → o que vai fazer. Responda no chat em linguagem normal. Ele vai preenchendo a configuração à direita conforme vocês conversam.
3. **(Opcional) Dar exemplos de atendimento** — No painel "Não sabe o que fazer? Comece por aqui!", use um atalho para a IA aprender o seu estilo a partir de conversas reais (veja abaixo).

**Ensinar o estilo com conversas de referência**

Dois atalhos alimentam a IA com exemplos do seu atendimento, e cada um tem o seu teto:

- **Conversas do Convergefy** — _"Use atendimentos reais já registrados aqui para a IA aprender seu estilo."_ Abre "Escolher conversas de referência": _"Toque nas conversas para escolhê-las (até 10). Use o botão para ver as mensagens."_ Dá para buscar (_"Buscar por nome ou telefone…"_) e filtrar por Todas / Aguardando / Em atendimento / Finalizadas.
- **Colar ou anexar conversa** — _"Cole conversas ou anexe arquivos de texto (.txt, .md) de qualquer origem."_ Cole o texto e clique em "Adicionar texto colado", ou use "Anexar arquivo" (limite de 2 MB por arquivo). Nada é enviado até você confirmar no botão final, que mostra _"Usar 1 conversa"_ / _"Usar {N} conversas"_. Aqui o teto é 5 conversas. Ao passar disso aparece _"Máximo de 5 conversas."_

## A página de configuração

A página do agente tem dois lados. À esquerda fica o chat do assistente, sempre à mão e redimensionável no computador. À direita ficam as seções de configuração, todas abertas uma abaixo da outra. Em telas menores que 1024 px (celular e tablet), a página alterna entre "Assistente" e "Configuração".

No topo ficam o avatar (clique para trocar a cor/ícone), o nome (clique para renomear), o estado, o botão "Testar" e o botão de publicar/pausar. As alterações são salvas automaticamente: um indicador discreto mostra _"Salvando…"_ e depois _"Salvo"_ (ou _"Erro ao salvar"_).

### As seções

- **Personalidade** — _"Quem o agente é, como se apresenta e o tom de voz que adota."_
- **Instruções** — _"Como o agente conduz o atendimento, o que prioriza e o que nunca faz."_
- **Base de informações** — _"Texto, links e documentos que o agente usa como base. Cada fonte é processada e convertida automaticamente."_
- **Perguntas e Respostas** — _"Respostas prontas para as dúvidas mais comuns. O agente as usa como referência no atendimento."_
- **Saídas de automação** — _"Situações que o agente reconhece na conversa. Cada uma vira um ponto de saída no passo de automação."_

> **Pedir ao assistente em qualquer seção**
>
> Cada seção tem o botão "Pedir ao assistente" (✨): a IA escreve ou sugere o conteúdo daquela parte para você. Você também pode editar tudo à mão. Em campos vazios aparece _"Nada definido ainda. Edite à mão ou peça ao assistente."_

### Base de informações (fontes)

Adicione fontes por arquivo, URL ou texto:

- **Arquivo** — _"Clique para selecionar ou arraste um arquivo"_. Aceita PDF, TXT, MD (Markdown), DOC e DOCX, até 50 MB por arquivo. Para planilhas, apresentações ou qualquer outro formato, exporte em PDF ou cole o conteúdo como fonte Texto.
- **URL** — Informe um endereço válido (_"Informe uma URL válida"_) e um título opcional. A Convergefy lê o conteúdo da página automaticamente e o converte em texto para o agente. Páginas e sites muito grandes podem vir parciais (veja os estados abaixo). Como a página pode mudar com o tempo, você pode reprocessar uma fonte de URL quando quiser, para recapturar o conteúdo atualizado.
- **Texto** — Cole o conteúdo direto e dê um título opcional.

**Sobre o seletor de arquivos**

A área de arquivos aceita PDF, DOC, DOCX, TXT e MD (Markdown), e é essa a lista que aparece embaixo dela. Qualquer outro formato é recusado na hora, com _"Tipo de arquivo não suportado"_.

> **Conteúdo que só aparece ao clicar não é capturado**
>
> Ao ler uma URL, a Convergefy captura o que está visível na página assim que ela carrega. Conteúdo que só abre ao clicar fica de fora: perguntas de uma FAQ em sanfona (accordion), abas, botões "ver mais". Costuma vir só com os títulos, sem as respostas. Se a fonte importante está escondida atrás de um clique, cole o texto direto como fonte Texto, ou aponte para uma URL onde o conteúdo já apareça aberto.

Cada fonte na lista:

- pode ser ligada/desligada ou removida (_"Fonte removida"_);
- tem "Reprocessar" (_"Reprocessamento iniciado"_) só onde faz sentido: fonte com erro, com conteúdo parcial, ou fonte de URL já pronta. Arquivo e texto processados com sucesso não mostram a opção;
- quando está Pronta, deixa ver o conteúdo processado (o texto que o agente realmente lê) num painel lateral, sem sair da página.

Cada fonte é processada automaticamente antes de o agente poder usá-la.

**Estado de cada fonte**

- **Aguardando** (gray) — na fila, ainda não começou a processar.
- **Processando…** (blue) — a Convergefy está lendo e convertendo a fonte.
- **Pronto** (green) — processada por completo e disponível para o agente.
- **Parcial** (amber) — a fonte ficou disponível, mas o conteúdo veio incompleto, o que é comum em sites grandes. O agente usa o que foi capturado. Como resolver: passe o mouse para ver o motivo e use Reprocessar para tentar capturar o restante.
- **Erro no processamento** (red) — falhou ao ler/converter a fonte. Como resolver: passe o mouse para ver o erro e use Reprocessar; se persistir, troque a fonte.

### Saídas de automação (intenções)

Use "Adicionar saída" para definir uma situação que o agente reconhece. Cada saída tem:

- **Categoria** — Qualificação, Vendas, Suporte, Agendamento, Transferência ou Outro.
- **Nome** — Como a saída aparece (ex.: _"Interessado em comprar"_). Até 120 caracteres.
- **Chave** — Identificador único, em letras minúsculas, números e \_ (ex.: `interessado_comprar`), até 64 caracteres. Algumas chaves são reservadas pelo sistema. Se escolher uma delas, aparece _"Esta chave é reservada pelo sistema."_; use outra.
- **Quando detectar** — _"O cliente pede explicitamente atendimento humano…"_ descreve a situação para o agente saber quando acionar essa saída. Opcional, até 2000 caracteres.

Ao criar ou editar, uma pré-visualização mostra _"Como esta saída aparece no passo Agente de automação das automações:"_. A sua saída aparece junto às fixas: "Atendente entrou na conversa", "Sem resposta do contato" e "Tratamento de erro". No bloco real existe ainda a saída "Limite de respostas", que só aparece quando você preenche o limite no passo da automação.

> **Saída aparece ao salvar, vale depois de publicar**
>
> A saída aparece no bloco de automação assim que é salva, mas o agente só passa a acioná-la depois de publicar ou republicar. No editor de automação, um agente sem nenhuma saída cadastrada mostra _"Nenhuma saída de automação publicada. Publique no agente para ramificar por elas."_

## Testar o agente

Clique em "Testar" para abrir uma conversa de teste lateral, "Testar {nome do agente}": _"Conversa de teste — não envia ao lead nem dispara automações."_ Você escreve como se fosse o contato, e o agente responde com a configuração atual (rascunho). Dá para experimentar mudanças antes de publicar, sem afetar clientes nem fluxos reais.

Antes da primeira mensagem aparece _"Envie uma mensagem para testar"_, _"O agente responde com a configuração atual (rascunho), sem afetar conversas reais."_

## Publicar, pausar e republicar

> **Só o publicado vale, exceto a base de informações**
>
> Editar a configuração não muda o atendimento na hora: o que está no ar é a última versão publicada. Sempre publique (ou republique) para que as alterações passem a valer: personalidade, instruções, novas saídas de automação.
>
> A base de informações é a exceção: ela é lida ao vivo. Adicionar, editar, desativar ou excluir uma fonte vale na hora, sem republicar, inclusive num agente já em atendimento.

1. **Publicar** — Quando a configuração estiver pronta, clique em **"Publicar"**. Isso tira uma cópia da configuração atual e ativa o agente (estado Atendendo). Confirmação: _"Agente publicado e ativado"_. Um agente sem personalidade e sem instruções não publica: aparece _"Configure ao menos a personalidade ou as instruções antes de publicar."_
2. **Pausar** — Com o agente ativo, **"Pausar"** interrompe o atendimento (estado Pausado), com a mensagem _"Atendimento pausado"_, sem perder a configuração publicada.
3. **Republicar** — Depois de editar um agente já publicado, pause-o e use **"Republicar e ativar"** para que as mudanças passem a valer no atendimento. Esse botão só aparece com o agente Pausado. Com o agente em Atendendo, o cabeçalho mostra só "Pausar".

## Usar o agente numa automação

O agente entra no fluxo pelo passo "Agente de automação" do [editor de automações](https://docs.convergefy.com.br/kb/automacoes.md). Você escolhe qual agente atende, e o bloco ganha uma saída por situação cadastrada do agente, além de saídas fixas como _"Sem resposta do contato"_. Os detalhes do bloco (campos, saídas e limites) estão em [Automações](https://docs.convergefy.com.br/kb/automacoes.md).

### Como a mensagem do agente aparece no chat

Na conversa, cada mensagem que o agente envia leva o selo "Agente de IA" e o nome da automação que o acionou. Ao passar o mouse, aparece _"Enviada pelo agente de IA da automação {nome}"_. Assim a equipe distingue o que foi o agente do que foi um atendente.

## Excluir um agente

> **Excluir quebra as automações que usam o agente**
>
> Apagar um agente é permanente e derruba os passos "Agente de automação" das automações que dependem dele. Pause em vez de excluir se for só uma pausa temporária.

No menu (⋮) do cartão (que também tem "Testar"), use **"Excluir"**. É o único caminho: a página do agente não oferece a exclusão. A confirmação é **"Excluir agente?"**: _"O agente {nome} e todas as suas configurações serão removidos permanentemente. Automações que o usam deixam de funcionar. Esta ação não pode ser desfeita."_

## Erros e avisos esperados

- “Erro ao carregar agentes” — a lista de agentes não carregou (_"Ocorreu um problema ao listar os agentes. Tente novamente."_). Resolver: clique em “Tentar novamente”; se persistir, recarregue a página.
- “Disponível com uma assinatura ativa.” — o botão “Criar com IA” fica desativado sem assinatura ativa. Resolver: ative ou regularize a assinatura para criar agentes (ver Cobrança).
- “Máximo de 10 conversas.” — tentou escolher mais de 10 conversas do Convergefy como referência. Resolver: remova alguma antes de adicionar outra.
- “Máximo de 5 conversas.” — tentou colar/anexar mais de 5 conversas de fora. Resolver: remova alguma antes de colar ou anexar outra.
- “Configure ao menos a personalidade ou as instruções antes de publicar.” — tentativa de publicar um agente vazio. Resolver: preencha a personalidade ou as instruções e publique de novo.
- “Arquivo acima de 50 MB” — a fonte da base de informações passou do tamanho máximo. Resolver: reduza o arquivo ou divida o conteúdo em fontes menores.
- ““{arquivo}” passa de 2 MB.” — arquivo de referência grande demais. Resolver: anexe um arquivo de texto menor (até 2 MB).
- “Esta chave é reservada pelo sistema.” — a chave digitada na saída de automação é reservada. Resolver: escolha outra chave para a saída.
- “Não foi possível excluir o agente.” — falha ao excluir o agente. Quando dá certo, aparece _"Agente excluído com sucesso"_. Resolver: tente de novo; se persistir, procure o suporte.
