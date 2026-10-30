# Gateways de pagamento

Conecte o gateway de pagamento da sua empresa (hoje, a Payt) para a Convergefy receber as vendas de boleto, cartão e pix e usá-las nas automações. Aqui você conecta, confere se os eventos estão chegando, importa produtos e desconecta.

Na Central de Ajuda: https://docs.convergefy.com.br/#/gateways-pagamento

## Em resumo

Um **gateway de pagamento** é o serviço que cobra o seu cliente (hoje, a Payt). Quando alguém gera um boleto, paga um pix, tem o cartão recusado ou abandona o checkout, o gateway avisa a Convergefy por um endereço chamado webhook. Com esse aviso, uma [automação](https://docs.convergefy.com.br/kb/automacoes.md) pode reagir: por exemplo, mandar uma mensagem para quem gerou o boleto.

Você chega por Configurações → Integrações → Gateways de pagamento. Título da tela: "Gateways de pagamento", _"Receba as vendas de boleto, cartão e pix para usar nas automações."_

É uma área de **administrador**: o item só aparece no menu de Configurações para o Administrador da empresa. Nenhum nível de acesso da aba "Acesso" do membro dá esta permissão.

### Algo deu errado?

Procure o que você está vendo e siga a coluna da direita. O detalhe de cada caso está mais abaixo.

| O que você vê                                                                                                                | O que fazer                                                                                                                                                             |
| ---------------------------------------------------------------------------------------------------------------------------- | ----------------------------------------------------------------------------------------------------------------------------------------------------------------------- |
| Status "Falta a chave" (âmbar)                                                                                               | Nenhuma venda é processada. Cadastre a URL na Payt e salve a Chave Única no campo "Cole a chave aqui".                                                                  |
| Status "Aguardando primeiro evento"                                                                                          | Cadastre a URL na Payt e use "Testar URL" lá. O primeiro aviso que chegar confirma a conexão.                                                                           |
| Status "Chave diferente"                                                                                                     | Os avisos chegam com outra chave e não são processados. Copie a Chave Única atual na Payt e use "Trocar chave". O status só some quando a Payt mandar o próximo evento. |
| "Informe a chave." ou "A chave tem no máximo 255 caracteres."                                                                | Cole só a Chave Única da Payt, sem texto a mais.                                                                                                                        |
| "Não foi possível conectar o gateway." ou "Não foi possível salvar a chave."                                                 | Tente de novo. Se persistir, recarregue a página.                                                                                                                       |
| Gatilho "Gateway de pagamento" avisa _"Conecte um gateway em Configurações > Gateways de pagamento para usar este gatilho."_ | Conecte a Payt neste guia.                                                                                                                                              |
| Lista de produtos do gatilho vazia: _"Importe os produtos na tela do gateway."_                                              | Use "Importar produtos" (veja abaixo).                                                                                                                                  |
| Importação "Falhou"                                                                                                          | Use "Reprocessar" na linha, ou baixe o relatório de erros para corrigir a planilha.                                                                                     |
| "Não foi possível ler a planilha. Confira se o arquivo não está corrompido."                                                 | Abra a planilha no seu programa, salve de novo como csv, xlsx ou ods e reenvie.                                                                                         |
| Quer desconectar a Payt                                                                                                      | Atenção: apaga o histórico de vendas e cancela automações em andamento. Veja "Desconectar".                                                                             |

**Conceitos rápidos**

- **Gateway** — O serviço de pagamento que processa as vendas da sua empresa. A Convergefy só recebe os avisos dele; quem cobra o cliente continua sendo o gateway.
- **Webhook (URL do webhook)** — Um endereço exclusivo da sua empresa, gerado pela Convergefy, que o gateway chama toda vez que uma venda muda de situação. Você cadastra esse endereço no painel do gateway.
- **Postback** — O nome que a Payt dá a esse cadastro: é onde você coloca a URL do webhook para a Payt avisar a Convergefy.
- **Chave Única** — Um código que a Payt envia em todo aviso. A Convergefy compara com a chave que você salvou aqui: só processa o aviso se as duas forem iguais. É isso que impede que alguém de fora finja ser a Payt.
- **Evento** — Cada aviso do gateway: boleto gerado, pix pago, cartão recusado, carrinho abandonado… Os eventos viram o gatilho "Gateway de pagamento" das automações.
- **Order bump** — Uma oferta extra no mesmo checkout.

## Conectar a Payt

Na tela, a seção "Disponíveis" mostra o card da Payt: _"Boleto, cartão e pix"_, com o selo "Não conectado" e o botão "Conectar".

> **Sem a chave, nenhuma venda é processada**
>
> Conectar não basta. Enquanto a Chave Única não estiver salva, os avisos da Payt chegam, mas nenhuma venda é processada e nenhuma automação de pagamento inicia. O campo da chave fica aberto até você salvar.

1. **Conectar** — Clique em **"Conectar"** (ou no card). Isso só cria a integração e gera a URL do webhook. Ainda não liga nada: o painel da Payt abre com o status "Falta a chave". O card passa para a seção "Conectados".
2. **Copiar a URL e cadastrá-la na Payt** — No painel, a seção "URL do webhook" mostra o endereço, com um botão para copiar ("Copiar URL do webhook"). Siga o "Como configurar na Payt":

   1. Na Payt, abra Ofertas & Produtos > Postbacks.
   2. Crie um novo postback e cole a URL acima no campo de URL.
   3. Escolha os produtos e os eventos que quer receber.
   4. Salve e use "Testar URL" para conferir.

   Marque na Payt os eventos que suas automações usam. Para o gatilho de carrinho abandonado, por exemplo, o evento de abandono de checkout precisa estar marcado no postback (ver [Automações](https://docs.convergefy.com.br/kb/automacoes.md)).

   O "Testar URL" serve só para confirmar a conexão: a Convergefy grava a venda de teste, mas não inicia nenhuma automação com ela. Assim o comprador fictício do teste não recebe mensagem de verdade no WhatsApp.
3. **Salvar a Chave Única** — Na seção "Chave Única da Payt" aparece o campo **"Cole a chave aqui"**, com a dica _"Na Payt, abra Ofertas & Produtos > Postbacks e copie a Chave Única."_ Cole a chave e clique em **"Salvar chave"**. Aparece _"Chave salva."_
4. **Esperar o primeiro evento** — Com a chave salva, o status vai para "Aguardando primeiro evento". Assim que a Payt avisar qualquer evento, ele vira "Conectado" e o painel mostra quando foi o último aviso.

## Como saber se está funcionando

O status aparece no card (selo) e no topo do painel, com uma explicação logo abaixo. No card e no painel também fica o texto do último aviso (_"Último evento hoje, 10:32"_, _"Último evento ontem, 19:30"_, _"Último evento 27/09, 14:02"_) ou _"Nenhum evento recebido ainda"_.

**Os quatro status**

- **Falta a chave** (amber) — _"Cadastre a URL no gateway e salve a chave dele aqui. Sem a chave, nenhuma venda é processada."_ Como resolver: cadastre a URL na Payt e salve a Chave Única no campo “Cole a chave aqui”.
- **Aguardando primeiro evento** (gray) — _"Cadastre a URL no gateway. O primeiro evento que chegar confirma a conexão."_ Como resolver: cadastre a URL na Payt e use “Testar URL” lá; o primeiro aviso que chegar confirma a conexão.
- **Conectado** (green) — _"Os eventos estão chegando."_
- **Chave diferente** (amber) — _"Os eventos estão chegando com outra chave e não são processados. Confira a Chave Única abaixo."_ Como resolver: copie a Chave Única atual na Payt e use “Trocar chave” para salvá-la aqui. O status só some quando a Payt mandar o próximo evento.

### Trocar a chave

Com a chave salva, a seção "Chave Única da Payt" mostra a chave mascarada e o botão "Trocar chave". Ele abre o campo "Nova chave" com "Salvar chave" e "Cancelar". Use quando a Payt gerar uma chave nova ou quando o status estiver em "Chave diferente". A chave aceita até 255 caracteres.

Depois de salvar a chave certa, o status "Chave diferente" só muda quando a Payt mandar o próximo evento. Isso não significa que a correção falhou.

## Importar produtos da Payt

Na seção "Produtos" do painel: _"Os produtos são criados na primeira venda. Para montar as automações antes, importe a lista por planilha."_ Sem importar, o produto só aparece na lista de [Produtos](https://docs.convergefy.com.br/kb/produtos.md) depois da primeira venda dele. Importar serve para escolher o produto no gatilho da automação antes de vender.

Clique em "Importar produtos". O painel troca para "Importar produtos": _"Produtos da Payt, para montar as automações antes da primeira venda."_ Ele mostra o histórico das importações (vazio: _"Nenhuma importação ainda. Envie uma planilha para começar."_). A seta no topo volta um nível.

1. **Nova importação** — Clique em **"Nova importação"**. Envie a planilha: _"Uma linha por produto, com o ID dele no gateway. Nome, valor e SKU são opcionais."_ Formatos csv, txt, xlsx, ods, até 10.000 linhas e 20 MB. Enquanto lê, mostra _"Lendo a planilha…"_.
2. **Mapear as colunas** — Em "Mapeamento de colunas" (_"O ID no gateway é obrigatório."_), diga o que cada coluna é. A Convergefy já sugere pelo nome da coluna. Ajuste o que precisar e deixe "Ignorar" nas que não quer. Os destinos são:

   - **ID no gateway** — Obrigatório, em uma (e só uma) coluna. _"O código do produto no gateway. É por ele que as vendas encontram o produto."_
   - **Nome** — O nome do produto.
   - **Valor** — _"Em reais, como 97,00. Célula vazia não altera o valor."_
   - **SKU** — O código interno do produto, se houver.

   Cada campo só aceita uma coluna. Clique em **"Continuar"**.
3. **Confirmar** — O resumo mostra o "Arquivo" e as "Colunas mapeadas", com o aviso _"Produto que já existe é atualizado com o que vier preenchido. Célula vazia não apaga nada."_ Clique em **"Importar produtos"**. Aparece _"Importação iniciada. Ela roda em segundo plano."_

A importação roda em segundo plano. No histórico, cada linha mostra o estado e o resultado (_"{n} importados · {n} com erro · {n} repetidos"_):

**Estado de cada importação**

- **Na fila** (gray) — aguardando começar.
- **Processando** (blue) — importando as linhas, com o progresso em %.
- **Concluída** (green) — terminou.
- **Falhou** (red) — a importação não completou. Como resolver: use “Reprocessar” na linha, ou baixe o relatório de erros para corrigir a planilha.
- **Cancelada** (gray) — você interrompeu; os produtos já importados ficam.

**Ações em cada linha do histórico**

- "Cancelar": para importação na fila ou processando (_"Cancelar importação?"_ / _"Os produtos já importados são mantidos."_).
- "Reprocessar": para importação que falhou.
- No menu "Mais ações":
  - "Baixar relatório de erros" (só quando houve falhas);
  - "Excluir" (_"Excluir do histórico?"_ / _"Isto remove apenas o registro. Os produtos importados não são apagados."_), desativado enquanto a importação está em andamento.

O produto que veio da Payt ganha o ícone da Payt ao lado do nome na lista de [Produtos](https://docs.convergefy.com.br/kb/produtos.md) e, ao abrir o produto, a linha _"Vendido pelo gateway Payt · {ID no gateway}"_. Esse vínculo é o que faz cada venda encontrar o produto certo.

**Regras de produto entre vendas e gateways**

- Só o produto principal da venda cria ou encontra o produto na lista. Um order bump (oferta extra no mesmo checkout) não cria produto.
- Cada gateway tem os seus produtos, então o mesmo produto vendido em dois gateways aparece como dois.
- Produto cadastrado à mão em [Produtos](https://docs.convergefy.com.br/kb/produtos.md) nunca recebe venda de gateway.
- O código do produto no gateway não pode ser editado.

## Usar nas automações

Com a Payt conectada, o gatilho "Gateway de pagamento" das [automações](https://docs.convergefy.com.br/kb/automacoes.md) passa a receber os eventos (boleto, pix, cartão, carrinho abandonado). Sem nenhum gateway conectado, o formulário do gatilho avisa: _"Conecte um gateway em Configurações > Gateways de pagamento para usar este gatilho."_ A lista de produtos do gatilho vem daqui: se estiver vazia, _"Importe os produtos na tela do gateway."_ Os detalhes de cada evento estão em [Automações](https://docs.convergefy.com.br/kb/automacoes.md).

### O contato e o status da venda

**Como a Convergefy trata o contato e o status**

- Contato: a Convergefy procura o contato só pelo telefone do comprador. Com ou sem o +55, o número cai no mesmo contato. Se o contato já existe, só os campos vazios são preenchidos (nome, e-mail, documento): nada do que você já tinha é sobrescrito.
- Venda sem telefone utilizável é gravada sem contato e não inicia nenhuma automação. Se um aviso seguinte da mesma venda chegar com telefone, a venda passa a ser ligada ao contato.
- Avisos intermediários da Payt, como estorno parcial ou pendente, contestação aberta e reprocessamento, não mudam a venda: a Convergefy espera o aviso final.
- Boleto "expirado" na Payt não vira o evento Vencido. O Vencido é calculado pela Convergefy, no dia seguinte ao vencimento, se o boleto continuar sem pagamento.

## Desconectar

> **Desconectar apaga o histórico e encerra automações em andamento**
>
> A URL do webhook para de funcionar e o histórico de vendas recebidas é apagado. Não dá para desfazer. As automações em andamento que nasceram das vendas dessa integração, ou de carrinho abandonado dela, são canceladas, para não continuarem mandando mensagem de um gateway que não existe mais.
>
> Os produtos já criados continuam na lista de Produtos. Para voltar, conecte de novo: a URL e a chave são novas, então é preciso recadastrar a URL na Payt e salvar a chave.

No rodapé do painel, **"Desconectar"** abre a confirmação _"Desconectar a Payt?"_: _"A URL do webhook para de funcionar e o histórico de vendas recebidas é apagado. Não dá para desfazer."_ Confirme em "Desconectar" ou desista em "Voltar". Aparece _"Payt desconectada."_

## Erros e avisos esperados

- “Não foi possível conectar o gateway.” — falha ao criar a integração. Resolver: tente clicar em “Conectar” de novo; se persistir, recarregue a página.
- “Informe a chave.” — o campo da chave está vazio. Resolver: cole a Chave Única da Payt no campo antes de salvar.
- “A chave tem no máximo 255 caracteres.” — a chave colada é longa demais. Resolver: confira se copiou só a Chave Única, sem texto a mais.
- “Não foi possível salvar a chave.” — falha ao salvar a chave. Resolver: tente salvar de novo; se persistir, recarregue a página.
- “Não foi possível desconectar o gateway.” — falha ao desconectar. Resolver: tente de novo; se persistir, recarregue a página.
- “Não foi possível carregar os gateways” — a lista de gateways não carregou. Resolver: use o botão “Tentar de novo” da tela.
- “Não foi possível ler a planilha. Confira se o arquivo não está corrompido.” — a planilha de produtos não pôde ser lida. Resolver: abra a planilha no seu programa, salve de novo como csv, xlsx ou ods e reenvie.
- “Máximo de 10000 linhas por importação. Divida o arquivo.” — a planilha passa do limite de linhas. Resolver: separe a planilha em arquivos menores.
- “Mapeie exatamente uma coluna para o ID no gateway.” — nenhuma coluna, ou mais de uma, foi mapeada para o ID. Resolver: aponte uma (e só uma) coluna para “ID no gateway”.
- “Cada campo só pode ser mapeado por uma coluna.” — duas colunas foram apontadas para o mesmo campo. Resolver: deixe uma coluna por destino e marque as outras como “Ignorar”.
- “Não foi possível iniciar a importação.” — falha ao disparar a importação de produtos. Resolver: confirme de novo; se persistir, reabra a importação.
- “Só dá para cancelar uma importação pendente ou em andamento.” — a importação já terminou. Resolver: veja o estado atual no histórico.
- “Só dá para reprocessar uma importação que falhou.” — a importação não falhou. Resolver: use “Reprocessar” só em linhas com o estado “Falhou”.
- “Cancele a importação antes de excluir.” — a importação ainda está na fila ou processando. Resolver: clique em “Cancelar” na linha e só depois exclua o registro.
