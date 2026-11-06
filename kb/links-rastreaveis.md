# Links rastreáveis

Um link rastreável abre o WhatsApp com uma mensagem já digitada e, ao mesmo tempo, registra de onde cada lead veio — do seu site ou de um anúncio. Você cria o link, cola no botão da sua página (ou usa o botão flutuante pronto) e acompanha cliques e conversas geradas.

Na Central de Ajuda: https://docs.convergefy.com.br/#/links-rastreaveis

## Em resumo

Um link rastreável é um link de WhatsApp com duas funções ao mesmo tempo: abre a conversa com um número seu já com uma mensagem digitada, e registra a origem de quem clicou (de qual página do seu site ou de qual anúncio a pessoa veio). Cada lead que chega pelo link já entra sabendo de onde veio, e essa origem alimenta o [Rastreamento](https://docs.convergefy.com.br/kb/meta-ads.md) (conversões para Meta e Google Ads).

1. **Instalar o pixel (uma vez)** — Cole o pixel no site para o link identificar a origem. Veja "Instalar o pixel (uma vez)", abaixo.
2. **Criar o link** — Clique em **"Novo link"**, escolha o nome, a conexão de WhatsApp e a mensagem inicial.
3. **Colocar o link para circular** — Cole o link no botão de WhatsApp do seu site, ou use o botão flutuante pronto.
4. **Acompanhar** — Veja "Cliques" e "Conversas" na lista de links.

### Algo deu errado?

Procure o que você está vendo e siga a coluna da direita. O detalhe de cada caso está mais abaixo.

| O que você vê                                                                          | O que fazer                                                                                                                                     |
| -------------------------------------------------------------------------------------- | ----------------------------------------------------------------------------------------------------------------------------------------------- |
| O botão "Novo link" não aparece                                                        | Criar, editar e desativar links exige o nível Administrar em Rastreamento. Peça a um Administrador.                                             |
| _"Informe um nome para o link."_                                                       | Preencha o campo "Nome".                                                                                                                        |
| _"Selecione a conexão de WhatsApp destino."_                                           | Escolha uma conexão no campo "Conexão de WhatsApp".                                                                                             |
| _"Escreva a mensagem inicial."_                                                        | Preencha a "Mensagem inicial".                                                                                                                  |
| "Nenhuma conexão disponível" (_"Conecte um WhatsApp em Conexões para criar um link."_) | A empresa não tem nenhuma conexão cadastrada. Conecte um número em [Conexões de WhatsApp](https://docs.convergefy.com.br/kb/conexoes.md).           |
| _"A conexão escolhida não tem telefone para o link do WhatsApp."_                      | A conexão escolhida não tem telefone. Escolha outra no campo "Conexão de WhatsApp".                                                             |
| O link abre o WhatsApp, mas não mostra de qual anúncio o contato veio                  | O pixel não está instalado no site. Sem ele, o link redireciona e conta cliques, mas não registra o anúncio. Veja "Instalar o pixel (uma vez)". |
| O link foi colado como texto e não registra a origem                                   | Cole o link no destino do botão (o atributo href), nunca só como texto. Veja "No seu site".                                                     |
| O link parou de abrir o WhatsApp e tem o selo "Desativado"                             | Alguém desativou o link. Abra o detalhe e clique em "Ativar link".                                                                              |
| "Cliques" é maior que "Conversas"                                                      | É esperado. Cada número conta eventos, não pessoas, e um clique só vira conversa quando a pessoa escreve no WhatsApp.                           |

> **Quem vê e quem altera**
>
> Os links rastreáveis ficam dentro de Rastreamento. Quem tem o nível Ver nessa área consulta a lista e o detalhe de cada link, só para leitura. Criar, editar e desativar links exige o nível Administrar em Rastreamento (definido na aba "Acesso" do membro; o Administrador da empresa tem tudo). Quem não tem acesso à área não vê o item no menu.

**Como o link funciona por baixo**

O link não é um `wa.me` cru (o endereço padrão de link do WhatsApp). É um endereço que passa primeiro pelo servidor da Convergefy e só então leva ao WhatsApp. Esse desvio é o que permite contar o clique e casar a origem com o contato.

**Conceitos rápidos**

- **Link rastreável** — O link que você cria aqui. Leva ao WhatsApp e, de quebra, registra a origem do lead. Substitui o `wa.me` cru quando você quer saber de onde as pessoas vieram.
- **Pixel** — Um trechinho de código que você cola uma vez no `<head>` (o início do código) do seu site. Ele captura as UTMs (parâmetros no fim do endereço que dizem de qual campanha veio o clique) e os identificadores de anúncio da página e injeta nos links rastreáveis. É o que permite atribuir a origem. Sem o pixel, o link ainda funciona, mas sem identificar de qual anúncio veio.
- **Botão flutuante** — Uma bolha de WhatsApp pronta, que fica fixa no canto da página. Você cola o script e ela funciona sozinha, sem precisar do pixel.
- **Cliques × Conversas** — Cliques: quantas vezes o link foi acionado. Conversas: quantas dessas viraram mensagem de entrada de fato atribuída ao link. Um clique só vira "conversa" quando a pessoa realmente escreve no WhatsApp.

## Onde fica e a lista de links

Na barra lateral → Rastreamento, seção Configurações → Link rastreável. A tela "Link rastreável" (_"Links que levam ao WhatsApp e atribuem a origem de cada lead — no site ou em anúncios."_) lista seus links e, para quem tem o nível Administrar, traz o botão **"Novo link"**.

A tabela tem estas colunas:

| Coluna    | O que mostra                                                                 |
| --------- | ---------------------------------------------------------------------------- |
| Nome      | O apelido do link. Links desligados ganham o selo "Desativado".              |
| Link      | O identificador do link + o botão "Copiar link" (copia o endereço completo). |
| Cliques   | Quantas vezes o link foi acionado.                                           |
| Conversas | Quantas conversas o link gerou (mensagens de entrada atribuídas a ele).      |
| Criado em | A data de criação.                                                           |

> **“Cliques” e “Conversas” são números diferentes, e contam eventos, não pessoas**
>
> "Cliques" conta cada acionamento do link; "Conversas" conta só os cliques que viraram mensagem recebida atribuída ao link. A mesma pessoa clicando três vezes soma três cliques. Um clique só entra em "Conversas" quando ela de fato escreve no WhatsApp. Ambos são totais desde a criação do link (o cabeçalho de cada coluna mostra esse aviso ao passar o mouse).

Clique numa linha para abrir o detalhe do link. A busca "Buscar por nome..." filtra pelo apelido e só aparece quando já existe pelo menos um link. Sem links ainda: _'Nenhum link rastreável ainda. Crie o primeiro em "Novo link".'_ (sem o nível Administrar, só _"Nenhum link rastreável ainda."_); busca sem resultado: _"Nenhum link encontrado para esta busca."_

## Instalar o pixel (uma vez)

Para o link atribuir a origem (de qual página ou anúncio veio o lead), o pixel precisa estar no seu site. Se você não mexe no site, mande este passo para quem cuida dele.

1. **Copiar o trecho** — Na própria tela de Link rastreável há o card "Instalação do pixel": _"Instale uma vez no `<head>` do site — captura o clique e as UTMs para injetar em todos os links."_ Copie o trecho.
2. **Colar no site** — Cole no `<head>` de todas as páginas. O botão **"Como instalar"** do card expande as instruções:

   - "No código do site:" dentro de `<head>` (ou no início do `<body>`);
   - "Via Google Tag Manager:" (ferramenta do Google para colocar códigos no site sem mexer no código): nova tag → HTML personalizado → cole o script → acionamento _All Pages_ → publique.

O pixel só captura dados de rastreamento (clique e UTMs); não coleta o conteúdo da página.

> **O que muda ter ou não o pixel**
>
> Com pixel: o link registra a origem (site e anúncio) e injeta as UTMs automaticamente. Sem pixel: o link ainda funciona (abre o WhatsApp e conta os cliques), mas não identifica de qual anúncio a pessoa veio. O botão flutuante é a exceção: ele funciona sozinho, mesmo sem o pixel.

## Criar um link

Clique em **"Novo link"**. Abre o painel "Novo link rastreável" (_"Um link que leva direto pro seu WhatsApp e registra de onde o contato veio."_). Preencha:

- **Nome** — Um apelido para você achar o link na lista (placeholder _"Ex.: Home, LP Orçamento"_). Use o lugar onde ele vai ficar (ex.: _"Home"_, _"Bio do Instagram"_). Vazio: _"Informe um nome para o link."_
- **Conexão de WhatsApp** — _"O número de WhatsApp que abre quando o contato clica no link."_ A lista traz as conexões da empresa, conectadas ou não. Só fica indisponível (_"Nenhuma conexão disponível"_) quando a empresa não tem nenhuma conexão cadastrada: _"Conecte um WhatsApp em Conexões para criar um link."_ (ver [Conexões de WhatsApp](https://docs.convergefy.com.br/kb/conexoes.md)). Sem escolher: _"Selecione a conexão de WhatsApp destino."_
- **Mensagem inicial** — A mensagem que já aparece digitada no WhatsApp do contato quando ele abre a conversa (ele só toca em enviar). Já vem preenchida com _"Tenho interesse, gostaria de mais informações!"_. Vazia: _"Escreva a mensagem inicial."_

Clique em **"Criar link"** (ou "Cancelar"). Ao criar: "Link rastreável criado." e o detalhe do novo link abre sozinho. Se a conexão escolhida não tiver telefone: _"A conexão escolhida não tem telefone para o link do WhatsApp."_; outra falha: _"Não foi possível criar o link."_

## O detalhe do link

Clicar num link abre um painel lateral com os números e as formas de usar. No topo, dois indicadores, "Cliques no link" e "Conversas geradas", com o total desde a criação (sem atividade ainda: _"Ainda sem cliques. Assim que o link começar a circular, os números aparecem aqui."_).

Três coisas são editáveis no próprio lugar (salvam sozinhas): o nome (no título), a "Conexão de WhatsApp" (troca o número de destino) e a "Mensagem inicial". Isso vale só para quem tem o nível Administrar; os demais veem os três como texto. Ao salvar: "Link atualizado."

Abaixo, três blocos mostram como usar o link. Use o que combina com o seu caso: colar no seu site, usar o botão flutuante ou, se você anuncia, usar os parâmetros para anúncios.

### No seu site

Bloco "No seu site" (_"Cole o link no botão de WhatsApp da sua página"_). Traz o campo "Seu link" (copiável).

> **Cole no atributo href, não como texto**
>
> _"Cole no atributo href do seu botão — nunca só como texto. Depende do pixel instalado no site."_ Ou seja: o link vai no destino do botão (`href`, o campo de endereço que o botão abre ao ser clicado), e o pixel, já instalado no `<head>`, cuida de injetar as UTMs e atribuir a origem quando alguém clica.

### Botão flutuante

Bloco "Botão flutuante" (_"Botão de WhatsApp pronto: cole e funciona"_). Traz o campo "Script do botão" (copiável) e, ao lado, o botão de ajuda "Como instalar", que abre um aviso com "Onde:" (logo antes de fechar `</body>` do site, ou tag HTML no Gerenciador de Tags, _All Pages_) e "Como fica:" (bolha fixa no canto inferior direito, igual em desktop, tablet e celular).

1. **Copiar o script** — Copie o conteúdo de "Script do botão".
2. **Colar no site** — _"Cole o script no `<body>`. Ele cria a bolha fixa no canto inferior direito e abre a conversa em nova guia."_ Idealmente logo antes de fechar o `</body>` (ou como tag HTML no Gerenciador de Tags, disparando em _todas as páginas_).

> **O botão flutuante funciona sozinho, sem pixel**
>
> _"Já vem pronta, nada pra configurar."_ A bolha é desenhada isolada do CSS do seu site (não quebra com o tema da página) e funciona mesmo sem o pixel, só que, nesse caso, sem as UTMs de anúncio. É a alternativa mais simples ao "No seu site" quando você não quer mexer no HTML dos seus botões.

### Parâmetros para seus anúncios

Bloco "Parâmetros para seus anúncios" (aberto por padrão; se você recolher, o navegador lembra a escolha e ela vale para todos os links). Este bloco é para quem anuncia e quer que o clique no anúncio traga a origem certa.

_"Quando anunciar, cole estes parâmetros no campo de rastreamento da sua campanha. O anúncio continua apontando para a sua página; a plataforma preenche os valores no clique e o pixel liga cada clique ao contato certo."_

Há um modelo pronto para cada plataforma (copiável), além dos links "Como configurar na Meta" e "Como configurar no Google". Copie como está: os trechos entre chaves são preenchidos pela plataforma no clique.

```text
Meta Ads
utm_source={{site_source_name}}&utm_medium={{placement}}&utm_campaign={{campaign.name}}&utm_content={{ad.id}}
```

```text
Google Ads
utm_source=google&utm_medium=cpc&utm_campaign={campaignid}&utm_content={creative}&utm_term={keyword}
```

> **O anúncio aponta para a sua página, não para o link**
>
> Nos anúncios, o destino continua sendo a sua página (com o pixel instalado). Os parâmetros vão no campo de rastreamento da campanha. A plataforma preenche os valores no clique, e o pixel injeta tudo no link rastreável que estiver na página. Não troque o destino do anúncio pelo link.

## Ativar e desativar um link

> **Desativar para o link**
>
> Um link desativado deixa de redirecionar e de registrar cliques: quem clicar nele não chega ao WhatsApp. Você pode reativá-lo depois.

No rodapé do detalhe:

- Link ativo: botão **"Desativar link"**. Pede confirmação, "Desativar este link?" (_"O link {nome} deixará de redirecionar e de registrar cliques. Você pode reativá-lo depois."_). Desativado, o link para de abrir o WhatsApp e ganha o selo "Desativado" na lista.
- Link desativado: botão **"Ativar link"**, que o religa na hora.

Ao desativar aparece "Link desativado."; ao ativar, "Link atualizado." Esses botões só aparecem para quem tem o nível Administrar. Outra falha: _"Não foi possível atualizar o link."_

## Pré-requisitos

- **Nível de acesso** — Ver em Rastreamento para consultar os links; Administrar para criar, editar e desativar. (Ver [Equipe e permissões](https://docs.convergefy.com.br/kb/equipe-permissoes.md).)
- **Uma conexão de WhatsApp** — É o número que abre no clique. Sem nenhuma conexão cadastrada, não dá para criar o link. (Ver [Conexões de WhatsApp](https://docs.convergefy.com.br/kb/conexoes.md).)
- **Pixel no site** — Necessário para atribuir a origem quando o link é usado no `href` da página. O botão flutuante e o redirecionamento funcionam sem ele, mas sem as UTMs de anúncio.

## Limitações conhecidas

> Sem o pixel instalado, o link redireciona e conta cliques, mas não registra de qual anúncio o contato veio (não há UTMs a injetar). Em caso de dúvida sobre um número (cliques × conversas), lembre que são eventos, não pessoas únicas.
