# Mensagens rápidas

Mensagens rápidas são modelos prontos — texto, áudio, imagem, vídeo ou documento — que sua equipe reaproveita no Chat com um clique ou com a tecla /, em vez de redigitar as respostas que se repetem todo dia.

Na Central de Ajuda: https://docs.convergefy.com.br/#/mensagens-rapidas

## Em resumo

Toda equipe tem respostas que se repetem: boas-vindas, instruções, tabela de preços, áudio de orientação. Em vez de redigitar (ou caçar o arquivo certo) toda vez, você salva uma **mensagem rápida** uma vez e a reaproveita no Chat com um clique.

Uma mensagem rápida pode ser texto, áudio, imagem, vídeo ou documento. Você não escolhe o tipo: ele sai do que você coloca na caixa de mensagem. Quem tem permissão cadastra tudo em Configurações → Estrutura operacional → **"Mensagens Rápidas"**; todos os membros usam as mensagens no Chat.

Escolher uma mensagem rápida no Chat **não envia nada ao cliente**. O texto cai no campo, e a imagem, o vídeo, o documento ou o áudio ficam esperando no campo até você enviar.

### Algo deu errado?

Procure o que você está vendo e siga a coluna da direita. O detalhe de cada caso está mais abaixo.

| O que você vê                                                                    | O que fazer                                                                                                                              |
| -------------------------------------------------------------------------------- | ---------------------------------------------------------------------------------------------------------------------------------------- |
| O botão "Salvar mensagem" (ou "Salvar", na edição) está apagado                  | Não é erro. Falta o título, falta o que enviar (texto, gravação ou arquivo) ou, numa mensagem existente, ainda não há nenhuma alteração. |
| _"Já existe uma mensagem rápida com esse nome."_                                 | Escolha outro título.                                                                                                                    |
| _"Não foi possível enviar o arquivo."_                                           | Confira formato e tamanho do arquivo (até 100 MB) e tente de novo.                                                                       |
| _"O arquivo anexado não está mais disponível. Anexe de novo."_                   | Remova o arquivo do campo, escolha-o de novo e salve.                                                                                    |
| O "/" não abre a lista                                                           | A barra só abre quando é a primeira coisa digitada num campo vazio. Veja "O atalho / no campo de digitação".                             |
| Aviso _A API oficial do WhatsApp não aceita "{nome}" como documento._            | Use esta mensagem rápida numa conversa do WhatsApp Web.                                                                                  |
| Não aparece o botão "Nova mensagem rápida"                                       | Criar, editar e excluir é de quem é Administrador ou tem o nível Administrar em Cadastros. Veja "Quem pode criar, editar e excluir".     |
| Escolhi uma mensagem com imagem, vídeo, documento ou áudio e ela não foi enviada | É o esperado: ela vira rascunho no campo até você enviar. Veja "O que acontece ao escolher".                                             |

> **Não é a mesma coisa que template da API Oficial**
>
> A **API Oficial** é o WhatsApp Business da Meta (também chamado WABA), um dos dois tipos de conexão. Os **templates** dela são mensagens aprovadas pela Meta, usadas só nessas conexões. As **mensagens rápidas** são internas da sua equipe, você cria à vontade e valem em qualquer conexão (com um limite para documentos na API Oficial, veja a seção "Limites e por quê").

**Conceitos rápidos**

- **Mensagem rápida** — O conteúdo salvo, um texto ou um arquivo, pronto para reaproveitar no Chat.
- **Legenda** — O texto que acompanha uma imagem, um vídeo ou um documento. É opcional. O áudio nunca leva texto.
- **Variável de contato** — Um dado do contato (como o primeiro nome) inserido no texto, que na hora de usar é trocado pelo dado do contato da conversa.
- **Favorita** — Mensagem marcada com a estrela. Ela sobe para o topo da lista e aparece numa faixa acima do campo de digitação.
- **Rascunho (não envia sozinho)** — Escolher uma mensagem rápida não dispara nada ao cliente: o texto cai no campo, e a imagem, o vídeo, o documento ou o áudio ficam esperando no campo até você enviar.

## Quem pode criar, editar e excluir

