# Automações: Ativar e acompanhar

Como validar e ativar a automação, pausar ou arquivar, mexer nela rodando e acompanhar cada execução para entender o que rodou e o que deu erro.

Na Central de Ajuda: https://docs.convergefy.com.br/#/automacoes-ativar

## Em resumo

Salvar vale a qualquer momento, mesmo com problemas: o rascunho é gravado. **Ativar** é que exige tudo válido. Depois de ativa, a automação pode ser editada, pausada ou arquivada, e cada execução fica registrada no painel "Execuções".

### Algo deu errado?

Procure o que você está vendo e siga a coluna da direita. O detalhe de cada caso está mais abaixo.

| O que você vê                                                                | O que fazer                                                                                             |
| ---------------------------------------------------------------------------- | ------------------------------------------------------------------------------------------------------- |
| _"Resolva as pendências para ativar"_ no botão "Ativar automação"            | Abra o indicador de problemas no cabeçalho (ex.: _"1 problema"_) e clique no item para ir ao que falta. |
| _"Alguém salvou esta automação antes de você"_ ao salvar                     | Escolha qual versão fica. "Salvar a minha por cima" apaga o trabalho do colega, então combine antes.    |
| Execução com status "Falhou"                                                 | Abra a execução, veja o erro e use "Ver bloco com problema". A automação não tenta de novo sozinha.     |
| _"Conexão indisponível para enviar a mensagem."_                             | Reconecte o número (ver Conexões) ou aponte outra conexão no bloco.                                     |
| _"Número do lead não é válido no WhatsApp."_                                 | Confira e corrija o número do contato.                                                                  |
| _"Nenhum caminho de saída configurado para o erro."_                         | Ligue a saída de erro do bloco a um caminho.                                                            |
| _"Nó removido da automação."_                                                | Reabra a automação e religue o fluxo.                                                                   |
| _"Nó executado {N} vezes."_                                                  | Revise o ciclo do fluxo. Se o laço for proposital, aumente o "Máximo de vezes" do bloco.                |
| Mensagem de texto livre que não chega a um número da API Oficial             | Fora da janela de 24h, só template chega. Use um template aprovado.                                     |
| Botões ou Menu interativo impedindo a publicação numa conexão da API Oficial | Use template com botões de resposta rápida, ou troque a conexão do bloco.                               |
| _"Esta automação não está ativa."_ ao disparar pelo Chat                     | Ative a automação antes.                                                                                |
| _"Nenhuma execução encontrada"_                                              | Use "Limpar filtros" (põe o período em "Todas").                                                        |

## Validar e ativar

"Ativar automação" só libera sem pendências (_"Resolva as pendências para ativar"_).

> **Como achar o que falta**
>
> O indicador de **problemas** no cabeçalho (ex.: _"1 problema"_) abre a lista; clicar leva ao que falta. O bloco com erro também fica marcado no quadro.

> **Laço e Máximo de vezes**
>
> Laço é quando o fluxo volta para um bloco que já passou. Para **evitar laço infinito**, cada bloco (exceto o Agente de automação) tem um "Máximo de vezes" (padrão **10**): quantas vezes pode rodar na mesma execução do contato. Só importa quando o fluxo tem um ciclo. Ao estourar, a execução **para** com o erro "Bloco repetiu demais". Se o ciclo é proposital, aumente o limite em "Máximo de vezes" (seção "Controle" em Mensagem, Ações e Espera; sob "Execução" nos demais).

**Validações de estrutura do fluxo**

- **"Adicione um gatilho para iniciar o fluxo"**: o bloco de gatilhos está vazio.
- **"Adicione pelo menos um passo ao fluxo"**: só o gatilho não basta.
- **"Bloco sem ligação de entrada"**: bloco solto, sem ligação chegando nele. Ligue-o ao fluxo ou apague.
- **"Conecte a saída do gatilho 2 · …"**: com "Uma saída para cada gatilho" ligado, cada saída de gatilho precisa de uma ligação.
- **Saídas obrigatórias**:
  - Contato existente: _'Conecte a saída "Encontrado"'_ (_Não encontrado_ e _Tratamento de erro_ são opcionais).
  - Aguardar evento: _'Conecte a saída "Evento"'_ e _'Conecte a saída "Tempo esgotado"'_.
  - Aguardar resposta, Menu e Menu interativo: _'Conecte a saída "Tempo esgotado"'_ (as demais são opcionais).
- **"Nem todos os caminhos que chegam aqui possuem um negócio criado…"**: Mover negócio, Finalizar negócio e Definir produto do negócio exigem que algum passo antes tenha criado ou carregado um negócio em todos os caminhos que chegam ali.

**Validações dentro de um bloco**

