# Conexões de WhatsApp

Uma conexão é um número de WhatsApp que sua empresa liga à Convergefy para enviar e receber mensagens. Sem pelo menos uma conexão ativa, não dá para atender no Chat nem disparar automações.

Na Central de Ajuda: https://docs.convergefy.com.br/#/conexoes

## Em resumo

A conexão é o **primeiro passo** para usar a plataforma: toda conversa no Chat e todo envio por automação dependem de pelo menos uma conexão ativa. Uma empresa pode ter várias conexões.

Cada conexão é de um de dois tipos: WhatsApp Web (liga por QR Code) ou API Oficial (o WhatsApp Business da Meta, também chamado WABA).

### Algo deu errado?

Procure o que você está vendo e siga a coluna da direita. O detalhe de cada caso está mais abaixo.

| O que você vê                                                                                               | O que fazer                                                                                                                  |
| ----------------------------------------------------------------------------------------------------------- | ---------------------------------------------------------------------------------------------------------------------------- |
| Status "Desconectado" no WhatsApp Web (o número caiu: celular sem internet ou sessão encerrada no aparelho) | Reconecte lendo o QR Code de novo.                                                                                           |
| Conexões do WhatsApp Web desligadas depois de mais de 15 dias sem assinatura                                | Ao voltar a assinar, leia o QR Code de novo.                                                                                 |
| Status "Acesso recusado" (vermelho) na API Oficial                                                          | Nenhuma mensagem sai até renovar o acesso. Clique em "Atualizar conexão" e conclua o login.                                  |
| Status "Reportada", "Qualidade Baixa", "Restringida" ou "Banida" na API Oficial                             | A decisão é da Meta, não da Convergefy. Resolva na conta Meta / WhatsApp Manager.                                            |
| Bolinha de status que parece travada                                                                        | Use "Sincronizar status".                                                                                                    |
| Balão "Falha ao enviar" ou "Não foi possível enviar" no Chat                                                | Confira a bolinha de status da conexão e reenvie. Na API Oficial, veja também se a janela de 24h de atendimento está aberta. |
| Conversa com o aviso "Conexão removida"                                                                     | A conexão foi excluída. Veja "A conexão dentro do Chat".                                                                     |
| "Você não tem permissão para fazer isso."                                                                   | Peça a um Administrador o nível Administrar em Conexões.                                                                     |

Você gerencia tudo em **Configurações → INTEGRAÇÕES**. Todos os membros enxergam as conexões. Para conectar, renomear, usar as ações e excluir, é preciso ter o nível Administrar em Conexões. As abas "Grupos" e "API" têm regras próprias, descritas abaixo.

**Quem pode configurar**

O nível Administrar em Conexões fica na aba "Acesso" do membro. O Administrador da empresa já tem. Sem esse nível, somem:

- **"Conectar WhatsApp"** e **"Conectar WhatsApp API"**;
- o menu ⋮ do card;
- o lápis de renomear;
- as ações do painel;
- **"Excluir conexão"**.

Ao abrir Configurações, o atendente cai direto em Membros.

**Conceitos rápidos**

- **Conexão** — Um número de WhatsApp ligado à plataforma. Uma empresa pode ter várias.
- **WhatsApp Web (Zap)** — Conexão não oficial, feita lendo um QR Code com o celular, igual ao WhatsApp Web do navegador. Rápida de configurar; usa o número de um aparelho.
- **API Oficial** — O WhatsApp Business da Meta, também chamado WABA. Conexão oficial pela API da Meta (WhatsApp Cloud API). Exige conta na Meta, mas é mais estável e permite templates (mensagens-modelo aprovadas) e vários atendentes no mesmo número.
- **QR Code** — O quadradinho que você escaneia no celular para ligar o WhatsApp Web.
- **Status** — A situação da conexão (conectada, aguardando QR, etc.), mostrada por uma bolinha colorida + texto.

## Os dois tipos — qual escolher

