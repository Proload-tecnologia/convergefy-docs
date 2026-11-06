# Agentes de IA

Um agente de IA é um atendente virtual que a sua empresa cria e ensina: ele responde direto nas conversas do WhatsApp, com o jeito, as informações e as ações que você definiu.

Na Central de Ajuda: https://docs.convergefy.com.br/#/agentes-ia

## Em resumo

Um **agente de IA** é um atendente virtual que a sua empresa monta e treina. Você escreve como ele atende (instruções), o que ele sabe (base de informações), o que ele pode enviar (mídias) e o que ele pode fazer no atendimento e no CRM (ações, como aplicar tag ou transferir).

Depois de **publicado**, ele atende direto nas conversas. Há três jeitos de colocar o agente numa conversa, explicados em [O agente nas conversas](https://docs.convergefy.com.br/kb/agentes-ia-conversas.md):

- pela **conexão**: o agente atende as conversas novas daquele número;
- pelo **chat**: um atendente atribui o agente a uma conversa;
- por uma **automação**: o bloco "Transferir para agente de IA" passa a conversa para ele, por exemplo depois de um menu de triagem.

Para retomar conversas de quem parou de responder, use os [Follow-ups](https://docs.convergefy.com.br/kb/agentes-ia-follow-ups.md).

> **Três coisas com nomes parecidos**
>
> Os **Agentes** deste guia são a versão nova. Os [Agentes de automação](https://docs.convergefy.com.br/kb/agentes-ia-automacao.md) são a versão anterior, que só conversa dentro de uma automação e continua funcionando. O [Assistente](https://docs.convergefy.com.br/kb/assistente.md) (a Letícia) responde as suas dúvidas sobre a plataforma, não fala com o seu contato.

### Algo deu errado?

Procure o que você está vendo e siga a coluna da direita. O detalhe de cada caso está mais abaixo.

| O que você vê                                                     | O que fazer                                                                                                                                                                                                               |
| ----------------------------------------------------------------- | ------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------- |
| O agente está "Atendendo", mas não fala com ninguém               | Ele só responde conversas em que foi colocado: ligue-o numa conexão, atribua no chat ou use o bloco "Transferir para agente de IA". Veja [O agente nas conversas](https://docs.convergefy.com.br/kb/agentes-ia-conversas.md). |
| Você mudou o agente e o atendimento não mudou                     | Salve e use "Publicar alterações". As conversas usam o que está publicado.                                                                                                                                                |
| "Publicar" não publica e abre "Falta completar antes de publicar" | Resolva cada item da lista (nome, instruções, menções sem valor ou salvar).                                                                                                                                               |
| "Escreva as instruções do agente antes de publicar."              | Escreva as instruções na aba "Instruções ao LLM", salve e publique.                                                                                                                                                       |
| O teste não mostra o que você acabou de mudar                     | O teste roda o que está salvo. Clique em "Salvar" antes de testar.                                                                                                                                                        |
| Chip "Item removido" ou "Valor removido" nas instruções           | O que ele citava foi apagado. Clique no chip e escolha outro valor, ou apague a menção.                                                                                                                                   |
| Habilidade com "não citada, o agente não usa"                     | Use "Citar nas instruções" ou cite com @ no ponto certo das instruções.                                                                                                                                                   |
| Fonte da base em "Erro: …"                                        | Use "Reprocessar". Se continuar, troque o arquivo ou cole o conteúdo como texto.                                                                                                                                          |
| "Arquivo acima de 25 MB" (base) ou "…até 100 MB" (mídias)         | Reduza o arquivo. Na base, dá para colar só o texto com "Adicionar texto".                                                                                                                                                |

## Como funciona, em 4 passos

1. **Criar** — Em "IA" → "Agentes", clique em **"Criar agente"** e dê um nome.
2. **Ensinar** — Escreva as instruções (o Builder ajuda), e, se precisar, crie habilidades, adicione fontes à base de informações e mídias para enviar. Clique em **"Salvar"**.
3. **Testar** — No painel lateral, use **"Testar"** para conversar com o agente como se fosse um contato, sem afetar conversas reais.
4. **Publicar e colocar para atender** — Clique em **"Publicar"**. Depois ligue o agente numa conexão, atribua no chat ou use o bloco "Transferir para agente de IA" (ver [O agente nas conversas](https://docs.convergefy.com.br/kb/agentes-ia-conversas.md)).

**Conceitos rápidos**

- **Instruções** — O texto que diz ao agente quem ele é, como fala, o que persegue e como conduz a conversa.
- **Habilidade** — Um bloco de instrução que o agente só lê quando a conversa chega no ponto em que ela é citada. Serve para o que só importa em parte das conversas.
- **Base de informações** — Arquivos e textos que o agente consulta para responder. A cada mensagem do contato, ele busca os trechos mais parecidos com ela.
- **Mídias** — Arquivos que o agente pode enviar ao contato na conversa.
- **Menção (@)** — O jeito de citar, dentro das instruções, uma ação, uma habilidade, uma mídia ou uma fonte da base.
- **Publicar** — Grava uma cópia da configuração salva e põe o agente para atender. As conversas sempre usam a cópia publicada.
- **Agente responsável** — O agente que responde uma conversa. Ele responde toda mensagem do contato até sair dela, por exemplo quando um atendente responde (ver [O agente nas conversas](https://docs.convergefy.com.br/kb/agentes-ia-conversas.md)).

## Onde fica e quem acessa

Na barra lateral, abra o menu **"IA"**. Ele mostra três opções:

- **"Agentes"** (com o selo "Novo"): _"Atendem direto nas conversas, com instruções, habilidades e base próprias."_ É este guia.
- **"Follow-ups"**: _"Retomam conversas de quem parou de responder."_ Veja [Follow-ups](https://docs.convergefy.com.br/kb/agentes-ia-follow-ups.md).
- **"Agentes de automação"**: _"Usados no passo Agente de automação (antigo) das suas automações."_ Veja [Agentes de automação](https://docs.convergefy.com.br/kb/agentes-ia-automacao.md).

O menu aparece para o Administrador e para quem tem o nível Administrar na área "Agentes de IA" (ver [Equipe e permissões](https://docs.convergefy.com.br/kb/equipe-permissoes.md)). Quem não tem esse nível não cria nem edita agentes, mas ainda vê a lista de agentes onde precisa escolher um, como no editor de automações e no chat.

Tela **"Agentes"**: _"Automatize o atendimento com agentes que conversam, qualificam e agendam."_ Cada agente é um cartão com avatar, nome, selo de estado e o modelo de IA. Clique no cartão para abrir a configuração. Sem nenhum agente: _"Nenhum agente ainda"_, _"Crie o primeiro agente para atender direto nas conversas."_

**Estado de cada agente**

- **Atendendo** (green) — publicado e ativo: responde as conversas em que está.
- **Pausado** (amber) — publicado, mas parado. Continua responsável pelas conversas em que está, só não responde.
- **Rascunho** (gray) — nunca foi publicado. Só existe em construção e não atende ninguém.

No menu "⋮" do cartão: um rascunho só tem "Excluir rascunho"; um agente atendendo tem "Testar", "Pausar" e "Excluir"; um pausado tem "Testar", "Retomar" e "Excluir". "Pausar" e "Retomar" valem na hora, sem confirmação.

## Criar um agente

1. **Abrir** — Em "IA" → "Agentes", clique em **"Criar agente"**. Abre **"Criar agente"**: _"O resto você configura em seguida."_
2. **Dar um nome** — Preencha **"Nome"** (até 60 caracteres, ex.: _"Suporte, Pré-vendas, Recuperação"_). O nome _"Serve para você achar o agente na lista. Como ele se apresenta aos contatos fica em Identidade, nas instruções."_ Não dá para repetir o nome de outro agente da empresa (o campo avisa _"Já foi utilizado."_).
3. **Criar** — Clique em **"Criar"**. O agente nasce como **rascunho**, com instruções-modelo divididas nas seções Identidade, Jeito de falar, Objetivo, Passo a passo e Limites, cada uma com uma dica entre colchetes. A configuração abre com o Builder pronto para conversar.

> **O nome não é o jeito de se apresentar**
>
> O agente nunca diz o nome da lista ao contato. Se ele deve se apresentar ("Oi, aqui é a Ana, do comercial"), escreva isso na seção Identidade das instruções.

## A página de configuração

No topo ficam o nome (clique no lápis para mudar), o selo de estado e os botões de salvar e publicar. Do lado esquerdo, o painel com **"Builder"** e **"Testar"** (dá para recolher com "Recolher painel"). No centro, as abas:

| Aba                   | Para que serve                                                 |
| --------------------- | -------------------------------------------------------------- |
| "Instruções ao LLM"   | O texto principal de como o agente atende, com as menções (@). |
| "Habilidades"         | Blocos de instrução lidos só quando a conversa chega neles.    |
| "Base de informações" | O que o agente sabe para responder: arquivos e textos.         |
| "Mídias"              | Arquivos que ele pode enviar ao contato.                       |
| "Config. LLM"         | Modelo, ritmo da conversa e ferramentas que ele pode usar.     |
| "Horários"            | Quando ele atende e o que faz fora do horário.                 |

> **Nada salva sozinho**
>
> As mudanças só ficam gravadas quando você clica em **"Salvar"** (ou desfaz com "Descartar"). Se tentar sair com mudanças, aparece _"Sair sem salvar?"_: "Continuar aqui" mantém você na tela, "Sair e perder" descarta.

Enquanto falta algo para publicar, o topo mostra uma linha como _"Falta: nome, instruções, menções sem valor, salvar"_, só com o que se aplica.

### Instruções ao LLM

_"Tudo que o agente precisa saber para conduzir a conversa, num texto só. Digite @ para inserir ações, habilidades, mídias e fontes da base."_

- **"Adicionar seção"** insere um título com uma dica, entre: Identidade, Jeito de falar, Objetivo, Passo a passo, Objeções, Passar para um atendente, Limites, Formato das mensagens e Exemplos. Só aparecem as seções que ainda não estão no texto.
- O contador mostra quantos caracteres o texto tem. O limite é de 50.000 caracteres, e cada menção (@) ocupa mais espaço do que mostra.

**Menções (@).** Digite **@** no texto para citar algo no ponto exato da conversa. A legenda embaixo do editor resume os tipos: **ação** _"faz algo no atendimento ou no CRM"_, **habilidade** _"sabe alguma coisa"_, **fonte** _"orienta a consulta"_, **mídia** _"envia ao contato"_.

- **Aplicar tag** — Marca o contato com uma tag que você escolhe.
- **Transferir atendimento** — Passa a conversa para um departamento ou atendente. Dá para escolher "Deixar a IA decidir".
- **Criar negócio** — Abre um negócio num funil e etapa que você escolhe, ou "Deixar a IA decidir".
- **Mover negócio** — Troca o negócio de etapa, se o contato já tiver um. Funil e etapa fixos ou "Deixar a IA decidir".
- **Finalizar atendimento** — Encerra a conversa.

Para enviar um arquivo num ponto certo, escolha o tipo **Mídias** no @ e o arquivo. Clique num chip para trocar o valor ou removê-lo. Quando o que o chip citava é apagado, ele vira _"Item removido"_ ou _"Valor removido"_. Numa ação, mídia ou fonte, isso conta como **menção sem valor** e impede publicar até você corrigir. Uma habilidade apagada não impede publicar, mas naquele ponto o agente não consulta nada.

### Habilidades

_"Blocos de instrução que o agente só lê quando chega no @ que chama cada um."_ Use para o que só importa em parte das conversas, como qualificação de lead, tabela de preços ou troca de plano.

1. **Criar** — Clique em **"Criar habilidade"** e preencha os três campos abaixo.
2. **Salvar** — Clique em **"Salvar"** no topo. Uma habilidade nova só pode ser citada depois de salva.
3. **Citar** — Nas instruções, digite @ e escolha a habilidade no ponto em que o agente deve lê-la.

- **Nome (até 40 caracteres)** — _"É o nome que aparece no @. Se mudar, as instruções acompanham."_
- **Quando usar (até 140 caracteres)** — _"O agente lê isto para decidir se vale abrir a habilidade."_
- **Conteúdo** — O que o agente deve fazer quando a habilidade é chamada. Aceita @ de ações, mídias e fontes, mas não de outra habilidade.

Cada habilidade mostra **"citada nas instruções"** ou **"não citada, o agente não usa"**. Habilidade não citada nunca é lida: use **"Citar nas instruções"** para incluir a citação no fim do texto e depois ajuste a frase. Excluir uma habilidade salva vale na hora e não dá para desfazer. Se ela estava citada, _"Nesses pontos o agente deixa de consultar qualquer coisa."_

### Base de informações

_"O que o agente sabe para responder o contato. Para enviar arquivos ao contato, use a aba Mídias."_

- **Arquivos**: clique ou arraste em _"Clique para selecionar ou arraste arquivos"_. Aceita PDF, TXT, MD, CSV, JSON ou XML, imagens (JPEG, PNG, WEBP, GIF) e áudios (MP3, M4A, OGG, WAV, WEBM), **até 25 MB** cada. DOC e DOCX não são aceitos: exporte em PDF.
- **Texto**: **"Adicionar texto"** abre _"Adicionar fonte de texto"_: um **"Título"** opcional e o **"Conteúdo"** colado.
- "Adicionar URL" ainda não está disponível (_"Em breve: ainda não lemos páginas da web."_).

Cada fonte é convertida em texto automaticamente. _"A cada mensagem do contato, o agente busca nas fontes em uso os 6 trechos mais parecidos com ela. Fonte que ainda está processando fica de fora da busca até terminar."_

**Estado de cada fonte**

- **Processando…** (gray) — sendo convertida em texto. A lista atualiza sozinha.
- **Em uso** (green) — pronta e ligada: entra na busca do agente.
- **Pronto · pausado** (gray) — pronta, mas desligada no interruptor "Usar esta fonte".
- **Erro: …** (red) — não deu para ler o arquivo. O motivo aparece ao lado. Como resolver: use Reprocessar; se continuar, troque o arquivo ou cole o texto.

O olho ("Ver conteúdo convertido") mostra o texto que o agente lê. O conteúdo de uma fonte não é editável: para mudar, remova e adicione de novo. Uma fonte citada com @ mostra "Citada no texto", ou "Citada, mas fora de uso" se estiver desligada ou com erro.

### Mídias

_"O que o agente pode enviar ao contato na conversa. O que ele precisa saber para responder fica na Base de informações."_

- Envie imagem, vídeo, áudio ou documento, **até 100 MB**. Imagem (JPEG, PNG, WEBP), vídeo (MP4, 3GP) e áudio (AAC, AMR, MP3, MP4, OGG) precisam estar num formato que o WhatsApp aceita. Qualquer outro arquivo vai como documento.
- Em cada mídia, o campo **"Quando enviar"** (até 500 caracteres) diz ao agente em que situação mandar o arquivo. Ele é gravado quando você clica em "Salvar".
- Para enviar num ponto certo do roteiro, cite a mídia com @ nas instruções. A mídia mostra "Citada nas instruções" ou "Não citada, o agente envia só pela descrição".

Para trocar um arquivo, remova a mídia e envie outra. Onde ela estava citada, o agente não envia nada.

### Config. LLM

_"Quem pensa pelo agente, o ritmo da conversa e o que ele pode fazer."_ Estas configurações _"passam a valer depois de publicar, inclusive nas conversas em andamento"_.

- **Modelo** — Só leitura: _"Definido pelo Convergefy. Não muda o que o agente diz, muda o quanto ele consegue seguir um roteiro longo."_
- **Esperar antes de responder** — O agente espera o contato terminar de escrever e lê tudo de uma vez. Opções: "Padrão" (5 a 6 segundos), "5 s", "10 s", "30 s", "1 min" e "5 min". A espera recomeça a cada nova mensagem do contato.
- **Mostrar “digitando…” antes de enviar** — Ligado por padrão. _"Só no WhatsApp Web. Na API Oficial o agente espera o mesmo tempo, sem o aviso na tela do contato."_ A espera acompanha o tamanho da mensagem, até 8 segundos por mensagem.
- **Ferramentas** — Liga ou desliga o que o agente pode fazer. Desligada, ele _"nem sabe que isso é possível"_.

**O que cada ferramenta faz**

| Ferramenta                           | O que faz                                                                                                 |
| ------------------------------------ | --------------------------------------------------------------------------------------------------------- |
| Responder o cliente                  | Manda texto ao contato. Desligada, o agente só lê e age pelas outras ferramentas, em silêncio.            |
| Consultar dados do cliente           | Lê nome, telefone e o cadastro do contato.                                                                |
| Consultar situação no funil          | Vê em que funil e etapa o contato está.                                                                   |
| Consultar departamentos e atendentes | Lista para quem transferir. Só funciona com "Transferir atendimento" ligado.                              |
| Consultar funis e etapas             | Lista onde criar ou mover um negócio. Só funciona com "Criar negócio" ou "Mover negócio de etapa" ligado. |
| Pedir atendimento humano             | Passa a conversa para os atendentes: o agente sai do chat e para de responder.                            |
| Encerrar sessão                      | Encerra a conversa do momento. O agente continua responsável e volta a responder se o contato escrever.   |
| Aplicar tag                          | Marca o contato com uma tag, quando as instruções mandarem.                                               |
| Transferir atendimento               | Passa a conversa para um departamento, um atendente, ou os dois.                                          |
| Finalizar atendimento                | Encerra o atendimento do contato.                                                                         |
| Criar negócio                        | Abre um negócio para o contato, com o nome dele.                                                          |
| Mover negócio de etapa               | Muda um negócio do contato de etapa.                                                                      |
| Fechar negócio                       | Fecha um negócio do contato como ganho ou perdido.                                                        |
| Enviar arquivo                       | Envia uma das mídias do agente. Fica indisponível sozinha quando ele não tem nenhuma.                     |
| Abrir habilidade                     | Abre o conteúdo de uma habilidade citada, quando a conversa chega nela.                                   |

### Horários

_"Quando o agente atende. Fora do horário ele não passa a conversa adiante: segue o que você escrever para esse caso."_

Sem horário, o agente atende a qualquer hora. Para limitar, ligue **"Limitar horário de atendimento"** e preencha:

- **Dias e horários** — Os dias e faixas em que ele atende (a sugestão inicial é segunda a sexta, 08:00 às 17:00). _"Só os dias adicionados contam como abertos."_
- **Fuso horário** — _"Os horários acima são lidos neste fuso."_
- **O que o agente faz fora do horário** — Até 2.000 caracteres, ex.: _"diga que voltamos às 8h e não mande mais nada."_ _"Vazio, ele avisa uma vez que está fora do horário e quando volta. Para ele não responder nada, escreva isso aqui."_
- **Concluir atendimentos em andamento** — _"A conversa que o agente já atendia dentro do horário continua até terminar."_ Desligado por padrão.

**Como o horário é contado**

Vale a hora em que o contato escreveu, no fuso escolhido. Fora do horário, o agente continua responsável pela conversa e segue o que você escreveu para esse caso: quem escreve a resposta é a IA, então o resultado depende do seu texto. Quando um atendente atribui o agente pelo chat, o horário não vale para aquela conversa.

## Builder e Testar

**Builder.** Uma IA que conversa com você e escreve as instruções junto: _"Me conte o que sua empresa vende e o que esse agente precisa resolver. Eu escrevo as instruções com você."_ Ele também propõe e ajusta habilidades.

- Tudo o que ele muda aparece no editor e pode ser editado. Para valer, clique em **"Salvar"**.
- Dá para anexar imagem, PDF, TXT ou MD (até 25 MB cada, 5 por mensagem). Quando você pede para guardar um anexo como fonte da base ou como mídia, ele é gravado na hora.
- **"Escolher conversas"**: _"O agente aprende com elas o jeito da casa de atender. Escolha até 10."_

**Testar.** Converse com o agente escrevendo _"como um contato"_. _"O agente responde com a configuração atual, sem afetar conversas reais."_

- O teste roda **o que está salvo**. Com mudanças não salvas: _"Salve as alterações para testar o agente: o teste roda o que está gravado, não o que está na tela."_
- Nada vai para o WhatsApp e nenhuma ação acontece de verdade. Abaixo da resposta, _"O que aconteceu na última resposta"_ lista o que ele teria feito (ex.: "Aplicou", "Transferiu", "Pediu atendimento humano").
- O teste não simula a espera antes de responder, o "digitando…" nem o horário de atendimento.
- "Recomeçar teste" começa uma conversa nova.

## Publicar, pausar e retomar

1. **Salvar** — Clique em **"Salvar"** depois de mudar qualquer coisa.
2. **Publicar** — Num rascunho, clique em **"Publicar"**. O agente passa a "Atendendo". Em um agente que já atende, as mudanças salvas só chegam às conversas depois de **"Publicar alterações"**.

Se faltar algo, o botão abre _"Falta completar antes de publicar"_ com os itens: "Dar um nome ao agente", "Escrever as instruções", "Corrigir menções sem valor" e "Salvar as alterações". Clique no item para ir até ele.

**Pausar** para o agente de responder na hora e encerra o que ele estava respondendo. As conversas continuam com ele como responsável: depois de **"Retomar"**, ele volta a responder quando o contato escrever de novo. Pausado, ele não pode ser atribuído pelo chat nem escolhido em automação. Se estiver ligado a uma conexão, continua entrando nas conversas novas dela, mas calado.

> **Retomar também publica**
>
> "Retomar" publica o que estiver salvo. Por isso ele pede as mesmas condições de "Publicar" (_"Falta completar antes de retomar"_), e as mudanças salvas passam a valer na hora, inclusive quando você retoma pelo menu do cartão.

> **O que espera a publicação**
>
> Instruções, habilidades, Config. LLM e horários só valem depois de publicar. As fontes da base e as mídias valem assim que ficam prontas.

## Excluir um agente

> **Não dá para desfazer**
>
> _"“NOME” e tudo que foi configurado nele somem. Não dá para desfazer."_ Excluir encerra as conversas que ele estava respondendo, tira o agente das conversas e das conexões em que estava e para os follow-ups dele. Se for só uma pausa, use "Pausar".

No menu "⋮" do cartão, clique em **"Excluir"** (ou **"Excluir rascunho"**) e confirme em "Excluir agente".

## Erros e avisos esperados

- “Escreva as instruções do agente antes de publicar.” — o agente não tem instruções. Resolver: escreva as instruções, salve e publique de novo.
- “Já existe um agente com esse nome.” — ao renomear, outro agente da empresa já usa esse nome. Ao criar, o campo "Nome" mostra _"Já foi utilizado."_ Resolver: escolha outro nome.
- “Não salvou: …” — parte da configuração não foi gravada. Resolver: confira os campos citados e clique em Salvar de novo.
- “Já existe uma habilidade com esse nome” — o nome repete o de outra habilidade do agente. Resolver: dê outro nome à habilidade.
- “Este arquivo não pode ser usado como fonte. Confira o tipo e o tamanho (até 25 MB).” — o tipo ou o tamanho não é aceito na base. Resolver: exporte em PDF, reduza o arquivo ou use Adicionar texto.
- “Este arquivo não pode ser enviado como mídia. Confira o tipo e o tamanho (até 100 MB).” — o tipo ou o tamanho não é aceito em Mídias. Resolver: converta para um formato aceito pelo WhatsApp ou reduza o arquivo.
- “Algo deu errado. Tente de novo.” — o teste não conseguiu gerar a resposta. Resolver: clique em Tentar de novo; se repetir, recomece o teste.