Todos os membros veem e usam as mensagens rápidas, na tela de Configurações e no Chat. Criar, editar e excluir é de quem é Administrador ou tem o nível **Administrar** na área "Cadastros" do acesso do membro (a mesma que cuida de departamentos, tags e produtos). Veja como definir isso em [Equipe e permissões](https://docs.convergefy.com.br/kb/equipe-permissoes.md).

Quem não tem essa permissão:

- não vê o botão "Nova mensagem rápida";
- vê, no lugar do menu do card, um ícone de olho ("Ver {nome}"), que abre a mensagem só para leitura, sem "Salvar" nem "Excluir";
- no Chat, não vê o "+ Nova" da lista nem o lápis de editar.

## Onde encontrar

Barra lateral → Configurações → seção Estrutura operacional → **"Mensagens Rápidas"**. A tela abre com o título "Mensagens Rápidas" e o texto _"Gerencie as mensagens rápidas que sua equipe pode usar no chat."_

No topo há um contador _"(N resultados)"_, uma busca "Buscar por nome ou conteúdo..." e um filtro por tipo: Todos, Texto, Áudio, Imagem, Vídeo, Documento. Cada mensagem aparece como um card com:

- o título e o menu "…" ("Opções de {nome}");
- o balão "como o contato recebe": o texto, o player do áudio, a miniatura da imagem ou do vídeo, ou o cartão do documento;
- embaixo, o tipo, por exemplo _"Imagem com legenda"_.

O card não mostra a data de criação; ela aparece ao abrir a mensagem. A lista carrega mais cards conforme você rola, até aparecer "Fim da lista".

## Criar uma mensagem rápida

1. **Abrir o painel** — Clique em **"Nova mensagem rápida"** (no celular, é o botão + ao lado da busca). Abre um painel à direita da tela, "Nova mensagem rápida", com o texto _"Escreva, anexe ou grave. O formato sai do que você colocar."_
2. **Dar um título** — O Título é obrigatório (ex.: _"Boas-vindas"_). É por ele que a equipe vai achar a mensagem na busca do Chat e no atalho /. Dois títulos iguais não são aceitos na mesma empresa.
3. **Escrever, anexar ou gravar** — Na caixa "Mensagem" você escreve o texto, anexa um arquivo ou grava um áudio, tudo na mesma caixa (veja a tabela abaixo). Abaixo dela, o bloco "Como o contato recebe" mostra a mensagem como ela chega no WhatsApp, com os dados de exemplo de um contato fictício (_"Exemplo com os dados de Maria Souza"_). Enquanto a caixa está vazia, ele diz _"Escreva ou anexe algo para ver a mensagem aqui."_
4. **Salvar** — Clique em **"Salvar mensagem"**. O botão só libera quando há título e alguma coisa para enviar (texto ou anexo). Aparece "Mensagem rápida criada com sucesso!", o painel fecha e a mensagem entra na lista.

**O que a caixa de mensagem aceita**

- **Texto** — Escreva no campo _"Escreva a mensagem. Use {{ para dados do contato"_. Sem anexo, a mensagem é só texto.
- **Imagem** — Botão "Imagem" (ou arrastar/colar o arquivo): JPG, PNG, GIF ou WebP. O texto da caixa vira a legenda (_"Escreva a legenda (opcional). Use {{ para dados do contato"_).
- **Vídeo** — Botão "Vídeo": MP4 ou 3GP. O texto da caixa vira a legenda.
- **Documento** — Botão "Documento": qualquer arquivo (até 100 MB). O documento tem legenda (o texto da caixa), e o card mostra _"Documento com legenda"_ quando você escreve uma.
- **Áudio** — Ícone de importar (_"Importar arquivo de áudio"_: OGG, WebM, MP3, M4A ou AAC) ou o microfone (_"Gravar áudio"_), à direita da barra de baixo. O áudio vai sozinho, sem texto, como no WhatsApp, por isso o microfone e a importação só funcionam com a caixa **vazia**. Com um áudio na caixa aparecem "Regravar" e "Remover áudio".

Detalhes que valem a pena saber:

- Um anexo só por mensagem. Escolher outro arquivo troca o anterior; para tirar, use o X ("Remover anexo"). Tirando o anexo, o texto que você escreveu continua e a mensagem vira texto.
- Arrastar um arquivo para a caixa mostra "Solte para anexar"; colar um arquivo também anexa.
- Se a caixa tem texto, o microfone avisa _"O áudio vai sozinho, sem texto. Apague o texto para gravar."_ Se já há um anexo, avisa _"Uma mensagem leva um anexo só. Remova o anexo para gravar."_
- No celular, os botões Imagem, Vídeo e Documento aparecem só com o ícone.

### Variáveis de contato

Para personalizar a mensagem, digite duas chaves abertas ({{) no texto, ou clique no botão de variável no canto da caixa. Abre uma lista com os dados do contato:

- **Nome do contato** — O nome completo.
- **Primeiro Nome** — Tudo até o primeiro espaço do nome.
- **Sobrenome** — O que vem depois do primeiro espaço.
- **Telefone do contato** — O telefone cadastrado.
- **E-mail do contato** — O e-mail cadastrado.
- **CPF/CNPJ do contato** — O documento cadastrado.
- **Endereço do contato** — O endereço cadastrado.
- **ID externo do contato** — O identificador do contato em outro sistema, quando houver.

Ao usar a mensagem numa conversa, cada variável é trocada pelo dado do contato daquela conversa, e o texto cai no campo já preenchido, para você revisar. Se o contato não tem aquele dado, a variável sai vazia: o cliente nunca recebe o código cru.

Num grupo de WhatsApp não há um contato para preencher, então cada variável entra entre colchetes, como \[Primeiro Nome], para você completar à mão antes de enviar.

## Ver e editar uma mensagem

Clique em qualquer ponto do card ou, no menu "…" do card, em "Editar". Abre um painel à direita com a mensagem:

- No topo: o ícone do tipo, o título (que se edita ali mesmo, clicando nele) e _"Criada em"_ com a data.
- O mesmo editor da criação (caixa de mensagem com os botões de anexar e gravar) e o bloco "Como o contato recebe" logo abaixo.
- No rodapé: "Excluir", "Cancelar" e "Salvar".

Nada é salvo sozinho: as alterações ficam pendentes até você clicar em **"Salvar"**, que mostra "Mensagem rápida atualizada com sucesso!" e mantém o painel aberto com a versão nova (se um filtro de tipo estiver ligado e esconder o novo tipo, a mensagem sai da lista e o painel fecha). "Cancelar" desfaz o que não foi salvo, sem fechar o painel. Os dois só ficam ativos quando há alguma alteração.

Para trocar o formato (por exemplo, de texto para imagem), basta anexar o novo arquivo; para voltar a texto, remova o anexo.

> **Fechar com alteração pendente pede confirmação**
>
> Se você fechar o painel (no X, no Esc ou clicando fora) com algo ainda não salvo, aparece "Descartar alterações?" com o texto _"O que foi preenchido ainda não foi salvo."_ Escolha "Continuar editando" para voltar ou "Descartar" para fechar sem salvar. Vale também no painel de criação, inclusive no botão "Cancelar".

## Usar no Chat

No Chat há quatro caminhos para usar uma mensagem rápida, e todos levam ao mesmo resultado: a mensagem cai no campo de envio e você decide quando enviar.

### O atalho / no campo de digitação

Num campo vazio, digite **/** (o campo diz _"Mensagem ou / para atalhos"_). Abre uma lista colada ao campo; continue digitando para filtrar. Use ↑ ↓ para navegar, Enter para usar o item destacado e Esc para fechar (a barra fica no campo como texto comum).

**Regras do atalho / (quando abre, fecha e busca)**

- **Quando abre** — Só quando a barra é a primeira coisa digitada num campo vazio. Uma barra no meio do texto (datas, "e/ou", links) não abre. Colar um texto que começa com "/" também não.
- **Quando fecha** — Se você digita um espaço logo depois da barra, se apaga a barra ou quebra a linha. Um espaço depois de uma letra não fecha: o título pode ter mais de uma palavra.
- **Como busca** — Pelo título, sem diferenciar maiúscula nem acento. Quem começa com o que você digitou vem primeiro.
- **Sem resultado** — Aparece o aviso de que não há nenhuma mensagem rápida com o que você digitou (e, com mais de um bloco, o mesmo para templates e automações), junto de _"Enter envia o texto como está"_: o Enter manda o que você digitou, barra incluída.
- **Onde não abre** — Em nota interna, ao editar uma mensagem já enviada, enquanto você grava um áudio e quando já há uma mídia de mensagem rápida esperando no campo.

Em uma conversa de API Oficial (que não seja grupo), a lista ganha o bloco "Templates", com os templates aprovados que dá para enviar. Em qualquer conversa fora de grupo, ela ganha também o bloco "Automações manuais".

- Escolher um template abre o formulário dele para preencher e enviar.
- Escolher uma automação pede a mesma confirmação do botão de automações.
- Com mais de um bloco, a ordem é sempre: mensagens rápidas, templates, automações manuais.

### O botão ⚡ "Mensagens rápidas"

O botão de raio ao lado do campo abre o painel "Mensagens Rápidas", com os Favoritos no topo e Todas logo abaixo. No cabeçalho:

- **+ Nova** — Cria uma mensagem rápida na hora, numa janela ("Nova mensagem rápida", com o botão "Salvar mensagem") com os mesmos campos da criação em Configurações. Só aparece para quem pode criar.
- **Buscar...** — Filtra por nome ou conteúdo. Sem resultado, aparece _"Nenhum resultado."_; sem nenhuma cadastrada, _"Nenhuma mensagem rápida."_
- **Filtro por tipo** — Restringe a lista a um tipo (texto, áudio, imagem, vídeo, documento), útil quando você sabe que procura um arquivo.

Cada item tem uma estrela (favoritar/desfavoritar) e, para quem pode editar, um lápis ("Editar {título}") que abre a edição numa janela, com o botão "Excluir" dentro dela. O lápis aparece ao passar o mouse; no toque, fica sempre à vista.

### A faixa de favoritas

Acima do campo de digitação, as mensagens rápidas e as automações favoritas aparecem como cartões que deslizam de lado. Clicar num cartão de mensagem rápida usa a mensagem; num cartão de automação, pede a confirmação para executá-la.

- Em grupo, a faixa mostra só as mensagens rápidas favoritas: as automações não aparecem.
- Enquanto você digita no campo, os cartões filtram pelo que foi escrito; se nenhum combina, aparece _"Nenhum favorito corresponde à busca"_.
- Sem nenhuma favorita, a faixa não aparece.

> **Favoritos deixam o dia a dia mais rápido**
>
> Favoritar é uma estrela no próprio item do painel: clique nela e a mensagem sobe para o grupo Favoritos, no topo, e ganha um cartão na faixa. Não é uma configuração escondida em outra tela: dá para marcar e desmarcar no meio do atendimento, conforme a semana muda.

### O que acontece ao escolher

- **Texto:** o conteúdo é inserido no campo de envio, com as variáveis já preenchidas. Você ainda revisa e envia.
- **Imagem, vídeo ou documento:** a mídia não é enviada na hora. Ela vira um rascunho no campo: uma faixa "Mensagem rápida", com a miniatura e o título (no documento, o nome do arquivo), aparece acima do campo, e a legenda da mensagem entra no próprio campo (_"Adicione uma legenda..."_), onde você pode editá-la. O envio é seu, com o botão de enviar ou o Enter. Para desistir, use o X da faixa ("Descartar mensagem rápida").
- **Áudio:** também vira rascunho na faixa, mas sem campo de legenda. Para desistir, use o X da faixa ou a tecla Esc.

O rascunho fica preso à conversa em que foi escolhido: se você trocar de conversa sem enviar, ele não vai junto para outro contato.

> **Documento que a API Oficial não aceita**
>
> Numa conversa de API Oficial, a Meta não aceita alguns tipos de documento (por exemplo ZIP ou CSV). Ao escolher uma mensagem com um documento assim, nada é anexado e aparece o aviso _A API oficial do WhatsApp não aceita "{nome}" como documento. Use esta mensagem rápida numa conversa do WhatsApp Web._

Mensagens rápidas, áudios e arquivos também funcionam em grupos (nos grupos, o "/" não mostra templates nem automações). Também dá para agendar uma mensagem rápida para sair depois (ver [Atendimento / Chat](https://docs.convergefy.com.br/kb/chat.md)).

## Limites e por quê

**Tamanhos e formatos de arquivo**

- Qualquer arquivo: até **100 MB**.
- É exatamente o mesmo limite do Chat: uma mensagem rápida acaba sendo enviada pelo WhatsApp como qualquer outra.
- A checagem acontece na hora de anexar, com um aviso na tela: _"O arquivo passa do limite de 100 MB."_, ou, para um formato não aceito, _"Formato não aceito. Use JPG, PNG, GIF ou WebP."_ (imagem), _"…Use MP4 ou 3GP."_ (vídeo) e _"…Use OGG, WebM, MP3, M4A ou AAC."_ (áudio). Se houver texto na caixa e você tentar anexar um áudio: _"O áudio vai sozinho, sem texto. Apague o texto para anexar um áudio."_
- O título vai até 255 caracteres e o texto até 65.535.
- Em conexão da API Oficial, o WhatsApp aplica tetos menores por tipo: imagem 5 MB, vídeo e áudio 16 MB, documento 100 MB.
  - Antes de enviar, a plataforma ajusta sozinha o que dá: JPEG e PNG acima de 5 MB são reduzidos, GIF vira MP4 e áudio fora do formato aceito vira OGG.
  - Vídeo e documento acima do teto (e o que o ajuste não resolver) são aceitos aqui, mas a Meta recusa na entrega. Ver [Atendimento / Chat](https://docs.convergefy.com.br/kb/chat.md).

## Excluir uma mensagem

> **Excluir só remove da galeria da equipe**
>
> Isso só remove a mensagem da galeria da equipe. Não afeta mensagens já enviadas em conversas.

No menu "…" do card, escolha "Excluir", ou use o botão "Excluir" no rodapé do painel da mensagem. Aparece a confirmação "Excluir mensagem rápida?". Confirmando em "Excluir", o sistema responde "Mensagem rápida excluída com sucesso.", a mensagem some da lista e, se o painel estava aberto, ele fecha.

## Erros e avisos esperados

Se o "Salvar mensagem" (ou o "Salvar", na edição) estiver apagado, não é erro: falta o título, falta o que enviar (texto, gravação ou arquivo) ou, numa mensagem existente, ainda não há nenhuma alteração.

- “Título é obrigatório” — o título ficou em branco. Resolver: preencha o título e salve de novo.
- “Já existe uma mensagem rápida com esse nome.” — cada mensagem precisa de um nome próprio na empresa. Resolver: escolha outro título.
- “Não foi possível enviar o arquivo.” — o arquivo não subiu, e a mensagem não foi salva. Resolver: confira formato e tamanho do arquivo (até 100 MB) e tente de novo.
- “O arquivo anexado não está mais disponível. Anexe de novo.” — o arquivo que estava no formulário deixou de existir antes de salvar. Resolver: remova o arquivo do campo, escolha-o de novo e salve.
- “Não foi possível criar a mensagem rápida.” — falha ao criar a mensagem. Resolver: confira sua internet e tente criar de novo; se o conteúdo for arquivo, confirme formato e tamanho.
- “Não foi possível atualizar a mensagem rápida.” — falha ao salvar as alterações de uma mensagem existente. Resolver: tente salvar a edição de novo.
- “Não foi possível excluir a mensagem rápida.” — falha ao remover a mensagem. Resolver: tente excluir de novo; se persistir, recarregue a página.
- “Nenhuma mensagem rápida encontrada” — a lista de Configurações está vazia para o filtro atual (não é um erro de fato). Resolver: ajuste a busca ou o filtro de tipo; quem pode criar também vê a sugestão de criar uma nova mensagem rápida.
- “Nenhuma mensagem rápida. / Nenhum resultado.” — no Chat, não há mensagens (ou a busca não achou nada). Resolver: crie mensagens em Configurações (se você tiver permissão), ou limpe a busca dentro do painel.