| Tipo         | Como aparece           | Quando usar                                                                                                               |
| ------------ | ---------------------- | ------------------------------------------------------------------------------------------------------------------------- |
| WhatsApp Web | "WhatsApp Web"         | Começar rápido, sem burocracia. Usa um celular com o número. Bom para times pequenos.                                     |
| API Oficial  | "WhatsApp API Oficial" | Operação séria e estável: vários atendentes no mesmo número, templates aprovados, menos risco de queda. Exige conta Meta. |

> **Por que existem dois**
>
> O WhatsApp Web é prático, mas depende de um celular ligado. A API Oficial é mais robusta e profissional, mas exige configuração na Meta.

> **Não encontrou o item “WhatsApp Web”?**
>
> Se o item "WhatsApp Web" não aparece no menu de Configurações → Integrações, fale com o suporte.

Cada conexão aparece como um card com o nome, o número completo (em formato internacional; sem número, aparece _"Sem número associado"_) e o selo de status (bolinha + texto). Na API Oficial, o nome do negócio aparece ao lado do nome (_"· {nome do negócio}"_) e a qualidade do número aparece ao lado do status (veja mais abaixo).

### Buscar uma conexão

Quando já existe pelo menos uma conexão, aparece acima dos cards, nas duas telas, o campo **"Buscar por nome ou telefone"**. Se nada bate, a tela mostra "Nenhuma conexão encontrada": _"Confira o nome ou o telefone digitado."_

## Conectar por WhatsApp Web (QR Code)

Tela "WhatsApp Web": _"Gerencie suas conexões do WhatsApp Web."_

