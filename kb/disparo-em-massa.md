# Disparo em massa

O Disparo em massa envia a mesma mensagem de WhatsApp para um público escolhido por tags, por colunas do funil, por atendente principal, ou uma combinação deles — no ritmo e nos horários que você definir. Você monta a campanha uma vez e acompanha o envio pela lista.

Na Central de Ajuda: https://docs.convergefy.com.br/#/disparo-em-massa

## Em resumo

Uma campanha de disparo é uma mensagem só, enviada para muitos contatos, um a um, no ritmo que você escolher. Você chega por barra lateral → **"Disparo em massa"** (no celular, o item se chama **"Disparos"**). Título da tela: "Disparo em massa", com o texto _"Crie campanhas de disparo e envie mensagens em massa pelo WhatsApp."_

Há duas portas de entrada, e elas se comportam diferente:

| Por onde você cria                                        | O que acontece ao salvar                                                                                        |
| --------------------------------------------------------- | --------------------------------------------------------------------------------------------------------------- |
| Botão **"Nova campanha"** da lista                        | A campanha nasce em Rascunho e **não envia nada** até você clicar em **"Iniciar"**.                             |
| Menu (⋮) de uma coluna do Funil → **"Disparar em massa"** | A campanha **começa a enviar na hora**, assim que você confirma. Veja "Disparar direto de uma coluna do Funil". |