- **"Adicione pelo menos um passo ao bloco"**: bloco Mensagem, Ações ou Espera vazio.
- **"O passo que cria saídas precisa ser o último do bloco"**: vale para Menu, Menu interativo, Aguardar resposta, Aguardar evento e Randomizador.
- **Passo exclusivo do WhatsApp Web numa conexão da API Oficial**: _"Menu interativo só funciona em conexões WhatsApp Web. … Troque a conexão deste bloco ou remova o passo."_ (e o equivalente para botões). Se a culpa é de um gatilho, a mensagem cita qual gatilho escuta uma conexão da API Oficial.

**Campos obrigatórios e tempos**

- Cada passo exige seus campos principais (mensagem, arquivo, funil e etapa, tag, status, departamento ou atendente…). O Menu e o Aguardar resposta mostram **"Adicione pelo menos uma opção"** / **"Cada opção precisa de ao menos uma palavra-chave"**.
- **"Deve ser maior que 0"** · **"Máximo 90 dias"**: esperas e tempos-limite vão de poucos segundos a 90 dias.
- **"Entre 1 e 60 segundos"**: duração do _digitando… / gravando…_.

## Ativar, pausar e arquivar

O estado aparece como um ponto colorido na lista e no topo do editor (passe o mouse para ver a descrição).

**Estados da automação**

- **Pausada** (gray) — _"Não começa para ninguém até ser ativada."_
- **Ativa** (green) — _"Começa sempre que um gatilho dispara."_
- **Pausa suave** (amber) — _"Não aceita contatos novos. Quem já entrou termina o fluxo. Fica assim até você ativar ou pausar."_ Como resolver: não vira Pausada sozinha: ative ou pause quando quiser.
- **Arquivada** (gray) — _"Arquivada. Não pode mais ser editada nem reativada."_ Como resolver: estado final: não dá para reverter nem editar.

> **Pausar, arquivar e excluir têm consequência na hora**
>
> - **Pausar** para de aceitar contatos novos e **cancela quem está no meio do fluxo**.
> - **Arquivar não tem volta**: a automação para, cancela as execuções em andamento e não pode mais ser editada nem reativada.
> - **Excluir** faz a automação e o histórico de execuções sumirem para sempre. Só aparece no menu da lista, em automações Pausadas ou Arquivadas.
> - Para parar sem cancelar ninguém, use **Pausar suavemente**: quem já entrou termina o fluxo.

**Controles de estado**

- **Ativar automação** — _"A automação passa a começar quando um gatilho disparar."_ Indisponível com pendência.
- **Pausar** — _"Para de aceitar contatos novos e cancela quem está no meio do fluxo."_ Em Pausa suave, o botão vira "Pausar agora" (_"Cancela quem ainda está no meio do fluxo."_).
- **Pausar suavemente** — No menu de três pontos (do editor ou da lista). Não aceita contatos novos, mas deixa terminar quem já entrou: o status vira Pausa suave. Para voltar a aceitar contatos, use "Reativar" no menu de três pontos do editor.
- **Arquivar (irreversível)** — "Arquivar automação?": _"Ela para, cancela as execuções em andamento e não pode mais ser editada nem reativada."_ → "Arquivar".
- **Duplicar** — "Duplicar automação": _"Criar uma cópia de X? A cópia será criada como inativa."_ (inativa é o mesmo que Pausada). Ao confirmar em "Duplicar", aparece "Duplicada!" (_"Abrindo a cópia…"_) e a cópia abre no editor. O nome é "Cópia de X" (se já existir, "Cópia de X (2)" e assim por diante). Ative a cópia quando estiver pronta.
- **Excluir** — Só no menu da lista, em automações Pausadas ou Arquivadas. "Excluir automação?": _"A automação e o histórico de execuções somem para sempre."_ → "Excluir".

## Editar com a automação rodando

> **Editar uma automação Ativa é permitido**
>
> Ao salvar, a mudança **já vale**, inclusive para quem está no meio do fluxo. Ficam somente leitura as automações Arquivadas e, para quem não tem o nível Administrar em Automações, todas.

> **Duas pessoas editando ao mesmo tempo**
>
> Se outra pessoa salvou enquanto você editava, ao salvar aparece "Alguém salvou esta automação antes de você". "Salvar a minha por cima" sobrescreve o que o colega salvou, **perdendo o trabalho dele**. Combine antes.

**Salvamento versionado e conflito de versão**

O aviso diz: _"Outra pessoa salvou mudanças enquanto você editava. Escolha qual versão fica."_ "Usar a versão salva" descarta o que você mudou; "Salvar a minha por cima" sobrescreve o que o colega salvou.

## Execuções: acompanhar o que rodou