Imagem: [A tela WhatsApp Web: o botão Conectar WhatsApp fica no canto de cima, e cada card mostra o nome, o número e o status da conexão.](https://docs.convergefy.com.br/img/conexoes/lista-de-conexoes.webp)

1. **Iniciar** — Clique em **"Conectar WhatsApp"**. Abre "Conectar WhatsApp Web": _"Dê um nome para esta conexão e escaneie o QR Code para conectar."_ Preencha o "Nome da conexão" (ex.: _"Suporte WhatsApp"_) e clique em **"Avançar"**.

   Imagem: [A janela Conectar WhatsApp Web: dê um nome e clique em Avançar para ver o QR Code.](https://docs.convergefy.com.br/img/conexoes/conectar-whatsapp-web.webp)
2. **Aguardar o QR** — A janela prepara a conexão ("Preparando conexão…") e passa para "Leitura do QR Code", com o QR Code na tela.
3. **Escanear no celular** — No celular: WhatsApp → **Aparelhos conectados** → **Conectar um aparelho** → aponte a câmera para o QR Code.
4. **Pronto** — Ao ligar, aparece "Conexão estabelecida!" e a janela fecha sozinha em \~2 segundos.

**Status do WhatsApp Web (bolinha colorida)**

- **Conectado** (green) — funcionando, pronto para enviar/receber.
- **Aguardando QR** (amber) — bolinha amarela; falta escanear o QR Code.
- **Preparando…** (blue) — preparando a conexão.
- **Conectando…** (blue) — autenticando.
- **Desligando…** (gray) — encerrando.
- **Desconectado** (gray) — o número caiu (celular sem internet, sessão encerrada no aparelho). Como resolver: reconecte lendo o QR de novo.

Quando o status está sincronizando, a bolinha vira um ícone girando (em vez da bolinha fixa).

> **Sem assinatura, a conexão é desligada**
>
> Se a empresa ficar mais de **15 dias** sem assinatura ativa, a Convergefy desliga as conexões do WhatsApp Web que estavam ligadas. Elas passam a "Desconectado" e o card volta a mostrar _"Sem número associado"_. Ao voltar a assinar, leia o QR Code de novo para reconectar.

### O painel da conexão

Clicando no card da conexão, abre um painel lateral com o nome no topo e as abas de configuração. O lápis ao lado do nome renomeia ali mesmo (_"Nome atualizado."_). Quais abas aparecem depende do canal:

|              | Abas                                                     |
| ------------ | -------------------------------------------------------- |
| WhatsApp Web | Geral · Grupos, mais API para o Administrador da empresa |
| API Oficial  | só Geral (o painel não mostra barra de abas)             |

As ações de gerenciar ficam na aba "Geral". O menu ⋮ do card muda conforme o canal:

- No WhatsApp Web, o menu ⋮ repete essas ações e inclui "Excluir".
- Na API Oficial, o menu ⋮ tem só "Sincronizar" e "Excluir". "Atualizar conexão" fica apenas no painel.
- "Excluir conexão" fica fora das abas, num botão no rodapé do painel.

> **Excluir é irreversível**
>
> Excluir derruba o número da plataforma: as conversas dele passam a mostrar "{nome} · removida". O histórico das mensagens é preservado, mas o envio por aquele número fica bloqueado.
>
> A tela pede confirmação:
>
> - WhatsApp Web: _"Tem certeza que deseja excluir {nome}? Esta ação não pode ser revertida."_
> - API Oficial: _"Tem certeza que deseja excluir a conexão “{nome}”? Esta ação não pode ser revertida."_
>
> No WhatsApp Web, se a conexão não estiver "Desconectado", aparece o aviso _"Esta conexão está ativa. Será desligada automaticamente antes de ser excluída."_ e ela é desligada antes. Ao terminar: "Conexão excluída com sucesso."

**Gerenciar uma conexão (aba “Geral”)**

No WhatsApp Web as ações mudam conforme o status da conexão. Na API Oficial existem só "Sincronizar status" e "Atualizar conexão": ela não tem pareamento nem instância para desligar.

- **Sincronizar status** — força a checagem da situação atual (use se a bolinha parecer travada).
- **Ver QR** — reexibe o QR code de uma conexão que ainda está esperando leitura. Não desconecta nada, só mostra o código de novo.
- **Trocar conta / novo QR** — aparece quando a conexão já está ligada: encerra a sessão atual e libera um QR novo, para trocar de aparelho/número.
- **Conectar** — (re)inicia a conexão quando ela está parada: abre "A iniciar conexão…" e depois "Leitura do QR Code".
- **Desligar instância** — para a conexão. → "Instância desligada com sucesso."
- **Atualizar conexão** — (só API Oficial) _"Refaz o login no Facebook para renovar o acesso ou registrar outro número."_ Veja "Atualizar a conexão" mais abaixo.
- **Excluir conexão** — remove a conexão (veja o aviso acima). Fica no rodapé do painel, não na lista de ações.

## Aba "Grupos" (WhatsApp Web)

Define se o número recebe mensagens de grupos do WhatsApp e como cada grupo novo é liberado para a equipe. O painel avisa: _"Vale para os próximos grupos — os que já chegaram não mudam."_

Quem tem o nível Administrar em Atendimento vê os controles:

- **Atender grupos** — chave que liga ou desliga os grupos deste número: _"Os grupos deste número aparecem na aba Grupos do chat."_ Desligada, as mensagens de grupo deste número não são recebidas.
- **Modo de liberação** — como o grupo que chega pela primeira vez é tratado. Fica apagado enquanto "Atender grupos" está desligado.

* **Liberar novos grupos automaticamente** — _"Todo grupo que chegar por este número fica visível para todos os membros da empresa."_
* **Aprovar cada grupo manualmente** — _"O grupo chega visível só para administradores e supervisores do atendimento e espera a sua liberação."_ Para liberar: no chat, aba Grupos, clique no grupo e ligue "Visível para toda a empresa" no painel da direita (também dá para clicar com o botão direito no card do grupo).

Quem não tem o nível Administrar em Atendimento vê a aba só para leitura ("Ativo" / "Desativado" e "Aprovação manual" / "Automático"). Ver [Atendimento / Chat](https://docs.convergefy.com.br/kb/chat.md).

## Aba "API" — disparo por sistemas externos (WhatsApp Web)

A aba "API" existe só no WhatsApp Web e só para o Administrador da empresa (o nível Administrar em Conexões não basta). Ela entrega um token (uma espécie de senha) para outro sistema enviar mensagens por esta conexão.

> **Só vale para o WhatsApp Web, com assinatura ativa**
>
> O token não funciona em conexão da API Oficial e só envia enquanto a assinatura da empresa estiver ativa. Quem tem o token envia mensagens por aquele número: guarde-o como uma senha e gere um novo se ele vazar.

- **Token para disparo via API** — _"Envie mensagens por esta conexão a partir de sistemas externos. O token vale somente para esta conexão; guarde como uma senha."_
- **URL de envio** — o endereço para onde o sistema externo envia as mensagens, com o botão "Copiar URL de envio".
- **Token** — aparece mascarado; o olho ("Mostrar token" / "Ocultar token") revela e o botão "Copiar token" copia. Se não carregar: _"Não foi possível carregar o token."_ e o botão "Tentar de novo".
- **Gerar novo token** — abre "Gerar novo token?": _"O token atual para de funcionar na hora. As integrações que usam ele falham até receberem o novo."_ Ao confirmar: "Novo token gerado."

## Conectar pela API Oficial (WhatsApp Business / WABA)

Tela "WhatsApp API Oficial": _"Gerencie sua conexão com a API Oficial do WhatsApp Business."_ Sem nenhuma conexão ainda, aparece _"Nenhuma conexão configurada"_ com o botão **"Conectar WhatsApp API"**.

O que você precisa (a tela lista em _"O que você precisa:"_):

- Conta do Facebook Business Manager.
- Número de telefone verificado.
- WhatsApp Business aprovado pela Meta.

1. **Dar um nome** — Clique em **"Conectar WhatsApp API"**. Abre "Conectar WhatsApp Business API": _"Dê um nome para esta conexão e autentique através do Facebook Business Manager"_. Preencha o "Nome da Conexão" (ex.: _"API Oficial - Vendas"_).
2. **Continuar com Facebook** — Clique em **"Continuar com Facebook"**: _"Você será redirecionado para fazer login com sua conta Meta"_. Numa janela da Meta você escolhe o número e autoriza. A própria Meta conduz o cadastro.
3. **Aguardar e pronto** — A tela acompanha o progresso (_"Conectando ao Facebook..."_ → _"Verificando número de telefone..."_ → _"Configurando sua conta..."_) e termina com "Conexão estabelecida com sucesso!". A janela fecha sozinha e aparece o aviso "Conexão criada com sucesso!"

> **Um único botão: a Meta decide o tipo**
>
> Você não escolhe entre "Padrão" e "Coexistência", nem digita PIN aqui. O fluxo é um só botão. Pelo número informado na janela da Meta, a própria Meta decide se ele entra como **Conexão Padrão** (número novo na API) ou **Conexão em Coexistência** (coexistência é quando o número já usa o WhatsApp Business App). O tipo aparece depois, como selo ao lado do status, no painel da conexão.

### Quando a Meta recusa o acesso

Se a Meta deixa de aceitar o acesso da conexão, o card mostra o status "Acesso recusado" (vermelho) e **nenhuma mensagem sai** por ela até o acesso ser renovado.

O painel ganha, no topo, o aviso "A Meta recusou o acesso" (_"Nenhuma mensagem sai por esta conexão até o acesso ser renovado."_), com:

- o motivo dado pela Meta;
- de onde veio: "Ao consultar o número", "Na renovação automática do acesso" ou "Ao enviar uma mensagem";
- a data e hora;
- o "Código N." do erro.

> **Enquanto o acesso está recusado**
>
> - Campanhas de disparo que usam essa conexão são pausadas. Depois de renovar o acesso, use "Retomar" na lista de campanhas.
> - Mensagens agendadas por essa conexão não saem e deixam um aviso de falha na conversa.
> - Automações que enviam por essa conexão seguem pela saída "Tratamento de erro" do bloco. O histórico da execução registra "Conexão indisponível".

Para resolver, clique em **"Atualizar conexão"** (o botão aparece no aviso e na lista de ações, para quem tem o nível Administrar em Conexões) e conclua o login. Quando a Meta recusa algo sem derrubar o acesso, o mesmo painel mostra o aviso mais discreto "Última recusa da Meta", sem o botão.

O acesso da API Oficial é renovado sozinho pela Convergefy. Se essa renovação falhar, o motivo aparece nesse aviso.

### Atualizar a conexão

"Atualizar conexão" (aba "Geral" do painel) reabre o login da Meta. Use quando o acesso foi recusado ou para registrar outro número na mesma conexão. Ao terminar: "Conexão atualizada com sucesso!" Se o número já estiver em outra conexão ou a Meta recusar o cadastro: _"Não foi possível cadastrar este número: ele já está em outra conexão ou a Meta recusou o cadastro."_

### Qualidade do número

Ao lado do status, o card da API Oficial mostra "Qualidade alta", "Qualidade média" ou "Qualidade baixa" (verde, amarelo e vermelho): é a nota que a Meta dá ao número. Com o acesso recusado a qualidade some, porque a última leitura não vale mais. Não confunda com o status "Qualidade Baixa" abaixo, que já indica bloqueio de envio.

**Status da API Oficial (passe o mouse na bolinha para ver a explicação)**

Na prática você verá quase sempre Conectado / Verificada. Os outros estados aparecem só quando a Meta sinaliza algum problema com o seu número. Nos textos abaixo, “registrar” o número é habilitá-lo para uso na API, e “des-registrar” é tirá-lo da API.

> **Por que laranja/vermelho bloqueiam o envio**
>
> Esses estados (Reportada, Qualidade Baixa, Restringida, Banida…) vêm de decisões da Meta sobre sua conta: qualidade, limite ou política. Nesses casos o problema não é da Convergefy. É preciso resolver na conta Meta / WhatsApp Manager.

- **Conectado / Verificada** (green) — associado a uma WABA registrado para uso na API e pode enviar mensagens. Tudo certo.
- **Pendente** (amber) — bolinha amarela; associado a uma WABA, mas ainda não foi “registrado” para uso na API.
- **Não Verificada** (amber) — bolinha amarela; após “verificado”, 14 dias se passaram e o número não foi “registrado”.
- **Reportada** (orange) — não pode enviar mensagens porque usuários reportaram “spam”.
- **Qualidade Baixa** (orange) — não pode enviar mensagens porque está com “baixa qualidade”.
- **Restringida** (orange) — não pode enviar mensagens porque alcançou o limite de envios.
- **Migrada** (blue) — número foi migrado de uma WABA para outra.
- **Desconectada** (gray) — foi “des-registrado” da API.
- **Acesso recusado** (red) — a Meta recusou o acesso desta conexão; nenhuma mensagem sai até ele ser renovado. Como resolver: use “Atualizar conexão” para renovar o acesso.
- **Banida** (red) — não pode enviar mensagens devido a uma violação de política.
- **Deletada** (red) — deletado da API (30 dias depois que o número foi deletado pelo WhatsApp Manager).
- **Desconhecido** (red) — problema desconhecido: “des-registre” e “registre” novamente.

### Painel da conexão: renomear, diagnosticar e atualizar

Ao clicar no card de uma conexão da API Oficial, o painel lateral mostra:

- **Nome** — o lápis ao lado do nome permite renomear; ao apertar Enter ou clicar fora, salva sozinho (_"Nome atualizado."_). Nome vazio: _"Informe um nome para a conexão."_
- **Selo do tipo** — "Conexão Padrão" ou "Conexão em Coexistência", conforme a Meta registrou, ao lado do status.
- **Atualizar conexão** — refaz o login no Facebook para renovar o acesso ou registrar outro número nesta conexão (veja "Atualizar a conexão", acima).
- **Diagnóstico da Conta** — quando a Meta sinaliza problema, um painel lista o que está "Bloqueado", "Limitado" ou em "Aviso" (Número de Telefone, Conta WhatsApp, Gerenciador de Negócios, Aplicativo Meta) com a "Solução:" sugerida.
- **Dados da conta** — grade só-leitura com "Nome Verificado", "Empresa (Gerenciador)", "Fuso Horário", "Número de telefone", "ID do número" e "WABA ID".

> **O PIN de verificação**
>
> O PIN (código de 6 dígitos que protege o número contra registros não autorizados) não é pedido na criação. Ele aparece, só para consulta, em "PIN de verificação" (campo mascarado, com olho para revelar), e apenas quando existe: conexões de coexistência, por exemplo, não geram PIN, então o campo nem é mostrado.

### Sincronização de histórico (coexistência)

Quando o número entra em coexistência (já vinha sendo usado no WhatsApp Business App), a Meta pode importar o histórico de conversas para a Convergefy. Só quem tem o nível Administrar em Conexões acompanha esse progresso, em dois lugares:

- **No topo do Chat** — um aviso "Sincronizando histórico" com uma barra e o percentual por conexão. Ao terminar: "Histórico concluído"; se o cliente recusar: "Cliente recusou compartilhar o histórico".
- **No card da conexão** — o mesmo progresso aparece no rodapé do card, com selos "Histórico concluído" / "Histórico recusado" no fim.

**Como a importação de histórico se comporta**

- É uma importação silenciosa: as conversas antigas entram já finalizadas, não reabrem atendimento nem disparam automações, e as mensagens ficam com a data original.
- As conversas importadas aparecem sozinhas para todos (sem recarregar a página). Só o aviso de progresso é exclusivo de quem gerencia conexões.
- Os avisos de concluído/recusado ficam até a pessoa fechar no ×. Uma sincronização parada há mais de 1 hora deixa de ser exibida ao recarregar a página.
- Se o cliente recusar compartilhar o histórico (uma escolha dele, no aparelho), nada é importado.
- A Meta importa até 180 dias de conversas passadas. O que for mais antigo que isso não vem.

## Limitações conhecidas

> - A importação de histórico na coexistência depende de o cliente aceitar compartilhar, e traz as conversas antigas já finalizadas (não reabrem atendimento).
> - Nas automações, enviar para números da API Oficial fora da janela de 24h exige templates aprovados. Texto livre pode não chegar (ver [Automações](https://docs.convergefy.com.br/kb/automacoes.md)).

## A conexão dentro do Chat

No cabeçalho de cada conversa aparece a conexão usada e seu status (mesma bolinha). Se a conexão cair, o envio falha e o balão mostra "Falha ao enviar" ou "Não foi possível enviar". Em "Não foi possível enviar", o clique abre "Falha no envio", com o motivo.

> Se a conexão for removida, a conversa mostra "{nome da conexão} · removida" (ícone vermelho) e a caixa de digitação fica bloqueada, com o aviso "Conexão removida": _"Não é possível enviar mensagens nesta conversa — a conexão "{nome}" foi removida."_
>
> Dá para escolher outra conexão ali mesmo em empresas que atendem uma conversa por conexão. Nas demais, o caminho é recadastrar o número. (Ver [Atendimento / Chat](https://docs.convergefy.com.br/kb/chat.md).)

## Por que o status muda sozinho

A bolinha de status atualiza sozinha, sem recarregar a página: quando o número conecta, cai ou muda de situação na Meta, a tela reflete na hora. Enquanto sincroniza, aparece o ícone girando. Se algo parecer travado, use "Sincronizar status". (Ver [Tempo real](https://docs.convergefy.com.br/kb/tempo-real.md).)

## Erros e avisos esperados

- “Não foi possível iniciar a conexão.” — falha ao abrir/preparar a conexão Web. Resolver: tente de novo; se persistir, recarregue a página e reinicie a conexão.
- “Não foi possível criar a conexão.” — falha ao criar a conexão Web. Resolver: confira sua internet e tente criar de novo.
- “Não foi possível sincronizar o status.” — falha ao atualizar o status. Resolver: tente Sincronizar de novo.
- “Não foi possível renomear a conexão.” — falha ao salvar o novo nome. Resolver: tente salvar o nome de novo.
- “Não foi possível atualizar a conexão da API Oficial.” — falha ao salvar a atualização de uma conexão da API Oficial. Resolver: tente “Atualizar conexão” de novo.
- “Não foi possível cadastrar este número: ele já está em outra conexão ou a Meta recusou o cadastro.” — ao conectar ou atualizar uma conexão da API Oficial. Resolver: confira se o número já não está em outra conexão da empresa; se não estiver, revise na Meta o cadastro do número e tente de novo.
- “Não foi possível conectar a API Oficial.” — falha ao salvar a nova conexão da API Oficial depois do login na Meta. Resolver: tente de novo; se persistir, procure o suporte.
- “Não foi possível desligar a instância.” — falha ao desligar a conexão Web. Resolver: aguarde alguns segundos e tente de novo; se travar, recarregue a página.
- “Não foi possível encerrar a sessão.” — falha ao encerrar a sessão em "Trocar conta / novo QR". Resolver: aguarde alguns segundos e tente de novo; se travar, recarregue a página.
- “Desligue a conexão antes de excluir.” — o sistema não conseguiu desligar a conexão Web sozinho antes de excluir. Resolver: use “Desligar instância” e tente excluir de novo.
- “Não foi possível excluir a conexão.” — falha ao excluir a conexão Web. Resolver: tente de novo; se persistir, recarregue a página.
- “Não foi possível excluir a conexão. Tente novamente.” — falha ao excluir a conexão da API Oficial. Resolver: tente de novo; se persistir, recarregue a página.
- “Erro ao tentar realizar login: {motivo}” — o login do Facebook foi recusado ou voltou incompleto ao conectar a API Oficial. Resolver: refaça a conexão pelo botão da Meta e conceda todas as permissões pedidas; o motivo, depois dos dois-pontos, vem da própria Meta.
- “Login cancelado. Tente novamente.” — (API Oficial) você fechou o login do Facebook. Resolver: reabra o login do Facebook e conclua sem fechar a janela.
- “Ocorreu um erro ao tentar realizar login. Tente novamente.” — (API Oficial) a resposta da Meta não pôde ser lida durante o login. Resolver: tente de novo; confirme que sua conta Meta tem as permissões necessárias.
- “Não foi possível gerar um novo token.” — (aba "API") falha ao gerar um novo token do disparo via API. Resolver: tente gerar de novo; se persistir, recarregue a página.
- “Não foi possível salvar a configuração da conexão.” — (aba "Grupos") falha ao salvar a configuração de grupos da conexão. Resolver: tente salvar de novo; se persistir, recarregue a página.
- “Não foi possível carregar o token.” — (aba "API") o token do disparo via API não carregou. Resolver: use “Tentar de novo”; se persistir, recarregue a página.
- “Você não tem permissão para fazer isso.” — sua conta não tem o acesso necessário para a ação. Resolver: peça a um Administrador o nível Administrar em Conexões.
- “Erro interno do servidor, tente novamente mais tarde.” — falha do lado da Convergefy, não da sua conexão. Resolver: aguarde alguns minutos e tente de novo; se persistir, procure o suporte.
- “Sem conexão com o servidor. Verifique sua internet.” — o navegador não conseguiu falar com a Convergefy. Resolver: confira sua internet e tente de novo.
- “Falha ao enviar / Não foi possível enviar” — no balão do chat, costuma indicar conexão caída (Web desconectado) ou, na API Oficial, janela de atendimento fechada / status que bloqueia o envio. Resolver: confira a bolinha de status da conexão e reenvie; na API Oficial, verifique a janela de 24h de atendimento.
