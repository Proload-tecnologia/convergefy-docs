# Glossário

Dicionário rápido das palavras que aparecem na Convergefy, explicadas para quem está começando. Cada termo aponta para o guia onde ele é detalhado.

Na Central de Ajuda: https://docs.convergefy.com.br/#/glossario

## Em resumo

Esta página reúne os termos que você encontra pela plataforma, de Conexão a Webhook, explicados em linguagem simples. Está em dúvida sobre uma palavra? Procure-a no grupo correspondente abaixo. Quase todo termo traz um link para o guia onde o assunto é aprofundado.

## Pessoas e acesso

- **Conta** — Seu login pessoal (e-mail + senha). Uma mesma conta pode participar de várias empresas. Ver [Conta e acesso](https://docs.convergefy.com.br/kb/conta-acesso.md).
- **Empresa** — O espaço de trabalho do seu negócio, onde ficam conversas, funil e equipe. Ver [Dados da empresa](https://docs.convergefy.com.br/kb/organizacao.md).
- **Membro** — Uma pessoa com acesso à empresa. Ver [Equipe e permissões](https://docs.convergefy.com.br/kb/equipe-permissoes.md).
- **Administrador** — Membro que gerencia tudo: equipe, plano e integrações.
- **Atendente** — Membro que opera o dia a dia (conversas e vendas), sem acesso a configurações sensíveis.
- **Departamento** — Uma equipe operacional (ex.: Vendas, Suporte) usada para rotear atendimentos. Ver [Tags e Departamentos](https://docs.convergefy.com.br/kb/tags-departamentos.md).

## Atendimento

- **Conexão** — Um número de WhatsApp ligado à plataforma. Ver [Conexões](https://docs.convergefy.com.br/kb/conexoes.md).
- **WhatsApp Web** — Conexão não oficial, via QR Code (lê o WhatsApp de um celular).
- **API Oficial** — O WhatsApp Business da Meta (a empresa dona do WhatsApp), também chamado WABA. Conexão oficial pela API da Meta: mais estável e permite templates.
- **Conversa / atendimento** — O histórico de mensagens com um cliente. Ver [Atendimento / Chat](https://docs.convergefy.com.br/kb/chat.md).
- **Status do atendimento** — Em que ponto a conversa está: Aguardando (ninguém respondeu), Em Atendimento (alguém assumiu) ou Finalizados (encerrado). Ver [Atendimento / Chat](https://docs.convergefy.com.br/kb/chat.md).
- **Dono do atendimento** — O atendente que assumiu a conversa (ao responder). Outro atendente não vê a conversa que já tem dono; só o Administrador, quem tem permissão para ver todas as conversas ou uma transferência muda isso.
- **Atendimento único × múltiplo** — O modo da empresa. No único, cada contato tem uma conversa e você escolhe o número ao enviar; no múltiplo, há uma conversa por número para o mesmo contato. Ver [Atendimento / Chat](https://docs.convergefy.com.br/kb/chat.md).
- **Nota interna** — Recado só para a equipe; o cliente não vê.
- **Mensagem rápida** — Modelo de resposta pronto para reusar. Ver [Mensagens rápidas](https://docs.convergefy.com.br/kb/mensagens-rapidas.md).
- **Template (API Oficial)** — Mensagem-modelo aprovada pela Meta, usada para reabrir conversa fora da janela de 24h. O WhatsApp só permite mensagem livre por 24h após a última mensagem do cliente; depois disso, só template.
- **Tag** — Etiqueta colorida para classificar contatos e conversas. Ver [Tags e Departamentos](https://docs.convergefy.com.br/kb/tags-departamentos.md).
- **Grupo** — Uma conversa de grupo do WhatsApp. Fica num seletor próprio no Chat ("Conversas" / "Grupos") e tem notificação separada. Ver [Atendimento / Chat](https://docs.convergefy.com.br/kb/chat.md).
- **Campanha de disparo** — Envio da mesma mensagem para um público escolhido por tags, por colunas do funil, por atendente principal, ou uma combinação deles, em ritmo e horários controlados. Ver [Disparo em massa](https://docs.convergefy.com.br/kb/disparo-em-massa.md).

## Contatos e CRM

- **Contato / Lead** — O cliente, a pessoa do outro lado. Ver [Contatos](https://docs.convergefy.com.br/kb/contatos.md).
- **ID Externo** — Identificador opcional para casar o contato com outro sistema seu.
- **Funil** — O quadro de vendas em estilo Kanban (na tela aparece como "Funil"). Ver [Funis e CRM](https://docs.convergefy.com.br/kb/funis.md).
- **Etapa / Coluna** — Uma fase da venda dentro do funil.
- **Negócio (deal)** — O cartão de uma oportunidade, ligado a um contato.
- **Produto** — Um item do catálogo da empresa: nome, SKU e valor, cadastrado em **Configurações → Produtos**. Ver [Produtos](https://docs.convergefy.com.br/kb/produtos.md).
- **SKU** — O código interno do produto, se a empresa usa um (ex.: `PLANO-01`). Opcional, e pode repetir.
- **Produto cadastrado** — O campo do negócio que puxa um produto do catálogo e copia o nome e o valor dele. O negócio guarda a cópia, não um vínculo.
- **Ganho / Perda** — O desfecho de um negócio (irreversível).

## Automação

- **Automação** — Um fluxo que reage sozinho a um evento e executa passos. Ver [Automações](https://docs.convergefy.com.br/kb/automacoes.md).
- **Gatilho** — O evento que inicia a automação. Uma automação pode ter vários.
- **Bloco** — Cada caixa do quadro da automação, ligada às outras por ligações.
- **Passo** — Cada item dentro de um bloco: algo que a automação faz, espera ou decide.
- **Condição** — Bloco que escolhe o caminho do fluxo pelo que encontra ou lê: contato, negócio, atendente principal, status do atendimento, horário de funcionamento ou tipo do anexo. Cada um tem as suas saídas (por exemplo, Encontrado / Não encontrado). Não existe um bloco de condição genérico.
- **Espera** — Bloco que pausa o fluxo, com os passos Aguardar tempo, Aguardar resposta e Aguardar evento.
- **Execução** — Uma "rodada" da automação para um contato.
- **Variável** — Texto que a automação preenche sozinha, como o nome ou o telefone do contato. Digite {{ no campo de texto para escolher qual dado entra.
- **Webhook** — Uma URL exclusiva que um sistema externo chama para disparar uma automação.
- **Menu interativo** — Passo que envia botões ou uma lista que o cliente toca (em vez de digitar o número da opção). Só funciona em conexões WhatsApp Web. Ver [Automações](https://docs.convergefy.com.br/kb/automacoes.md).

## Plataforma

- **Tempo real** — Atualização automática da tela (mensagens, status) sem recarregar. Ver [Tempo real](https://docs.convergefy.com.br/kb/tempo-real.md).
- **Notificação** — Aviso (som/visual) de mensagem nova. Ver [Notificações](https://docs.convergefy.com.br/kb/notificacoes.md).
- **Agente de IA** — Atendente virtual que a empresa cria e treina e que conversa com o cliente dentro de uma automação, pelo passo "Agente de automação", ramificando o fluxo por saída. Fica no item "Agentes de IA" da barra lateral. Ver [Agentes de IA](https://docs.convergefy.com.br/kb/agentes-ia.md).
- **Assistente (Letícia)** — A ajuda inteligente que atende você dentro da plataforma, não o seu cliente: responde dúvidas sobre usar a Convergefy. Ver [Assistente](https://docs.convergefy.com.br/kb/assistente.md).
- **Assinatura** — O plano pago que mantém a empresa ativa. Ver [Cobrança](https://docs.convergefy.com.br/kb/cobranca.md).
- **Período de experiência (trial)** — Período em que a empresa já usa a plataforma antes da primeira cobrança da assinatura. A tela "Dados da empresa" mostra quanto falta.
- **Token de API** — Chave para integrar a Convergefy a outro sistema. Ver [Perfil e conta](https://docs.convergefy.com.br/kb/perfil-usuario.md).
- **Rastreamento (Meta Ads / Google Ads)** — Envio de conversões do CRM para os anúncios da Meta e do Google Ads, e medição da origem de cada contato. Antes chamada "Meta Ads". Ver [Rastreamento](https://docs.convergefy.com.br/kb/meta-ads.md).
- **Link rastreável** — Link de WhatsApp criado na Convergefy que registra o clique e a origem de quem chega por ele. Ver [Links rastreáveis](https://docs.convergefy.com.br/kb/links-rastreaveis.md).
- **Pixel** — Trecho de código instalado no seu site que identifica de qual anúncio a pessoa veio antes de ela abrir a conversa. Ver [Links rastreáveis](https://docs.convergefy.com.br/kb/links-rastreaveis.md).
