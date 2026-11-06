# Erros e avisos comuns

Catálogo das mensagens que você pode ver na tela, agrupadas por área. Para cada uma, o que significa e como resolver. Se a sua mensagem não estiver aqui, procure o suporte em vez de adivinhar.

Na Central de Ajuda: https://docs.convergefy.com.br/#/erros-comuns

## Em resumo

Catálogo das mensagens que aparecem na tela: o que cada uma significa e o que fazer. Estão agrupadas pela área onde aparecem (Conexões, Chat, Funis, etc.).

> **Como achar sua mensagem**
>
> Veja em qual tela o erro apareceu (Chat, Conexão, Funil, Contato, Automação) e vá à seção dela. As mensagens de sessão, internet e servidor podem aparecer em qualquer tela e estão na primeira seção, logo abaixo.

> **Regra geral antes de tudo**
>
> Muitas falhas são um pré-requisito faltando: uma conexão ativa, um campo obrigatório vazio ou falta de permissão de acesso ao atendimento. Para falhas de envio, suspeite primeiro da conexão (ver [Conexões](https://docs.convergefy.com.br/kb/conexoes.md)).

**Palavras que aparecem neste guia**

- **API Oficial** — O WhatsApp Business da Meta, também chamado WABA. Conexão oficial, diferente do WhatsApp Web (que liga por QR Code).
- **Template** — Modelo de mensagem aprovado pela Meta, usado só em conexões da API Oficial.
- **Janela de 24h** — O WhatsApp só permite mensagem livre até 24 horas depois da última mensagem do cliente. Passado esse prazo, só um template aprovado chega.
- **Gatilho** — O evento que inicia uma automação. Uma automação pode ter vários.
- **Bloco e saída** — Bloco é cada caixa do quadro da automação. Saída é o ponto de onde sai uma ligação; blocos que decidem ou esperam têm várias (ex.: "Tempo esgotado").

## Mensagens globais do sistema (sessão e rede)

Avisos que podem aparecer em qualquer tela, ligados à sua sessão ou à conexão de internet.

- “Sessão expirada, por favor faça login novamente.” — você ficou muito tempo inativo ou a sessão caiu. Resolver: entre de novo na plataforma (ver Conta e acesso). Você foi levado de volta para o login.
- “Sem conexão com o servidor. Verifique sua internet.” — o navegador não conseguiu falar com a Convergefy. Resolver: confira sua rede e tente de novo.
- “Erro interno do servidor, tente novamente mais tarde.” — algo falhou no servidor. Resolver: aguarde alguns instantes e tente de novo. É falha temporária no servidor.
- “Muitas tentativas seguidas. Aguarde um instante.” — você repetiu a ação rápido demais. Resolver: espere alguns segundos antes de repetir a ação.
- “Você não tem permissão para fazer isso.” — seu acesso não inclui essa ação. No Chat, em geral é porque o atendimento pertence a outro atendente. Quando a conversa abre no lugar da tela normal, o título é _"{nome} é responsável por essa conversa"_ (ou _"Esta conversa está restrita"_), com o recado _"Peça a transferência para continuar esse atendimento."_ Resolver: no Chat, peça a transferência do atendimento ao atendente responsável, ou a quem pode ver todas as conversas. Em qualquer outra área, peça a quem administra a empresa para liberar o acesso à área em questão.
- “Não encontramos este item. Ele pode ter sido excluído.” — o registro que você tentou abrir ou mudar não existe mais. Resolver: atualize a página. Se o item sumiu, alguém o excluiu.
- “Não foi possível carregar as informações.” — aviso genérico quando uma lista ou tela não carrega. Resolver: recarregue a página; se persistir, procure o suporte.
- “Não foi possível concluir a ação.” — aviso genérico quando uma ação falha sem um motivo específico. Resolver: tente de novo; se persistir, procure o suporte.

Algumas situações não mostram um aviso: levam você a outra tela.

- Confirmação de e-mail: o seu e-mail ainda não foi confirmado. Confirme pelo link enviado para o seu e-mail para liberar a plataforma (ver [Conta e acesso](https://docs.convergefy.com.br/kb/conta-acesso.md)).
- Escolha de empresa: sua conta não tem empresa selecionada. Escolha ou crie uma empresa para continuar.
- Tela de assinatura: a assinatura ou o período de experiência terminou e o acesso foi bloqueado. Quem administra a empresa precisa renovar a assinatura (ver [Cobrança](https://docs.convergefy.com.br/kb/cobranca.md)).

> A maioria desses avisos aparece como toast, um cartãozinho no canto da tela, e some sozinho depois de alguns segundos.

## Conexões

- “Status Desconectado (WhatsApp Web)” — a sessão caiu: celular sem internet ou aparelho desconectado. Resolver: reconecte lendo o QR Code de novo (verifique se o celular está com internet).
- “Status laranja ou vermelho na API Oficial (Reportada, Qualidade Baixa, Restringida, Banida…)” — problema na conta da Meta que bloqueia o envio: qualidade, limite ou política. Resolver: resolva na conta Meta / WhatsApp Manager. Não é falha da Convergefy.
- “Não foi possível sincronizar o status.” — falha ao atualizar o status da conexão. Resolver: use “Sincronizar status” de novo (no menu ⋮ do card da API Oficial, o item se chama “Sincronizar”). Se travar, recarregue a página.
- “Erro ao carregar conexões” — a lista de conexões não carregou. O subtexto é _"Ocorreu um problema ao listar as conexões. Tente novamente."_ Resolver: use “Tentar novamente” logo abaixo do aviso. É instabilidade momentânea ao carregar a lista.
- “{nome da conexão} · removida” — (no Chat) a conexão daquela conversa não existe mais e o envio fica bloqueado. Resolver: em empresas com mais de uma conexão, escolha outra na própria conversa. Com conexão única, recadastre o número.

> A lista completa de cada status (bolinha colorida) do WhatsApp Web e da API Oficial está no guia de [Conexões](https://docs.convergefy.com.br/kb/conexoes.md).

## Chat

Duas mensagens que você pode procurar aqui estão em outras seções: “Você não tem permissão para fazer isso.” (em Mensagens globais) e “Não foi possível criar o contato.” (em Contatos).

### Iniciar uma conversa

- “Telefone é obrigatório.” — o número está faltando. Resolver: informe o número do contato.
- “Telefone inválido. Verifique o número informado.” — o número está em formato errado. Resolver: corrija o formato do número (DDD + número).
- “Selecione uma conexão para iniciar a conversa.” — falta escolher a conexão. Resolver: escolha uma conexão ativa antes de iniciar.
- “Não foi possível iniciar a conversa.” — falha ao abrir o atendimento. Resolver: confira se há uma conexão ativa e se o contato tem telefone válido. Tente de novo e, se persistir, recarregue.
- “Não foi possível carregar a conversa.” — falha ao abrir a conversa a partir do cartão do Funil ou do painel de Rastreamento. Resolver: tente abrir de novo; se persistir, recarregue a página.
- “Todos os atendimentos deste contato estão sendo conduzidos por outros atendentes…” — toda conversa desse contato já tem dono: outros atendentes a assumiram. Resolver: só quem pode ver todas as conversas (administradores e quem tem nível Supervisor ou Administrar em Atendimento) ou uma transferência dá acesso a você (ver dono do atendimento em Atendimento / Chat).

### Anexos

- “Anexos não são suportados no modo nota interna.” — você tentou anexar dentro de uma nota interna. Resolver: saia do modo nota interna para anexar arquivos.
- “O arquivo “{nome}” excede o limite de 100 MB.” — um dos arquivos anexados passa do teto de 100 MB. Resolver: comprima o arquivo ou mande um menor. Os demais do lote seguem normalmente.
- “O arquivo “{nome}” não é um tipo aceito.” — o tipo daquele arquivo não entra no chat. Resolver: converta para um formato aceito (imagem, áudio, vídeo ou documento).
- “Você pode anexar até 10 arquivos por vez. {n} arquivos ficaram de fora.” — o chat aceita até 10 arquivos por envio. O aviso diz quantos ficaram de fora (com um só, aparece _"1 arquivo ficou de fora."_). Resolver: envie os que ficaram de fora em outra leva.
- “Não foi possível processar o arquivo.” — arquivo inválido ou corrompido, ou tipo não suportado. Resolver: troque o arquivo; ele pode estar corrompido ou ser de um tipo não aceito.

### Enviar, encaminhar e agendar

- “Selecione uma conexão para enviar a mensagem.” — falta escolher a conexão. Resolver: escolha a conexão pela qual a mensagem vai sair.
- “Não foi possível enviar” — (no balão) o WhatsApp não entregou a mensagem. Em geral é conexão caída, número sem WhatsApp ou janela de 24h fechada na API Oficial. Na lista de conversas, e nas mensagens de template, aparece como "Falha no envio". Resolver: clique no texto (quando estiver sublinhado) para ver o motivo em Falha no envio. Confira a bolinha de status da conexão e, na API Oficial, a janela de 24h. Depois use Tentar novamente.
- “Falha ao enviar” — (no balão) o navegador não conseguiu mandar a mensagem, que nem saiu. Resolver: clique em Tentar novamente; se persistir, confira sua internet.
- “Não foi possível encaminhar as mensagens.” — falha ao encaminhar mensagens. Resolver: tente encaminhar de novo.
- “Você pode encaminhar para até {n} conversas por vez.” — passou do teto de destinos do encaminhamento. Resolver: tire alguém da seleção ou encaminhe em duas levas.
- “Não foi possível salvar o agendamento.” — falha ao agendar mensagem. Resolver: revise o horário e tente agendar de novo.

### Templates (API Oficial)

Template é um modelo de mensagem aprovado pela Meta, usado só em conexões da API Oficial.

- “Este template não pode ser enviado para este contato agora. Confira se ele está aprovado.” — o template oficial não existe mais, ainda não foi aprovado ou o contato não aceita aquele tipo de mensagem. Resolver: confirme que o template está aprovado pela Meta e escolha outro se for preciso.
- “Preencha todas as variáveis do template.” — falta valor em alguma variável do corpo ou do cabeçalho. Resolver: complete todos os campos de variável do template antes de enviar.
- “Preencha o valor dos botões do template.” — algum botão do template ficou sem valor. Resolver: complete o valor dos botões que pedem um dado (como o final de um link).
- “Confira o cabeçalho do template: falta o arquivo ou o formato ainda não é suportado.” — o cabeçalho com imagem, vídeo ou documento está sem arquivo ou com formato que a Convergefy ainda não envia. Resolver: anexe o arquivo do cabeçalho em um formato aceito.
- “A Meta recusou o arquivo do cabeçalho. Confira o arquivo escolhido.” — a Meta não aceitou a mídia do cabeçalho. Resolver: troque por outro arquivo, dentro do formato e do tamanho aceitos pela Meta.
- “Este template usa um recurso que a Convergefy ainda não envia.” — o template tem um componente que ainda não é enviado pela plataforma. Resolver: escolha outro template.
- “Este contato não tem um telefone válido para WhatsApp.” — o número do contato não serve para enviar. Resolver: corrija o telefone do contato e tente de novo.
- “A conexão desta conversa não está pronta para enviar.” — a conexão da conversa não é uma API Oficial pronta para enviar template. Resolver: confira a bolinha de status da conexão (ver Conexões) ou escolha outra conexão.
- “Não foi possível enviar o template.” — o envio do template oficial falhou por outro motivo. Resolver: tente enviar de novo. Se persistir, confira a aprovação do template, as variáveis e a conexão da API Oficial.

## Mensagens rápidas

- “Formato não aceito. Use JPG, PNG, GIF ou WebP.” — uma imagem, vídeo ou áudio foi recusado assim que você o escolheu. Documento não é recusado: aceita qualquer arquivo. Resolver: troque para um formato aceito. Para vídeo a mensagem diz \*“MP4 ou 3GP”\* e para áudio \*“OGG, WebM, MP3, M4A ou AAC”\*.
- “O arquivo passa do limite de 100 MB.” — o anexo passou do tamanho máximo. A recusa acontece na hora de escolher, não ao salvar. Resolver: comprima ou troque o arquivo por um menor.
- “Não foi possível excluir a mensagem rápida.” — falha ao excluir uma mensagem rápida. Resolver: tente excluir de novo; se persistir, recarregue a página.
- “Nenhuma mensagem rápida encontrada / Nenhuma mensagem rápida.” — não há mensagens rápidas cadastradas. Resolver: é só uma lista vazia; crie uma mensagem rápida para começar.

## Funis / CRM

Primeiro, as confirmações que pedem cuidado: o que elas fazem não tem volta.

- “Marcar como Ganho?” — diálogo do cartão do negócio, com o campo "Valor da venda" (opcional, já preenchido com o valor atual) e o aviso _"Depois de marcado, o negócio não volta a ficar em aberto."_ Resolver: depois de marcado, o negócio não volta a ficar em aberto, então confirme só com certeza. Confira o campo “Valor da venda” antes de confirmar.
- “Marcar como Perda?” — diálogo do cartão do negócio, sem campo de valor, com o mesmo aviso _"Depois de marcado, o negócio não volta a ficar em aberto."_ Resolver: depois de marcado, o negócio não volta a ficar em aberto, então confirme só com certeza.
- “Remover negócio?” — confirmação ao excluir: _"O negócio '{título}' será removido permanentemente. Esta ação não pode ser desfeita."_ Resolver: a remoção é permanente, então confirme apenas se tiver certeza.

Agora as falhas.

- “Não foi possível criar o funil.” — falha ao criar um funil. Resolver: tente criar de novo; confira sua internet.
- “Não foi possível criar a coluna.” — falha ao criar uma etapa/coluna do funil. Resolver: tente criar a coluna de novo.
- “Não foi possível remover a coluna.” — falha ao excluir uma etapa. Quando o motivo é a coluna ter negócios, a mensagem é _"Só dá para excluir uma coluna sem negócios. Limpe a busca e os filtros para ver os negócios dela."_ Com uma coluna só, _"O funil precisa de ao menos uma coluna."_ Com negócios dentro, o item “Excluir” do menu já aparece desativado, sem mensagem nenhuma. Resolver: esvazie a coluna antes de excluir e lembre que o funil precisa de ao menos uma coluna.
- “Este funil não tem etapas.” — o funil escolhido no campo "Etapa" está sem coluna nenhuma. O mesmo texto aparece no diálogo "Mover negócio", com _"Escolha o funil e a etapa de destino."_ Resolver: crie ao menos uma coluna no funil antes de pôr negócio nele.

## Contatos

- “O telefone é obrigatório” — campo obrigatório vazio no cadastro. Resolver: informe o telefone do contato.
- “Digite um e-mail válido” — o e-mail informado está inválido. Resolver: corrija o e-mail para um formato válido.
- “Não foi possível criar o contato.” — falha ao cadastrar o contato. Aparece no cadastro de Contatos e também ao iniciar uma conversa no Chat. Resolver: revise os dados do contato (telefone, e-mail) e tente de novo.
- “Não foi possível salvar as informações de contato.” — falha ao editar o contato. Como a edição é campo a campo, a mensagem muda conforme o que você mexeu: _"Não foi possível salvar o nome."_ ou _"Não foi possível salvar os campos personalizados."_ Resolver: revise os dados e tente salvar de novo.
- “Não foi possível excluir o contato.” — falha ao remover o contato. Resolver: tente excluir de novo; se persistir, recarregue a página.
- “Não foi possível atualizar as tags do contato.” — falha ao mudar as tags de um contato. Resolver: tente adicionar ou remover a tag de novo.
- “Nenhum lead encontrado.” — não há contatos para mostrar. Resolver: é só uma lista vazia; ajuste o filtro ou cadastre um contato.

## Tags e Departamentos

- “Excluir tag?” — diálogo de exclusão: _"A tag {nome} será removida de todos os leads que a possuem. Esta ação não pode ser desfeita."_ Resolver: a tag some de todos os contatos que a têm, então confirme só se tiver certeza.
- “Erro ao carregar tags / Tentar novamente” — a lista de tags não carregou. Resolver: clique em “Tentar novamente”. É falha momentânea ao listar.
- “Erro ao carregar departamentos / Tentar novamente” — a lista de departamentos não carregou. Resolver: clique em “Tentar novamente”. É falha momentânea ao listar.

## Automações

### Ao montar o fluxo no editor

- “Resolva as pendências para ativar” — a automação tem erro de validação. **Salvar continua funcionando** mesmo com o fluxo inválido: ele só fica desativado quando não há nenhuma mudança para gravar. Resolver: abra o indicador de problemas no topo do editor e corrija cada item. O botão “Ativar automação” libera quando tudo estiver válido.
- “Adicione um gatilho para iniciar o fluxo” — a automação está sem gatilho. Resolver: abra o bloco Gatilhos e clique em “Adicionar gatilho”.
- “Adicione pelo menos um passo ao fluxo” — o fluxo só tem gatilhos. Resolver: adicione ao menos um bloco depois dos gatilhos.
- “Bloco sem ligação de entrada” — sobrou um bloco solto no quadro. Resolver: ligue uma saída de outro bloco até a entrada dele, ou apague o bloco.
- “Conecte a saída "Tempo esgotado"” — um bloco que espera ou decide está com uma saída obrigatória solta. Resolver: ligue a saída indicada a um próximo bloco.
- “Adicione pelo menos uma opção” — o passo está sem opções obrigatórias. Resolver: preencha as opções que faltam no passo.
- “Cada opção precisa de ao menos uma palavra-chave” — falta palavra-chave em uma opção. Resolver: adicione ao menos uma palavra-chave por opção.
- “Deve ser maior que 0” — valor inválido no passo. Resolver: informe um número maior que zero no campo.
- “Máximo 90 dias” — o prazo informado passou do limite. Resolver: reduza o prazo para no máximo 90 dias.
- “Entre 1 e 60 segundos” — o tempo informado está fora do intervalo. Resolver: informe um tempo entre 1 e 60 segundos.
- “Saída sem ligação” — na execução, um passo falhou e a saída de erro dele estava solta, então a execução parou. Resolver: ligue a saída de erro do bloco a um caminho, ou ligue o “Tratamento de erro” na seção Controle.

### Ao disparar pelo Chat

- “Esta automação não está ativa.” — (no disparo manual pelo Chat) a automação está pausada ou arquivada. Resolver: ative a automação no editor e dispare de novo.
- “Não foi possível executar a automação.” — o disparo manual pelo Chat falhou. Resolver: tente disparar de novo; se persistir, procure o suporte.
- “Automação iniciada com sucesso” — não é erro: confirma que o disparo manual pelo Chat funcionou. Resolver: nenhuma ação necessária.

> Validações detalhadas e execuções estão em [Automações](https://docs.convergefy.com.br/kb/automacoes.md).

## Disparo em massa

- “Pause ou cancele a campanha antes de excluir.” — tentativa de excluir uma campanha que está enviando. Resolver: use “Pausar” ou “Cancelar” e só então exclua.
- “Escolha ao menos uma tag, coluna do funil ou atendente.” — a campanha ficou sem público. Ao iniciar, se o público ficou vazio (por exemplo, uma tag ou coluna foi apagada entre montar e disparar), o aviso é _"Escolha ao menos uma tag, coluna do funil ou contato."_ Resolver: marque pelo menos uma tag, uma coluna ou um atendente principal em “Quem recebe”.
- “O template escolhido não foi encontrado ou não está aprovado.” — ao iniciar, o template da API Oficial escolhido já não está aprovado. Resolver: escolha outro template. Se ele existia, confira o status dele no painel da Meta.
- “A conexão escolhida foi removida, está desligada ou está incompleta.” — a conexão usada foi apagada, está desligada ou falta credencial da API Oficial. Resolver: reconfigure a conexão em Conexões ou crie a campanha de novo apontando uma conexão ativa.
- “Com a campanha pausada, só dá para mudar nome, dias, horários e velocidade.” — edição de campo congelado. Resolver: ajuste apenas nome, dias/horários e velocidade. Para trocar público ou mensagem, cancele e crie outra.
- “Contato sem telefone válido.” — motivo de um destinatário não ter recebido. Resolver: corrija o telefone do contato. Ele aparece como “pulado” no relatório da campanha.

> Os motivos de falha listados no detalhe da campanha vêm crus do WhatsApp e podem ser técnicos (ex.: _"cURL error 28: Operation timed out"_). Detalhes em [Disparo em massa](https://docs.convergefy.com.br/kb/disparo-em-massa.md).

## Rastreamento (Meta e Google Ads)

- “A integração com a Meta não está configurada neste ambiente. Fale com o suporte.” — falta configuração da integração; tentar de novo não resolve. Resolver: não há o que fazer do seu lado. Acione o suporte.
- “Não foi possível carregar o conector da Meta. Um bloqueador de anúncios, extensão de privacidade ou a rede da sua empresa pode estar bloqueando connect.facebook.net.” — o componente da Meta não carregou. Resolver: desative o bloqueador nesta página (ou peça liberação da rede) e clique em “Tentar novamente”.
- “Não conseguimos abrir a janela da Meta. Verifique se o navegador bloqueou o pop-up desta página e tente de novo.” — a janela de autorização foi barrada. Resolver: libere pop-ups para o endereço da Convergefy e repita.
- “Não foi possível carregar suas contas do Google Ads.” — a lista de contas não carregou. Resolver: use “Tentar de novo”. Confira se a conta Google conectada tem acesso a contas do Google Ads.
- “Não foi possível carregar as ações de conversão.” — a lista de ações de conversão não carregou. Resolver: use “Tentar de novo” no seletor. Confira em Contas de Anúncio se a conta Google continua conectada.

## Conta e perfil

- “Não foi possível alterar a senha.” — a troca de senha falhou. A causa mais comum é a senha atual errada. Resolver: confira a “Senha atual”. Se não lembra, saia e use “Esqueceu a senha?” no login.
- “A senha atual informada não confere.” — aparece dentro do campo “Senha atual”, quando a senha informada está errada. Resolver: a “Senha atual” digitada não confere. Corrija-a ou use “Esqueceu a senha?” no login.
- “As senhas não correspondem.” — a confirmação não bate com a nova senha. Resolver: repita exatamente a mesma senha no campo de confirmação.
- “A nova senha precisa de ao menos 8 caracteres.” — a nova senha é curta demais. Resolver: escolha uma senha mais longa.
- “Perfil atualizado com sucesso.” — não é erro: confirma que seus dados (nome, telefone, e-mail) foram salvos. Resolver: nenhuma ação necessária.
- “Senha alterada com sucesso.” — não é erro: confirma que a troca de senha foi concluída. Resolver: nenhuma ação necessária.

## Quando a mensagem não está aqui

1. **Identifique a tela** — Veja em qual área o erro apareceu: Chat, Conexão, Funil, Contato ou Automação.
2. **Procure um pré-requisito faltando** — Confira o básico: há uma conexão ativa? Algum campo obrigatório está vazio? Você tem permissão para aquele atendimento?
3. **Para falhas de envio, olhe a conexão** — Mensagem que não sai aponta quase sempre para a conexão. Confira a bolinha de status (ver [Conexões](https://docs.convergefy.com.br/kb/conexoes.md)).
4. **Se ainda assim não resolver** — Procure o suporte em vez de adivinhar. É melhor confirmar do que supor uma causa errada.