No editor, o botão **"Execuções"** abre o painel com cada contato que passou pela automação, passo a passo, e onde parou. O painel se atualiza a cada 5 segundos; "Atualizar" recarrega na hora.

> **Histórico é apagado, cancelar não tem volta**
>
> _"Execuções finalizadas são apagadas depois de 7 dias."_ Vale para concluídas, com falha e canceladas. Cancelar uma execução em andamento tira o contato do fluxo agora e não dá para desfazer (veja "Cancelar uma execução", abaixo).

- **Período**: _Última 1 hora_ (padrão), _Últimas 2 horas_, _Últimas 4 horas_, _Hoje_, _Ontem_ ou _Todas_.
- **Status**: filtra pelas situações abaixo.
- **Busca**: _"Buscar por nome ou telefone…"_.
- Sem resultado no filtro: _"Nenhuma execução encontrada"_, com "Limpar filtros", que põe o período em Todas (não volta para _Última 1 hora_).
- Automação que nunca rodou: _"Nenhuma execução registrada"_. Lista que não carrega: _"Falha ao carregar execuções"_, com "Tentar novamente".

**Situação de cada execução**

- **Em andamento** (green) — Rodando agora.
- **Em espera** (amber) — Pausada num passo de espera (resposta, evento ou tempo).
- **Concluída** (green) — Terminou com sucesso.
- **Falhou** (red) — Um passo deu erro e a execução parou.
- **Cancelada** (gray) — _"Automação foi desativada durante a execução"_ (ou cancelada à mão).

Ao abrir uma execução, você vê o gatilho de entrada (_"Entrou pelo gatilho"_), o contato, o negócio (se houver) e cada passo na ordem em que rodou. Contato ou negócio apagado depois aparece como "Contato removido" / "Negócio removido".

Quando um passo falha, o registro guarda o erro com um selo:

- **"Tratado"**: havia um caminho de erro e o fluxo seguiu por ele.
- **"Sem tratamento"**: não havia caminho de erro, então a execução falhou.

O botão "Ver bloco com problema" leva ao bloco no quadro.

> **Por que a automação não tenta de novo sozinha**
>
> Se um passo falha, a execução **falha** e **não** tenta de novo. Isso evita, por exemplo, enviar a mesma mensagem duas vezes. Para tratar falhas, ligue a saída de erro do bloco a um caminho alternativo (ex.: uma nota interna avisando o atendimento).

**Disparar à mão pelo Chat (gatilho Execução manual)**