> **O WhatsApp pune excesso de envio em massa**
>
> Envio em massa é o tipo de uso que mais leva **número a bloqueio**: quanto mais rápido e mais volumoso o disparo, maior o risco. Comece pela velocidade "Recomendado", use listas realmente interessadas e prefira números já aquecidos (ver [Conexões de WhatsApp](https://docs.convergefy.com.br/kb/conexoes.md)).

### Algo deu errado?

Procure o que você está vendo e siga a coluna da direita. O detalhe de cada caso está mais abaixo.

| O que você vê                                                             | O que fazer                                                                                                                                                                 |
| ------------------------------------------------------------------------- | --------------------------------------------------------------------------------------------------------------------------------------------------------------------------- |
| Disparou pelo Funil e não queria                                          | Use "Pausar" na lista. O que já saiu não volta.                                                                                                                             |
| Campanha "Pausada" depois que a conexão caiu                              | Ela não volta sozinha. Reconecte o número e use "Retomar" na lista.                                                                                                         |
| Campanha "Pausada" por você                                               | Use "Retomar" para voltar a enviar.                                                                                                                                         |
| Campanha "Falhou"                                                         | Não foi possível preparar a lista de destinatários e nada foi enviado. Confira o público e a conexão, e crie a campanha de novo.                                            |
| Contato "pulado" com o motivo _"Contato sem telefone válido."_            | Esse contato não recebe: ele entra como pulado.                                                                                                                             |
| Cadeado na linha e _"Esta campanha usa uma conexão que você não acessa."_ | A campanha fica só para leitura e qualquer ação nela é recusada. Veja a restrição de conexões em [Equipe e permissões](https://docs.convergefy.com.br/kb/equipe-permissoes.md). |
| _"O template escolhido não foi encontrado ou não está aprovado."_         | Escolha outro template na lista; se ele existia, confira o status dele no painel da Meta.                                                                                   |
| _"A conexão escolhida foi removida, está desligada ou está incompleta."_  | Reconfigure a conexão em Conexões ou crie a campanha de novo apontando uma conexão ativa.                                                                                   |

O item aparece para quem tem o nível **Operar** na área Disparo em massa (aba "Acesso" do membro, ver [Equipe e permissões](https://docs.convergefy.com.br/kb/equipe-permissoes.md)). Quem está no nível básico, que nessa área é "Nenhum", não vê as campanhas nem o item no menu. Ao lado do título, a tela conta quantas campanhas existem (_"(7 campanhas)"_), traz a busca "Buscar por nome..." e o botão "Nova campanha".

**Conceitos rápidos**

- **Campanha** — A configuração inteira: público, mensagem, dias/horários e velocidade.
- **Destinatário** — Cada contato da lista, com o próprio resultado (enviado, falha, pulado, cancelado).
- **Janela** — Um intervalo de horas de um dia da semana em que a campanha pode disparar.
- **Velocidade** — De quanto em quanto tempo sai uma mensagem, mostrada como "envios por hora" (média).
- **API Oficial** — O WhatsApp Business da Meta, também chamado WABA. É um dos dois tipos de conexão (o outro é o WhatsApp Web). Veja [Conexões de WhatsApp](https://docs.convergefy.com.br/kb/conexoes.md).
- **Template** — Mensagem-modelo aprovada pela Meta. Fora de uma conversa aberta, é o único formato que a Meta entrega nessa conexão.

## O que a lista mostra

Cada linha da tabela traz: Nome · Conexão · Dias · Velocidade · Progresso · Falhas · Status · Ações.

Os Dias aparecem como as iniciais da semana (S T Q Q S S D), com os dias liberados em destaque. A Velocidade aparece como _"≈ 120/h"_ (ou "Máximo"). O Progresso mostra a barra com _"128/300"_ e o percentual. **Clicar na linha abre os detalhes** da campanha.

Quando não há nada ainda: "Nenhuma campanha de disparo ainda", com o texto _"Crie uma campanha para enviar uma mensagem em massa para seus contatos por tag."_ Com busca sem resultado: "Nenhuma campanha encontrada".

## Criar uma campanha

Clique em **"Nova campanha"**. Abre o painel lateral "Nova campanha" (_"Configure o público, a mensagem e o agendamento do disparo."_) com quatro seções, uma abaixo da outra. Nesse caminho a campanha nasce em Rascunho e só envia quando você clicar em "Iniciar", na lista. O atalho do Funil é diferente e tem um aviso próprio, logo depois dos passos.

1. **Básico** — Preencha o "Nome da campanha" (_"Ex.: Promoção de Julho"_) e escolha a "Conexão" que fará os disparos (_"Escolha uma conexão"_). Cada conexão aparece com o selo "Web" (WhatsApp Web) ou "WABA" (API Oficial) e a bolinha de status.

   **Trocar a conexão depois limpa a mensagem já montada**, porque o formato muda entre os dois tipos.
2. **Quem recebe** — _"Escolha por tag, por coluna do funil ou por atendente principal. Quem casa com qualquer um dos critérios recebe."_ São três campos:

   - "Tags" (_"Adicionar tag"_);
   - "Colunas do funil" (_"Adicionar coluna"_; as colunas aparecem agrupadas pelo nome do funil);
   - "Atendente principal" (_"Adicionar atendente"_).

   É obrigatório escolher ao menos um. Não existe seleção manual de contatos nem importação de planilha aqui.

   O atendente principal é o campo do cadastro do contato (ver [Contatos](https://docs.convergefy.com.br/kb/contatos.md)), não quem está atendendo a conversa. A campanha vai para todos os contatos que têm um dos atendentes escolhidos como principal.

   Escolhendo coluna, aparece "Situação dos negócios" com os chips "Em aberto", "Ganho" e "Perda". Nada marcado: _"Nada marcado: a coluna inteira entra, em qualquer situação."_ Algo marcado: _"Só quem tem negócio nessa situação recebe."_
3. **O que enviar** — Depende do tipo da conexão. Veja "A mensagem, por tipo de conexão", mais abaixo.
4. **Dias e horários** — _"Adicione os dias em que a campanha pode disparar e as janelas de hora de cada um."_ Use "Adicionar horário": ele cria um bloco em que você marca os dias da semana e define o intervalo de horas. Deixar vazio é permitido: _"Sem dias configurados, a campanha envia a qualquer dia e horário. Adicione dias para restringir."_
5. **Velocidade e salvar** — Escolha a "Velocidade de envio" (veja abaixo) e clique em **"Salvar"**. A campanha nasce em Rascunho e ainda não envia nada até você mandar iniciar.

**Atendente principal e resumo do público**

O ícone de informação ao lado do campo "Atendente principal" lembra: _"Defina no cadastro de cada contato, na tela de Contatos."_ Depois de criada, o resumo da campanha lista cada critério do público numa frase só, por exemplo _"Recebem os contatos com essas tags e os contatos com esses atendentes principais."_ Só com atendentes principais, fica _"Recebem os contatos com esses atendentes principais."_

### Disparar direto de uma coluna do Funil

> **Pelo Funil, o disparo começa na hora**
>
> O atalho **"Disparar em massa"** do Funil não cria um rascunho: a campanha já começa a enviar assim que você confirma **"Disparar agora?"**. Dá para pausar depois, mas o que já saiu não volta. Confira o público e a mensagem antes de confirmar.

No [Funil](https://docs.convergefy.com.br/kb/funis.md), o menu (⋮) da coluna tem "Disparar em massa" (para quem tem o nível Operar em Disparo em massa). Abre "Disparar para {nome da coluna}" com o texto _"Vai para os negócios abertos desta coluna, sem os filtros da tela. Confira o público, escreva a mensagem e defina o ritmo. O disparo começa assim que você confirmar."_

O formulário já vem preenchido: nome sugerido, aquela coluna como público e a situação "Em aberto" marcada.

|                        | Pela lista ("Nova campanha")                                 | Pelo Funil ("Disparar em massa") |
| ---------------------- | ------------------------------------------------------------ | -------------------------------- |
| Botão final            | "Salvar"                                                     | "Disparar"                       |
| Confirmação            | "Iniciar disparo?" (ao clicar em "Iniciar" na lista, depois) | "Disparar agora?"                |
| Quando começa a enviar | Só depois de "Iniciar"                                       | Ao confirmar                     |
| Estado inicial         | Rascunho                                                     | Já enviando                      |

A confirmação do Funil diz: _"As mensagens começam a sair para o público escolhido, no ritmo configurado. Dá para pausar depois, mas o que já saiu não volta."_

> **Os horários são sempre de Brasília**
>
> A própria tela avisa: _"Os horários seguem o Horário de Brasília (GMT-3)."_ Se a sua operação está em outro fuso, converta antes de montar as janelas.

### A mensagem, por tipo de conexão

- **WhatsApp Web** — _"Componha a mensagem ou reaproveite uma mensagem rápida."_ Escreva em "Mensagem" (_"Escreva a mensagem. Use {{ ou o botão para inserir dados do contato"_), com opção de "Usar mensagem rápida" (traz o texto de um modelo salvo) e "Anexar mídia (opcional)". O texto da mensagem rápida é **copiado** para a campanha: editar o modelo depois não muda o que já foi montado.
- **API Oficial** — _"Conexões WABA disparam templates aprovados."_ Aparece o aviso _"Conexão WABA: o envio usa um template aprovado pela Meta."_ e o campo "Template" (_"Selecione um template aprovado"_), que lista **apenas templates aprovados**. Templates com cabeçalho de imagem, vídeo ou documento pedem também a "Mídia do cabeçalho". Se o template tiver variáveis, veja logo abaixo.

**Variáveis do template (API Oficial)**

Se o template tiver variáveis, a seção "Variáveis" pede o valor de cada uma: _"Ligue cada variável a um campo (cada destinatário recebe o valor dele) ou use um valor fixo."_ Alterne entre "Usar campo" (primeiro nome, sobrenome, nome completo, telefone, e-mail, documento, endereço) e "Usar fixo".

> **Por que a API Oficial exige template**
>
> Fora de uma conversa aberta, a Meta só entrega mensagem que a empresa inicia (proativa) em formato de template aprovado. Por isso a campanha na API Oficial não aceita texto livre. No WhatsApp Web não há essa exigência, mas o risco de bloqueio do número é maior. Veja [Conexões de WhatsApp](https://docs.convergefy.com.br/kb/conexoes.md).

### Velocidade de envio

- **Lento** — ≈ 30 por hora, ou 1 mensagem a cada 2 minutos. A tela diz _"≈ 120s entre envios"_.
- **Recomendado** — ≈ 60 por hora, ou 1 mensagem por minuto. A tela diz _"≈ 60s entre envios"_. É a opção que já vem marcada.
- **Médio** — ≈ 120 por hora, ou 1 mensagem a cada 30 segundos. A tela diz _"≈ 30s entre envios"_.
- **Rápido** — "Máximo", com o texto _"sem intervalo"_. Uma mensagem sai atrás da outra; é a configuração com maior risco de bloqueio do número.
- **Personalizado** — _"definir taxa"_: informe "Envios por hora (média)", de 1 a 3.600.

O próprio painel explica o comportamento: _"A taxa por hora é uma média: o valor real varia com a espera na fila. Os envios só ocorrem dentro das janelas configuradas; o que não sair no período continua na próxima janela."_

## Iniciar, pausar, cancelar

As ações ficam no fim de cada linha da lista e mudam conforme a situação da campanha:

| Situação                      | Ações disponíveis           |
| ----------------------------- | --------------------------- |
| Rascunho                      | Iniciar · Editar · Excluir  |
| Enviando                      | Pausar · Cancelar           |
| Pausada                       | Retomar · Editar · Cancelar |
| Finalizada, Cancelada, Falhou | Excluir                     |

Cada ação pede confirmação com o que vai acontecer:

- **Iniciar disparo?** — _"A campanha {nome} começará a enviar dentro dos dias e horários configurados."_ Se a conexão estiver fora do ar, o aviso é claro: _"A conexão {nome} está desconectada. A campanha inicia, mas fica pausada até a conexão voltar."_
- **Cancelar campanha?** — _"Os envios pendentes de {nome} serão cancelados. Os já disparados seguem o curso."_ Cancelar é **definitivo**: não existe "descancelar".
- **Excluir campanha?** — _"{nome} e o histórico de envios dela serão removidos."_

> **Quem cai fora sozinho**
>
> Se a conexão da campanha cair durante o envio, a campanha é pausada automaticamente. Ela **não volta sozinha** quando o número reconecta: depois de restabelecer a conexão, use "Retomar" na lista. Contatos sem telefone válido não recebem: entram como pulados, com o motivo _"Contato sem telefone válido."_

> **Campanha de uma conexão que você não acessa**
>
> Se a campanha usa uma conexão à qual o seu usuário não tem acesso (ver restrição de conexões em [Equipe e permissões](https://docs.convergefy.com.br/kb/equipe-permissoes.md)), ela continua na lista, mas só para leitura: no lugar dos botões da linha aparece um cadeado com a dica _"Esta campanha usa uma conexão que você não acessa."_, o painel de detalhes mostra o selo "Somente leitura" e some o rodapé com "Editar campanha" e "Excluir". Qualquer ação nela é recusada. Ao criar uma campanha, essas conexões também não aparecem no seletor "Conexão".

## Acompanhar uma campanha

Clique na linha para abrir o painel de detalhes. Ele mostra, de cima para baixo:

- **Progresso** — Os números "Enviados", "Falhas" e "Destinatários", a barra com _"150/150 processados"_ e a explicação _"Processados inclui enviados, falhas e contatos pulados."_ Numa campanha cancelada, a frase ganha _"Os N restantes foram cancelados antes do envio."_ Os cancelados **não** são contados como progresso.
- **Por que falhou** — A lista dos motivos das falhas, do mais frequente para o menos, com a quantidade de cada um (ex.: _"Número não encontrado no WhatsApp"_, _"Rate limit exceeded (429)"_).
- **Configuração, Dias e horários, Quem recebe, O que enviar** — Um resumo, só de leitura, do que foi configurado: as tags e as colunas do público (com a situação dos negócios, quando houver) e a mensagem/template usados. Coluna que foi apagada depois aparece como "Coluna removida".

Aparecem ainda "Iniciada em" e "Encerrada em". No rodapé ficam o botão "Editar campanha" (quando a situação permite) e o "Excluir" (que segue as mesmas regras de exclusão da lista).

**Por que alguns motivos de falha parecem técnicos**

Alguns motivos são técnicos porque são a resposta literal do provedor (ex.: _"cURL error 28: Operation timed out"_, que significa que o envio demorou demais e foi interrompido; e _"Rate limit exceeded (429)"_, que significa que o limite de envios foi atingido). Isso é proposital: esconder o texto atrapalharia o diagnóstico. Em campanhas com muitas falhas, a contagem é uma amostra: _"Contagem parcial: calculada sobre as 100 primeiras falhas de 130."_

## O que dá para mudar depois

- **Em Rascunho** — Tudo.
- **Pausada** — Só nome, dias e horários e velocidade. O painel avisa: _"A campanha já foi iniciada: conexão, público e mensagem estão congelados. Você ainda pode ajustar o nome, os dias e horários e a velocidade."_ Os campos travados aparecem marcados como "congelado", e a seção "Quem recebe" vira só leitura: _"Público definido na criação (não editável depois de iniciada)."_
- **Enviando, Finalizada, Cancelada, Falhou** — Nada: a campanha vira somente leitura.

Por quê: trocar público ou mensagem no meio de um disparo produziria uma campanha em que metade das pessoas recebeu uma coisa e metade outra, sem registro de qual foi qual. Para mudar a mensagem, **cancele** e crie outra campanha.

## Situação da campanha

**Legenda de status**

- **Rascunho** (gray) — criada, mas ainda não começou a enviar. Como resolver: use “Iniciar” quando estiver pronta.
- **Enviando** (blue) — armada e disparando dentro das janelas configuradas. Fora do horário permitido ela fica parada, mas continua nesta situação. Como resolver: acompanhe o progresso; use “Pausar” se precisar interromper.
- **Pausada** (amber) — interrompida por você ou automaticamente, porque a conexão caiu. Como resolver: use “Retomar” para voltar a enviar.
- **Finalizada** (green) — a lista inteira foi processada.
- **Cancelada** (red) — os envios pendentes foram descartados; os já disparados seguiram.
- **Falhou** (red) — não foi possível preparar a lista de destinatários; a campanha nem chegou a enviar. Como resolver: confira o público e a conexão, e crie a campanha de novo.

Os avisos rápidos (toasts) de cada ação são: _"Campanha criada com sucesso"_, _"Alterações salvas"_, _"Campanha excluída"_, _"Disparo iniciado"_, _"Campanha pausada"_, _"Campanha retomada"_ e _"Campanha cancelada"_.

Quando a campanha termina, você recebe uma notificação com o resumo (_"Campanha "{nome}" concluída"_, com o texto _"Total: N. Enviadas: N, falhas: N."_). Se a preparação da lista falhar, chega _"Campanha "{nome}" falhou"_, com o texto _"Não foi possível preparar a lista de envios. Tente novamente."_ (ver [Notificações](https://docs.convergefy.com.br/kb/notificacoes.md)).

## Erros e avisos esperados

Os quatro mais prováveis:

- “O template escolhido não foi encontrado ou não está aprovado.” — ao iniciar, o template escolhido já não está aprovado naquela conexão da API Oficial. Resolver: escolha outro template na lista; se ele existia, confira o status dele no painel da Meta.
- “A conexão escolhida foi removida, está desligada ou está incompleta.” — a conexão usada foi apagada, está desligada ou falta credencial da API Oficial. Resolver: reconfigure a conexão em Conexões ou crie a campanha de novo apontando uma conexão ativa.
- “Esta campanha já saiu do rascunho.” — você tentou iniciar uma campanha que já foi iniciada. Resolver: atualize a lista: a campanha já foi iniciada por outra pessoa.
- “Pause ou cancele a campanha antes de excluir.” — tentativa de excluir uma campanha que está enviando. Resolver: use “Pausar” ou “Cancelar” e só então exclua.

**Outros avisos, de público, mensagem e edição**

- “Escolha ao menos uma tag, coluna do funil ou atendente.” — a campanha ficou sem público. Resolver: escolha uma tag, uma coluna ou um atendente principal em “Quem recebe”.
- “Escolha ao menos uma tag, coluna do funil ou contato.” — ao iniciar a campanha, o público ficou vazio, por exemplo porque uma tag ou coluna foi apagada entre montar e disparar. Resolver: volte ao público e escolha de novo antes de disparar.
- “Escreva a mensagem da campanha.” — ao iniciar, a campanha está sem mensagem. Resolver: volte à campanha e preencha o texto da mensagem.
- “Escolha uma mensagem rápida.” — a campanha aponta para uma mensagem rápida que não está mais escolhida. Resolver: selecione a mensagem rápida ou escreva o texto à mão.
- “Só dá para pausar uma campanha que está enviando.” — a campanha não está em “Enviando”. Resolver: confira a situação da campanha na lista.
- “Só dá para retomar uma campanha pausada.” — a campanha não está em “Pausada”. Resolver: confira a situação da campanha na lista.
- “Esta campanha já foi encerrada.” — você tentou cancelar uma campanha que já terminou. Resolver: campanha cancelada ou finalizada não volta a enviar; crie outra se precisar.
- “A campanha só pode ser editada em rascunho ou pausada.” — você tentou salvar uma campanha que mudou de situação com o painel aberto. Resolver: só campanhas em Rascunho ou Pausada aceitam edição.
- “Com a campanha pausada, só dá para mudar nome, dias, horários e velocidade.” — edição de um campo congelado numa campanha pausada. Resolver: ajuste apenas nome, dias/horários e velocidade; para mudar público ou mensagem, cancele e crie outra.
- “O fim deve ser após o início.” — janela de horário invertida. Resolver: corrija o intervalo de horas do dia.
- “Não foi possível enviar o arquivo.” — falha ao subir a mídia da mensagem ou do cabeçalho. Resolver: tente anexar de novo; confira o tamanho e o formato aceitos pelo template.
