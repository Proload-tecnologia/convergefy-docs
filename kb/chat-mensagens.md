# Atendimento / Chat: Enviar mensagens

Tudo o que acontece na caixa de digitação e depois do envio: texto, mídia, áudio, notas internas, agendamento, transferência e o status de cada mensagem.

Na Central de Ajuda: https://docs.convergefy.com.br/#/chat-mensagens

## Em resumo

Esta página cobre o que acontece na caixa de digitação do Chat e depois do envio: texto, mídia, áudio, notas internas, agendamento, transferência e o status de cada mensagem. O resto do Chat está em [Atendimento / Chat](https://docs.convergefy.com.br/kb/chat.md).

Algumas regras mudam conforme o tipo de conexão: WhatsApp Web (liga por QR Code) ou API Oficial (o WhatsApp Business da Meta, também chamado WABA). Template é uma mensagem-modelo aprovada pela Meta e só existe na API Oficial. Veja [Conexões](https://docs.convergefy.com.br/kb/conexoes.md).

### Algo deu errado?

Procure o que você está vendo e siga a coluna da direita. O detalhe de cada caso está mais abaixo.

| O que você vê                                                                           | O que fazer                                                                                                                                                                                           |
| --------------------------------------------------------------------------------------- | ----------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------- |
| "Falha ao enviar" no balão (vermelho)                                                   | O navegador não conseguiu mandar a mensagem para a Convergefy, em geral por internet instável, e ela nem chegou a sair. Clique em "Tentar novamente"; se persistir, confira sua internet.             |
| "Não foi possível enviar" no balão (vermelho, às vezes sublinhado)                      | A mensagem chegou à Convergefy, mas o WhatsApp não a entregou. Clique no texto para ver o motivo, resolva o que ele indica e use "Tentar novamente", quando aparecer.                                 |
| Falha sem o botão "Tentar novamente"                                                    | Reenviar não adianta: conta do WhatsApp restrita, contato que bloqueou o número ou envio não autorizado.                                                                                              |
| Aviso "Fora da janela de 24 h: o WhatsApp só entrega template até o contato responder." | Na API Oficial, só um template aprovado pela Meta reabre a conversa. Use o botão "Enviar template".                                                                                                   |
| "A conexão desta conversa não está pronta para enviar."                                 | Confira em Conexões se o número está conectado; reconecte se preciso e reenvie.                                                                                                                       |
| "Selecione uma conexão para enviar a mensagem."                                         | Escolha o número no seletor de conexão do cabeçalho.                                                                                                                                                  |
| "O arquivo anexado não está mais disponível. Anexe de novo."                            | Anexe o arquivo outra vez e reenvie.                                                                                                                                                                  |
| "Anexos não são suportados no modo nota interna."                                       | Saia do modo nota interna para enviar arquivos.                                                                                                                                                       |
| Aviso de que não deu para editar ou apagar agora                                        | A mensagem pode ainda estar sendo enviada, a conexão pode estar fora do ar ou o prazo passou (15 minutos para editar, cerca de dois dias para apagar). Espere a mensagem ser enviada e tente de novo. |
| Editar ou Excluir não aparecem no menu da mensagem                                      | Fora das janelas de 15 minutos (editar) e 48 horas (excluir), o item não aparece.                                                                                                                     |
| Um destino marcado com falha ao encaminhar                                              | Os outros destinos não são afetados. Veja o motivo marcado na janela, que continua aberta para tentar de novo.                                                                                        |

### Enviar uma mensagem em quatro passos

1. **Abrir a conversa** — Abra a conversa no Chat. Em conexão API Oficial, olhe a linha da janela de atendimento acima da caixa (ver "Limites e regras").
2. **Escrever** — Digite no campo _"Mensagem ou / para atalhos"_. Se quiser, anexe arquivos em **Anexar arquivo**.
3. **Enviar** — No computador, aperte Enter. No celular, Enter quebra a linha: use o botão **"Enviar mensagem"**.
4. **Conferir o status** — Veja o ícone no balão. Se falhar, use a tabela acima.

## Enviar mensagens (a caixa de digitação)

O campo mostra _"Mensagem ou / para atalhos"_. Em nota interna: _"Digite uma nota interna..."_. Ao editar: _"Edite a mensagem..."_. Com arquivo anexado, o campo de legenda diz _"Legenda (opcional)..."_. No computador, Enter envia e Shift+Enter quebra a linha; no celular, Enter quebra a linha.

O botão da ponta direita muda:

- campo vazio: o microfone "Gravar áudio";
- texto ou anexo pronto: "Enviar mensagem";
- ao editar: o ✓ "Salvar edição".

Digite "/" no início para abrir mensagens rápidas, templates e automações manuais (ver [Mensagens rápidas](https://docs.convergefy.com.br/kb/mensagens-rapidas.md)).

**Botões da barra de digitação**

- **Emojis** — Insere emojis no texto.
- **Gravar áudio** — Grava a voz na hora. Não importa arquivo: para enviar áudio já gravado, use Anexar → Áudios. Não existe em nota interna.
- **Anexar arquivo** — Menu com Documento, Imagens/Vídeos, Áudios e Contato (envia um cartão de contato). Os três primeiros já filtram os formatos aceitos. Desativado em nota interna. Dá para escolher vários arquivos de uma vez (veja abaixo).
- **Mensagens rápidas** — Modelos de texto prontos (ver [Mensagens rápidas](https://docs.convergefy.com.br/kb/mensagens-rapidas.md): atalho "/", favoritas e variáveis do contato).
- **Automações manuais** — Dispara uma automação à mão para aquele contato.
- **Modo nota interna** — Alterna para registrar uma nota só da equipe.
- **Agendar mensagem** — Programa um envio para o futuro.

**Anexar vários arquivos de uma vez**

Dá para escolher até 10 arquivos, que vão para uma bandeja acima do campo (_"{N} de 10"_) com legenda por arquivo (_"Legenda (opcional)..."_) e um × para tirar cada um.

O WhatsApp não junta tipos diferentes numa mensagem só (imagem com PDF, áudio com PDF): cada arquivo vai como uma mensagem. Áudio não tem legenda: a bandeja avisa _"Áudio é enviado sem legenda."_

> **Mensagens com botões: quem envia é a automação**
>
> A caixa de digitação não monta mensagens com botões ou lista. Isso é feito nas [Automações](https://docs.convergefy.com.br/kb/automacoes.md) (botões no passo de texto e passo Menu interativo, só em conexões WhatsApp Web).
>
> Na conversa, elas aparecem com o desenho de botões:
>
> - o botão de link abre o endereço;
> - o de código copia o código;
> - o de resposta rápida só o contato toca;
> - o de ligação não completa a chamada daqui.
>
> Quando o cliente toca num botão ou linha da lista (inclusive nos botões de resposta rápida de um template da API Oficial), entra uma mensagem de texto normal com o rótulo do botão (ex.: _"Falar com atendente"_). Quem ramifica pela escolha é a automação.

**Enviar e receber contatos (cartão de contato)**

Para enviar, abra Anexar → Contato, que abre "Enviar contato" (_"Escolha quem você quer enviar como cartão de contato."_). Busque em _"Buscar contato..."_, marque um ou vários e clique em "Enviar 1 contato" / "Enviar {N} contatos". "Incluir e-mail" e "Incluir endereço" valem para todos os marcados. Contato sem telefone aparece com "Sem telefone" e não dá para marcar. Cabem até 257 contatos por mensagem. Na API Oficial, a foto do contato não vai no cartão.

Para receber: o contato que o cliente manda aparece como um cartão com o nome. O botão "Conversar" cadastra a pessoa (se ainda não existir) e abre a conversa com ela; exige o nível Editar na área Contatos, e sem ele o botão some. Se o cartão tem vários contatos, o botão é "Ver todos os {N} contatos", que abre "Mostrar contato" com um "Conversar" para cada um. Cartão cujo número não tem WhatsApp mostra "Sem WhatsApp" e não oferece "Conversar".

**Enviar um template (API Oficial) com cabeçalho de mídia**

Se o cabeçalho do template for imagem, vídeo ou documento, o formulário mostra "Imagem do cabeçalho", "Vídeo do cabeçalho" ou "Documento do cabeçalho" para anexar o arquivo (o seletor já filtra o formato; o cabeçalho não tem legenda). Enquanto sobe: "Enviando…". Acima do limite: "Arquivo excede o limite de {limite}."

Não saem pela plataforma: cabeçalho de localização (_"Cabeçalho de localização ainda não é suportado no envio. Escolha outro template."_) e templates de autenticação (_"Templates de autenticação ainda não podem ser enviados pela plataforma."_).

**Cada mensagem tem um menu ('Ações da mensagem')**

Para abrir o menu, passe o mouse sobre a mensagem e clique na setinha do canto do balão ("Ações da mensagem"), ou clique com o botão direito no balão. A setinha some enquanto você arrasta para selecionar texto. O botão direito dentro de um texto selecionado abre o menu normal do navegador, para copiar.

Opções:

- "Responder": cita a mensagem. Mostra a prévia (com miniatura se for mídia) e "Cancelar resposta". Clicar na citação leva à mensagem original.
- "Encaminhar".
- "Copiar": texto ou legenda; em imagem, a própria imagem. Avisa "Mensagem copiada" (ou "Não foi possível copiar a mensagem"). Vídeo não tem "Copiar".
- "Baixar", só em mídia.
- "Editar" e "Excluir", nas mensagens que você enviou.

Clicar numa imagem ou vídeo abre o visualizador de mídia, com baixar, legenda e as mesmas ações.

> **Excluir apaga também no WhatsApp do cliente**
>
> A janela "Excluir mensagem?" avisa: _"A mensagem também será apagada no WhatsApp do cliente. Não é possível desfazer."_

**Editar e excluir uma mensagem enviada**

Só valem para mensagens que você enviou por uma conexão WhatsApp Web, já confirmadas pelo WhatsApp e ainda não apagadas.

- "Editar": só nos primeiros 15 minutos e só em texto ou mídia com legenda (áudio e mídia sem legenda não editam). Salve com o ✓ "Salvar edição"; o balão mostra "Editada".
- "Excluir": vale por 48 horas. Abre "Excluir mensagem?" (veja o aviso acima). Depois o balão fica como "Mensagem excluída".

Fora dessas janelas, o item não aparece no menu.

> **Mensagens excluídas no WhatsApp**
>
> Quando alguém apaga uma mensagem (o cliente ou o atendente), o balão fica esmaecido com o rótulo "Mensagem excluída" e um ícone de proibido. Não dá para responder, citar nem encaminhar uma mensagem excluída.

## Notas internas

Uma **nota interna** é um recado da equipe para a equipe, dentro da conversa. O cliente nunca a vê. Registra contexto para o próximo atendente (ex.: _"Cliente prefere ser chamado de João"_, _"Pediu retorno só depois das 18h"_), que assim entende a situação sem perguntar de novo ao cliente.

1. **Ativar o modo** — Ligue o **"Modo nota interna"**. Aparece o banner "Modo Nota Interna" (com um × para sair) e o campo muda para _"Digite uma nota interna..."_.
2. **Escrever e salvar** — A nota fica registrada em amarelo, com o rótulo "Nota Interna" (autor e horário). A seção "Notas internas" do painel direito reúne todas.

Nota aceita só texto (_"Anexos não são suportados no modo nota interna."_), não vai ao cliente e não muda o status do atendimento.

## Mensagens rápidas e automações manuais

**Mensagens rápidas no chat**

O botão "Mensagens rápidas" (ícone de raio) abre uma lista única: Favoritos no topo, Todas abaixo, com busca (_"Buscar..."_). Vazio: "Nenhuma mensagem rápida." / "Nenhum resultado." Ver [Mensagens rápidas](https://docs.convergefy.com.br/kb/mensagens-rapidas.md).

**Automações manuais no chat**

O botão "Automações manuais" lista as automações ativas com gatilho de Execução manual (busca _"Buscar automação..."_, seções "Favoritos" e "Todas"; "Todas" só aparece quando há favoritas e não favoritas). Ao escolher uma, abre "Iniciar automação?"; confirme em "Iniciar". Vazio: "Nenhuma automação com execução manual ativa." / "Nenhuma automação encontrada."

- Sucesso: "Automação iniciada com sucesso".
- Erros: "Esta automação não está ativa." (ative a automação antes) ou "Não foi possível executar a automação."

## Ouvir áudios

Só **um áudio toca por vez** em toda a tela: começar outro pausa o anterior, mesmo de outra conversa.

Se você sair da conversa com o áudio tocando, ele continua e aparece um mini player: no rodapé da lista no computador, no topo da tela no celular. Mostra avatar e nome da conversa (ou do grupo) de onde o áudio veio, não de quem gravou, com pausar/retomar, "Fechar áudio" e uma barra de progresso. Clicar no nome leva à conversa, e a bolha do áudio pisca. Com a conversa do áudio aberta não há mini player: o próprio balão controla.

A velocidade (1,0×, 1,5×, 2,0×, 2,5×, 3,0×) é preferência do seu navegador e vale para todos os áudios.

> **No chat aberto por outra tela não há mini player**
>
> Quando o chat abre num painel lateral (a partir do Funil, por exemplo), fechar o painel para o áudio, e não há mini player.

## Agendar mensagem

1. **Abrir** — Clique em **Agendar mensagem**. Abre "Agendar mensagem" (ou "Editar agendamento" ao editar).
2. **Definir quando enviar** — Em "Quando enviar", escolha data e horário (_"Selecione data e horário"_). Precisa ser no futuro e em até 365 dias.
3. **Escolher o que enviar** — Em "O que enviar", escreva a mensagem (_"Mensagem ou / para atalhos"_). É o mesmo editor do chat: aceita anexo (com legenda) e o atalho "/". Em conexão da API Oficial aparece também o seletor "Mensagem" / "Template", para agendar um template aprovado.
4. **Confirmar** — Clique em **"Agendar envio"** (ou **"Salvar alterações"**).

**Onde ficam e como gerenciar os agendamentos**

Os agendamentos pendentes ficam no painel "Agendamentos" (à direita) e também como balões no fim da conversa. Cada um tem "Editar mensagem agendada" (ou "Editar template agendado") e "Excluir mensagem agendada".

Na API Oficial, se a janela de 24 h estiver fechada ou fechar antes do horário marcado, a janela avisa que a mensagem só chega se o contato responder antes. O botão "Usar um template" troca para template (ver "Limites e regras").

- Sucesso: "Agendamento salvo para \[data/hora].", "Agendamento atualizado.", "Agendamento excluído."
- Erros: "Não foi possível salvar o agendamento." (também "atualizar" e "excluir") e "Escolha uma data e horário futuros" (data no passado).

## Transferir e encaminhar

Transferir passa o atendimento inteiro a outra pessoa. Encaminhar copia mensagens para outro contato.

> **Antes de transferir ou encaminhar**
>
> - Transferir: se você não pode ver todas as conversas e transferiu para outra pessoa (ou só para um departamento), a conversa fecha para você. Ela deixou de ser sua.
> - Encaminhar assume o atendimento, como qualquer envio: conversa em Aguardando passa para você e finalizada é reaberta. A que já está em atendimento continua com quem atende.

**Transferir o atendimento**

No cabeçalho, clique em **"Transferir"**. Abre "Transferir para": escolha "Selecione departamento" e/ou "Selecione atendente" e clique em "Transferir". A conversa vai para Aguardando do destino. Se você escolher só um departamento com distribuição automática, o sistema já pode escolher um atendente dele.

**Encaminhar mensagens (até 10)**

No menu "Ações da mensagem" escolha "Encaminhar".

- Entra o modo de seleção: barra no topo (_"X de 10 selecionada(s)"_) e uma caixinha em cada mensagem. Marque até 10; o × (_"Cancelar seleção"_) sai do modo.
- Clique em "Encaminhar". Em "Encaminhar {N} mensagem(ns)", busque o destino (_"Buscar conversa ou contato..."_), até 10 destinos.
- Para destinos sem conexão definida aparece o seletor "Enviar por" (_"Selecione a conexão"_).
- Vazio: "Nenhuma conversa recente" / "Nenhuma conversa ou contato encontrado".

O que acontece no envio:

- Conversa em andamento sai pela conexão dela. O seletor vale para contatos sem conversa e conversas sem conexão disponível.
- Contato sem conversa ganha uma nova na conexão escolhida, com você como responsável.
- Mídia reusa o arquivo guardado no sistema. Mensagens cujo arquivo não está mais disponível ficam de fora; o restante segue.
- Um destino com falha não impede os outros. Quem falhou fica marcado na janela com o motivo (_"Você não tem acesso a esta conversa"_, _"Conexão indisponível para este envio"_, _"Não foi possível abrir a conversa"_ ou _"Não foi possível enviar"_), e a janela continua aberta para tentar de novo. Nesse destino, as mensagens que faltavam também não saem.

## Status de envio no balão

**O que cada estado da mensagem significa**

- **Enviando** (blue) — a mensagem está saindo (relógio ou ícone girando).
- **Falha ao enviar** (red) — o seu navegador não conseguiu mandar a mensagem para a Convergefy (em geral internet instável). Ela nem chegou a sair. Como resolver: clique em Tentar novamente; se persistir, confira sua internet.
- **Não foi possível enviar** (red) — a mensagem chegou à Convergefy, mas o WhatsApp não a entregou. Como resolver: clique no texto para ver o motivo; resolva o que ele indica e use Tentar novamente, quando aparecer.

Quando o WhatsApp informa por que não entregou, "Não foi possível enviar" fica sublinhado e clicável. Abre "Falha no envio" com:

- **Código** — o código de erro do WhatsApp (só quando existe).
- **Motivo** — a explicação em português, para os erros mais comuns. Nos outros, o texto original do WhatsApp, que costuma vir em inglês.
- **Quando** — data e hora da falha.
- **Detalhes técnicos** — a resposta completa do WhatsApp, com botão de copiar. Útil para mandar ao suporte.

* Vale para a falha na hora do envio (número sem WhatsApp, mensagem recusada pela Meta) e para a que o WhatsApp avisa depois (janela de 24h fechada na API Oficial). Algumas falhas não trazem motivo, como conexão fora do ar por muito tempo: o texto aparece sem sublinhado.
* Em mensagens de template (API Oficial), a falha aparece só como "Falha no envio", sem detalhes e sem "Tentar novamente".
* "Tentar novamente" aparece embaixo da falha. Não aparece quando reenviar não adianta: conta do WhatsApp restrita, contato que bloqueou o número ou envio não autorizado.
* Por que falha: em geral a conexão está caída (WhatsApp Web desconectado), o número não tem WhatsApp ou, na API Oficial, a janela de atendimento fechou ou o status da conexão bloqueia o envio (ver [Conexões](https://docs.convergefy.com.br/kb/conexoes.md)).

## Tempo real e o "digitando..."

Mensagens novas, contagens e a bolinha de status da conexão atualizam sozinhas, sem recarregar. Detalhes em [Tempo real](https://docs.convergefy.com.br/kb/tempo-real.md) e [Notificações](https://docs.convergefy.com.br/kb/notificacoes.md).

> **Aviso de sincronização de histórico**
>
> Coexistência é quando o número da API Oficial já vinha sendo usado no WhatsApp Business App. Quando uma conexão em coexistência importa o histórico do WhatsApp, o topo do Chat mostra "Sincronizando histórico" (depois, "Sincronização de histórico"), com barra e percentual por conexão. Só vê quem tem o nível Administrar na área Conexões, ou administrador. Ao terminar: "Histórico concluído". Se o cliente recusar: "Cliente recusou compartilhar o histórico" (fecha no ×). As conversas antigas entram sozinhas, já finalizadas. Detalhes em [Conexões](https://docs.convergefy.com.br/kb/conexoes.md).

> **Sobre o 'digitando.../gravando áudio...'**
>
> O cliente vê _"digitando…"_ / _"gravando áudio…"_ no WhatsApp dele quando você digita ou grava áudio numa conversa de conexão WhatsApp Web, e quando uma automação envia (toggle "Mostrar digitando" num passo de mensagem; ver [Automações](https://docs.convergefy.com.br/kb/automacoes.md)). Nota interna não emite o aviso, e a API Oficial também não. O contrário não existe: a Convergefy não mostra "o cliente está digitando" ao atendente.

## Etiquetas e recibos no balão

**Quem enviou, formulário de anúncio e recibos**

- Etiqueta de origem: além do nome do atendente, o balão pode mostrar quem enviou de fato: "Agente de IA" (um [agente de IA](https://docs.convergefy.com.br/kb/agentes-ia.md) dentro de uma automação), "Agendada", "Disparo em massa", "API", "Celular" (enviada pelo aparelho, em conexão de coexistência), "Sistema" ou "Automação" com o nome da automação. Na lista, o card mostra o ícone da origem da última mensagem.
- Resposta de formulário de anúncio: aparece como um cartão no meio da conversa, no momento em que o contato enviou o formulário.
- Recibos: ✓ enviado, ✓✓ entregue, ✓✓ azul lido. Em áudio, "Áudio escutado". Em grupo ficam escondidos.
- Histórico longo: a conversa carrega aos poucos. Ao subir para ver mensagens antigas, aparece "Ir para as mensagens mais recentes".
- Conexão sem acesso: as mensagens aparecem como "Conteúdo restrito", a conexão aparece no seletor como "Sem acesso" (_"Você não tem acesso a esta conexão"_) e a caixa de digitação fica bloqueada.

## Limites e regras

**Limites de tamanho, formato e a janela de 24h (API Oficial)**

- Texto: até 4096 caracteres, ou 1024 quando é legenda de anexo. Mensagem agendada: 2000.
- Anexos: até 100 MB cada, em lotes de até 10 arquivos. Formatos: imagens (jpg, png, gif, webp), vídeo (mp4, 3gpp), áudio (ogg, webm, mp3, m4a, aac) e documentos (pdf, doc, docx, xls, xlsx, ppt, pptx, txt e, só em WhatsApp Web, zip e csv). Na API Oficial o WhatsApp aplica tetos menores por tipo (abaixo).
- Tetos da API Oficial: a Meta recusa acima de 5 MB para imagem, 16 MB para vídeo, 16 MB para áudio e 100 MB para documento. Para reduzir recusas, a plataforma ajusta o arquivo sozinha:

  - JPEG e PNG acima de 5 MB são reduzidos;
  - GIF vira MP4;
  - áudio fora dos formatos aceitos vira OGG/Opus.

  Se a conversão falhar, a mensagem sai com _"Não foi possível converter o anexo para um formato aceito pela WABA."_ Vídeo e documento acima do teto não são reduzidos: o envio é aceito e a Meta recusa na entrega. Comprima antes.
- Nota interna: só texto, sem anexo.
- Agendamento: data e hora futuras, em até 365 dias.
- Template: só em conexão da API Oficial. O WhatsApp só permite mensagem livre até 24 horas depois da última mensagem do cliente. Passada a janela, só um template aprovado pela Meta reabre a conversa.
- Aviso da janela (API Oficial): com uma conexão da API Oficial escolhida, uma linha acima da caixa de mensagem mostra a janela daquela conexão:

  - _"Janela de atendimento aberta até 15:30."_
  - Na última hora, em âmbar: _"A janela de atendimento fecha em 20 min."_
  - Se vai até o dia seguinte: _"Janela de atendimento aberta até amanhã, 15:30."_
  - Fechada: _"Fora da janela de 24 h: o WhatsApp só entrega template até o contato responder."_, com o botão "Enviar template".

  A janela é por conexão: se a conversa escolhe a linha de envio, trocar de conexão troca o aviso. Mensagem do histórico importado na coexistência não abre janela. O aviso só informa; se a mensagem sair fora da janela, a falha aparece no balão.

## Erros e avisos esperados

**Ao iniciar conversa ou criar contato**

- “Telefone é obrigatório.” — faltou o número. Resolver: informe o telefone do contato.
- “Telefone inválido. Verifique o número informado.” — o número não é válido. Resolver: confira DDD e dígitos.
- “Selecione uma conexão para iniciar a conversa.” — faltou a conexão. Resolver: escolha por qual número iniciar.
- “Não foi possível criar o contato.” — falha ao cadastrar o lead. Resolver: revise nome, telefone e e-mail e tente de novo.
- “Não foi possível iniciar a conversa.” — falha genérica ao abrir a conversa. Resolver: tente de novo; se persistir, recarregue a página.

**Ao enviar uma mensagem**

- “Selecione uma conexão para enviar a mensagem.” — faltou a conexão (ao encaminhar, a frase termina em 'para encaminhar'). Resolver: escolha o número no seletor de conexão do cabeçalho.
- “Este contato não tem um telefone válido para WhatsApp.” — o contato está sem número utilizável. Resolver: edite o contato e cadastre um telefone válido.
- “A conexão desta conversa não está pronta para enviar.” — a conexão foi removida, está desligada ou fora do ar (WhatsApp Web caído, ou número da API Oficial desconectado na Meta). Resolver: confira em Conexões se o número está conectado; reconecte se preciso e reenvie.
- “A mensagem respondida não está mais disponível.” — a mensagem citada não pode mais ser usada (por exemplo, ainda não foi confirmada pelo WhatsApp). Resolver: envie de novo sem citar, ou cite outra mensagem.
- “O arquivo anexado não está mais disponível. Anexe de novo.” — o anexo ainda está sendo processado ou expirou. Resolver: anexe o arquivo outra vez e reenvie.
- “Não foi possível enviar a mensagem.” — falha genérica no envio. Resolver: tente de novo; se persistir, confira a conexão e o contato.
- “Anexos não são suportados no modo nota interna.” — tentou anexar numa nota. Resolver: saia do modo nota interna para enviar arquivos.

**Ao anexar arquivos**

- “O arquivo "{nome}" excede o limite de 100 MB.” — o anexo passou do tamanho. Os outros arquivos do lote seguem. Resolver: reduza ou comprima o arquivo.
- “O arquivo "{nome}" não é um tipo aceito.” — tipo de arquivo não suportado. Resolver: use um formato aceito (ver Limites e regras).
- “A API oficial do WhatsApp não aceita "{nome}" como documento.” — a conversa é da API Oficial e a Meta não aceita esse documento (por exemplo ZIP ou CSV). Resolver: envie por uma conexão WhatsApp Web ou converta para PDF, DOC, XLS, PPT ou TXT.

**Ao editar, apagar, encaminhar ou carregar**

- “Não deu para editar agora. A mensagem pode ainda estar sendo enviada, a conexão pode estar fora do ar ou o prazo de 15 minutos já passou.” — a edição foi recusada. Resolver: espere a mensagem ser enviada e tente de novo; passados 15 minutos, não dá mais para editar.
- “Não deu para apagar agora. A mensagem pode ainda estar sendo enviada, a conexão pode estar fora do ar ou o prazo de cerca de dois dias já passou.” — a exclusão foi recusada. Resolver: espere a mensagem ser enviada e tente de novo; passado o prazo, não dá mais para apagar para todos.
- “Não foi possível encaminhar as mensagens.” — falha ao encaminhar. Resolver: confira o destino e a conexão e tente de novo.
- “Não foi possível carregar a conversa.” — falha ao abrir a conversa pelo cartão do Funil ou pelo painel de Rastreamento. Resolver: tente abrir de novo; se persistir, recarregue a página.

> **Templates da API Oficial e automações**
>
> Mensagens de template (API Oficial) têm avisos próprios, entre outros (ver [Erros e avisos comuns](https://docs.convergefy.com.br/kb/erros-comuns.md)):
>
> - _"Este template não pode ser enviado para este contato agora. Confira se ele está aprovado."_
> - _"Preencha todas as variáveis do template."_
> - _"Preencha o valor dos botões do template."_
> - _"A Meta recusou o arquivo do cabeçalho. Confira o arquivo escolhido."_
> - _"Este template usa um recurso que a Convergefy ainda não envia."_
>
> As automações também já enviam templates pela API Oficial (ver [Automações](https://docs.convergefy.com.br/kb/automacoes.md)).
