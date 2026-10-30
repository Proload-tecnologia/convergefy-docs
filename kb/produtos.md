# Produtos

Produtos é a lista do que a sua empresa vende. Você cadastra uma vez e escolhe na hora de criar o negócio, sem digitar nome e valor de novo a cada oportunidade.

Na Central de Ajuda: https://docs.convergefy.com.br/#/produtos

## Em resumo

**Produtos** é o cadastro do que a sua empresa vende. Você chega por **Configurações → Produtos** (no grupo "Estrutura operacional" do menu): _"Cadastre o que a empresa vende para preencher o negócio sem digitar tudo de novo."_

Todos os membros veem a lista e escolhem produtos nos negócios. Cadastrar, editar e excluir exige o nível Administrar na área Cadastros (a mesma dos departamentos, tags e mensagens rápidas, ver [Equipe e permissões](https://docs.convergefy.com.br/kb/equipe-permissoes.md)). Sem esse nível, o botão "Novo produto" e a lixeira não aparecem e o painel do produto abre só para leitura.

Cadastrar não é obrigatório: o negócio continua aceitando nome e valor escritos à mão. O cadastro serve para **não repetir digitação** e para todo mundo escrever o mesmo nome.

### Algo deu errado?

Procure o que você está vendo e siga a coluna da direita. O detalhe de cada caso está mais abaixo.

| O que você vê                                              | O que fazer                                                                          |
| ---------------------------------------------------------- | ------------------------------------------------------------------------------------ |
| Não aparecem "Novo produto" nem a lixeira                  | Falta o nível Administrar em Cadastros. Peça a um Administrador.                     |
| "Nome é obrigatório"                                       | Preencha o nome antes de criar o produto.                                            |
| "Valor não pode ser negativo"                              | Informe zero ou um valor positivo.                                                   |
| "Não foi possível criar o produto."                        | Tente de novo; se persistir, recarregue a página.                                    |
| "Nenhum produto encontrado."                               | Ajuste a busca por nome ou SKU.                                                      |
| O produto e o valor do negócio não podem mais ser editados | O negócio foi marcado como Ganho ou Perda. Veja "Ganho ou Perda bloqueia o produto". |

**Conceitos rápidos**

- **Produto** — Um item do seu catálogo: nome, SKU e valor. Vive em Configurações, não dentro do negócio.
- **SKU** — O código interno do produto, se a sua empresa usa um (ex.: `PLANO-01`). Opcional, e pode repetir.
- **Negócio** — O cartão do funil: uma oportunidade de venda com um contato (ver [Funis e CRM](https://docs.convergefy.com.br/kb/funis.md)).
- **Produto cadastrado** — O campo do negócio que puxa um produto da lista e copia o nome e o valor dele.
- **Produto de gateway** — Produto que veio de um gateway de pagamento (hoje, a Payt), por venda ou por importação de planilha. Aparece com o ícone do gateway ao lado do nome. Ver [Gateways de pagamento](https://docs.convergefy.com.br/kb/gateways-pagamento.md).

## Cadastrar um produto

Tela "Produtos", com a busca "Buscar por nome ou SKU...". A contagem de resultados vem logo depois do subtítulo. Sem nada cadastrado: _"Nenhum produto cadastrado. Cadastre o primeiro para escolhê-lo na criação de negócios."_

1. **Abrir** — Clique em **"Novo produto"**. Abre o painel lateral "Novo produto": _"Cadastre o produto para reaproveitá-lo na criação de negócios."_
2. **Preencher** — * **Nome (obrigatório)** — _"Ex: Plano Mensal"_. Até 255 caracteres.
   * **SKU** — _"Ex: PLANO-01"_. Opcional, e não precisa ser único.
   * **Valor (R$)** — O preço, em reais (_0,00_). Deixando em branco, o valor fica R$ 0 (o produto fica sem preço) e a coluna "Valor" mostra "R$ 0".
3. **Criar** — Clique em **"Criar produto"** (mostra _"Criando..."_). Aparece "Produto criado." e ele passa a valer na lista e no seletor do negócio. Editar mostra "Produto atualizado." e excluir, "Produto excluído."

Na tabela, cada produto mostra Nome, SKU, Valor e ID. Nome, SKU e ID são copiáveis com um clique.

- Ao lado do nome fica um ícone: o logo do gateway (por exemplo, a Payt) quando o produto veio de um gateway, ou um ícone genérico de pacote nos demais.
- Clicando na linha, o produto abre para editar.
- A coluna "Ações" traz a lixeira (só com o nível Administrar), que leva à mesma confirmação de exclusão.

### Produto que vem de um gateway

Quando o produto veio de um gateway de pagamento, o painel dele mostra a linha _"Vendido pelo gateway Payt · {ID no gateway}"_, só para leitura. É esse ID que faz as vendas do gateway encontrarem o produto. Os produtos aparecem sozinhos na primeira venda, ou antes disso se você importar a lista por planilha, ver [Gateways de pagamento](https://docs.convergefy.com.br/kb/gateways-pagamento.md).

## Usar o produto num negócio

Ao criar ou editar um negócio, o campo "Produto cadastrado" busca por nome ou SKU (produtos de gateway aparecem agrupados sob o nome do gateway). Escolhendo um, ele copia o nome e o valor para os campos "Nome do produto" e "Valor (R$)", que continuam editáveis. Se você mexer num dos dois, a seleção se desfaz: o negócio passa a valer com o que você escreveu, e o produto continua na lista.

O mesmo campo existe no passo "Criar negócio" das [automações](https://docs.convergefy.com.br/kb/automacoes.md).

> **O negócio guarda uma cópia, não um vínculo**
>
> _"Alterar o produto não muda negócios já criados — eles guardam uma cópia do nome e do valor."_ O mesmo vale ao excluir: o produto sai da lista de seleção, e os negócios feitos com ele continuam intactos.

## Excluir um produto

Excluir não pode ser desfeito. No painel do produto, clique em **"Excluir produto"** (ou na lixeira da lista). A confirmação "Excluir produto?" diz: _"O produto {nome} sai da lista de seleção. Negócios já criados com ele não mudam, porque guardam uma cópia do nome e do valor. Esta ação não pode ser desfeita."_

## Como o valor aparece

Valor redondo sai sem centavos (`R$ 1.234`); valor quebrado mostra os dois dígitos (`R$ 0,10`). Nunca uma casa só.

### Editar rápido pelo cartão do negócio

> **Sem abrir o formulário**
>
> No cartão do negócio, tanto no Funil quanto no painel do contato no Chat, o produto e o valor são editáveis na hora, sem abrir o formulário. Vale para quem tem o nível Operar em Funis e com o negócio em aberto.
>
> - **Produto:** clique nele. A busca _"Buscar produto por nome ou SKU..."_ abre já com o nome atual. Escolha um produto da lista (traz nome e valor; um produto sem preço vale R$ 0 e, ao ser escolhido, também zera o valor do negócio) ou use "Usar “texto”" para gravar o que você digitou. Sair sem escolher descarta.
> - **Valor:** clique e digite; Enter, o ✓ ou clicar fora salvam, Esc ou o ✕ desistem.
> - **Sem produto:** o cartão mostra o convite tracejado "Vincular produto". Quem não pode editar, ou em negócio finalizado, vê _"Sem produto"_.
> - **Sem valor:** o cartão mostra R$ 0, em tom apagado.

## Ganho ou Perda bloqueia o produto

Enquanto o negócio está em aberto, você edita produto e valor à vontade. Depois de marcado como Ganho ou Perda, os dois ficam somente leitura, inclusive no cartão. Acerte nome e valor antes de fechar: o que muda e o que continua possível depois de fechar está em [Ganhar ou perder um negócio](https://docs.convergefy.com.br/kb/funis.md).

## Erros e avisos esperados

- “Nome é obrigatório” — o cadastro exige ao menos o nome. Resolver: preencha o nome antes de criar o produto.
- “Valor não pode ser negativo” — o campo de valor não aceita número negativo. Resolver: informe zero ou um valor positivo.
- “Não foi possível criar o produto.” — falha ao criar o produto. Resolver: tente de novo; se persistir, recarregue a página.
- “Não foi possível atualizar o produto.” — falha ao editar o produto. Resolver: tente salvar de novo; se persistir, recarregue a página.
- “Não foi possível excluir o produto.” — falha ao excluir o produto. Resolver: tente de novo; se persistir, recarregue a página.
- “Nenhum produto encontrado.” — a busca não casou com nenhum produto cadastrado. Resolver: ajuste a busca por nome ou SKU.