Automações ativas com o gatilho "Execução manual" podem ser disparadas na hora, dentro de uma conversa (ver [Atendimento / Chat](https://docs.convergefy.com.br/kb/chat.md)):

- O botão "Automações manuais", com as seções "Favoritos" (marque com a estrela) e "Todas". Sem nenhuma: _"Nenhuma automação com execução manual ativa."_
- O atalho "/" no campo de mensagem: a categoria "Automações manuais" aparece junto das mensagens rápidas e dos templates (até 100 automações; não aparece em conversa de grupo). Veja [Mensagens rápidas](https://docs.convergefy.com.br/kb/mensagens-rapidas.md).

O Chat pede confirmação: "Iniciar automação?" (com o nome) → "Iniciar" ou "Cancelar". Sucesso: "Automação iniciada com sucesso".

Por padrão ela dispara **sempre**, mesmo com uma execução em andamento para aquele contato. Para evitar clique duplicado, mude "Quando disparar" para "Se não estiver em execução" no gatilho.

**Cancelar uma execução**

Numa execução Em andamento ou Em espera, use o botão de ícone "Cancelar execução" (só para quem tem o nível Administrar em Automações). Confirme em "Cancelar esta execução?" (_"O contato sai do fluxo agora. Não dá para desfazer."_) → "Cancelar execução", ou toque em "Voltar".

**Detalhes do comportamento (limpeza e simultaneidade)**

- **Histórico antigo é limpo:** a limpeza roda uma vez por semana, então uma execução finalizada pode ficar visível por até cerca de 14 dias.
- **Cada evento gera uma execução:** o mesmo contato pode ter várias ao mesmo tempo. É intencional.
- **Esperas longas:** esperas acima de 24 horas são retomadas por uma verificação a cada 10 minutos, então a retomada pode atrasar alguns minutos.

**Mensagens enviadas por automação no Chat**

Cada mensagem de uma automação aparece na conversa com o selo "Automação" e o nome dela (ao passar o mouse: _"Enviada pela automação NOME"_). As falas do Agente de automação têm o selo "Agente de IA" e o nome da automação (_"Enviada pelo agente de IA da automação NOME"_). O nome mostrado é o que a automação tinha no momento do envio. Mensagens enviadas antes desse recurso existir não mostram o nome da automação. Veja [Atendimento / Chat](https://docs.convergefy.com.br/kb/chat.md).

## Erros de execução

Quando um passo falha, a execução registra um título e uma mensagem.

- “Conexão indisponível para enviar a mensagem.” — título "Conexão indisponível": a conexão usada estava offline ou foi removida. O fim da frase muda conforme o passo (_"…para enviar a pergunta."_ no Menu interativo, _"…para enviar a pergunta do menu."_ no Menu, _"…para o agente responder ao lead."_ no Agente de automação). Na Nota interna a mensagem é _"Não foi possível encontrar Chat para registrar a nota interna."_; reconectar não resolve, confira se a conversa do contato existe. Resolver: reconecte o número (ver Conexões) ou aponte outra conexão no bloco.
- “Número do lead não é válido no WhatsApp.” — título "Número inválido no WhatsApp" (ou "Falha na execução", quando a frase vem do indicador de digitando): o telefone do contato não tem WhatsApp ou está errado. Resolver: confira e corrija o número do contato.
- “Nenhum caminho de saída configurado para o erro.” — título "Saída sem ligação": o passo deu um erro previsto, mas a saída de erro ficou solta. Quando o sistema sabe qual foi o erro, a frase termina com um código interno entre aspas simples. Resolver: ligue a saída de erro do bloco a um caminho (em Mensagem, Ações e Espera, confira também se o Tratamento de erro está ligado na seção Controle).
- “Nó removido da automação.” — título "Bloco seguinte removido": um bloco apontava para outro que foi apagado. (Nó é o mesmo que bloco.) Resolver: reabra a automação e religue o fluxo.
- “Nó executado {N} vezes.” — título "Bloco repetiu demais": o contato passou pelo bloco vezes demais na mesma execução (proteção contra laço). Resolver: revise o ciclo do fluxo; se o laço for proposital, aumente o Máximo de vezes do bloco (seção Controle em Mensagem, Ações e Espera; seção Execução nos demais).
- “Falha ao enviar a mensagem pelo WhatsApp Business.” — título "Falha na execução": o provedor da conexão (WhatsApp Web ou API Oficial) recusou o envio. Resolver: confira se a conexão usada no bloco continua conectada em Conexões e se o número do contato é válido; depois tente de novo.
- “Falha ao enviar a mensagem pelo WhatsApp.” — título "Falha na execução": o WhatsApp recusou o envio do Menu interativo. Resolver: confira se a conexão do WhatsApp Web continua conectada em Conexões e se o número do contato é válido; depois tente de novo.
- “O provedor recusou uma mensagem do agente.” — título "Falha na execução": o WhatsApp recusou uma fala do Agente de automação. Resolver: confira se a conexão usada pelo agente continua conectada em Conexões.
- “Não foi possível enviar o template WABA.” — título "Falha na execução": o passo Template (mensagem-modelo aprovada pela Meta) não conseguiu enviar. No Menu a partir de template a mensagem é _"Não foi possível enviar o template do menu."_. Se a Meta devolve um motivo, a mensagem mostra o motivo no lugar dessa frase. Resolver: confira se o template ainda existe e está aprovado nessa conexão e se todos os parâmetros foram preenchidos.
- “A execução não tem conexão para comparar com o acesso do atendente.” — título "Falha na execução": a condição não sabe por qual conexão a conversa chegou (por exemplo, o gatilho não vem de uma mensagem). Resolver: use a condição É do atendente principal logo depois de um gatilho que traga uma conversa (como Mensagem recebida).
- “Erro ao executar '{nome do passo}'” — falha não prevista naquele passo. Abaixo do título aparece a mensagem técnica do erro. Resolver: verifique a configuração do passo; se persistir, procure o suporte.

> **Disparo manual sem permissão**
>
> Ao disparar pelo Chat, você pode ver _"Esta automação não está ativa."_ (ative a automação antes), _"Não foi possível executar a automação."_ (tente de novo) ou _"Você não tem permissão para fazer isso."_.

## Limitações conhecidas

> **Automações + API Oficial**
>
> As automações já enviam pela API Oficial (o WhatsApp Business da Meta, também chamado WABA), inclusive **templates** aprovados e menus que ramificam por botões de resposta rápida (ver _Templates da API Oficial_). Continua limitando: **fora da janela de 24h**, só template chega (texto e anexo livres podem não ser entregues), e cabeçalho de localização em template não é suportado. Veja [Conexões de WhatsApp](https://docs.convergefy.com.br/kb/conexoes.md).

> **Botões nativos e Menu interativo só no WhatsApp Web**
>
> Os botões no passo Texto e o Menu interativo não têm equivalente na API Oficial: numa conexão da API Oficial eles **impedem a publicação**. Na API Oficial, use **template com botões de resposta rápida**.
