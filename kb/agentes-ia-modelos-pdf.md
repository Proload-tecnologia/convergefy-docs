# Agentes de IA: Modelos de PDF

Um modelo de PDF é um documento seu (proposta, protocolo, orçamento) em que você marca o que muda de pessoa para pessoa. O agente de IA envia o PDF já preenchido com os dados do contato da conversa.

Na Central de Ajuda: https://docs.convergefy.com.br/#/agentes-ia-modelos-pdf

## Em resumo

Um **modelo de PDF** é um arquivo que você envia uma vez, marcando os trechos que mudam (o nome do contato, o telefone, um campo personalizado). Na conversa, o agente gera uma cópia com os dados do contato e envia. Você revisa e **aprova** o modelo antes: enquanto for rascunho, o agente não envia.

Use quando o mesmo documento vai para muita gente com poucos dados diferentes. Para um arquivo que vai igual para todos, use um arquivo comum em "Arquivos para enviar" (ver [Agentes de IA](https://docs.convergefy.com.br/kb/agentes-ia.md)).

### Algo deu errado?

Procure o que você está vendo e siga a coluna da direita. O detalhe de cada caso está mais abaixo.

| O que você vê                                                                      | O que fazer                                                                            |
| ---------------------------------------------------------------------------------- | -------------------------------------------------------------------------------------- |
| "Só PDF pode ser modelo."                                                          | Envie um arquivo em PDF.                                                               |
| "O limite é de 15 páginas e 20 MB."                                                | Reduza o PDF ou divida em partes.                                                      |
| "Este PDF não pode ser modelo. As páginas são imagens, sem texto para trocar. …"   | Exporte de novo como PDF de texto, não escaneado, e envie outra vez.                   |
| "Este PDF não pode ser modelo. Exporte de novo pela ferramenta em que foi feito …" | Exporte o PDF de novo pelo programa em que foi criado e envie outra vez.               |
| Modelo com a etiqueta "Rascunho"                                                   | Clique em "Continuar", marque os trechos, confira e aprove. Até lá o agente não envia. |
| "Abra no desktop para marcar os trechos do documento."                             | Abra a Convergefy num computador. A marcação não funciona em tela estreita.            |
| "Selecione um trecho dentro de uma mesma linha."                                   | Selecione só o texto de uma linha.                                                     |
| "Este trecho já está marcado."                                                     | Esse texto já foi marcado. Edite ou remova a marcação existente.                       |
| "Não foi possível abrir o modelo."                                                 | Clique em "Tentar de novo".                                                            |
| "Não foi possível gerar a prévia. Tente de novo."                                  | Clique em "Tentar de novo".                                                            |
| Um trecho aparece "Em branco" na conferência                                       | O contato não tem esse dado. Nesse contato, o trecho sai em branco.                    |

## Antes de enviar o arquivo

> **Limites do modelo**
>
> O modelo precisa ser um **PDF com texto** (não uma foto ou digitalização), com **até 15 páginas e 20 MB**. Para arquivos comuns da aba Mídias o limite é maior (100 MB), mas modelo de PDF é menor. Um PDF feito de imagens não serve: não há texto para trocar.

## Criar um modelo

Na aba **"Mídias"** do agente, o bloco **"Modelos de PDF"** mostra: _"O agente envia o PDF preenchido com os dados de cada contato. Você marca o que muda e aprova antes."_ Sem nenhum modelo: _"Nenhum modelo adicionado ainda."_

1. **Enviar o modelo** — Clique em **"Enviar modelo"** e escolha o PDF. Se o arquivo for recusado, aparece um cartão vermelho com o nome dele e o motivo (ver "Erros e avisos esperados"). Se for aceito, o modelo entra como **rascunho**.
2. **Marcar os trechos** — Na linha do modelo, clique em **"Continuar"**. A tela cheia abre com _"Marque os trechos que mudam para cada contato"_. Selecione no documento o texto que muda (dentro de uma mesma linha). No balão **"O que entra aqui"**, escolha no seletor o dado do contato (ele começa em "Nome completo") e clique em **"Marcar trecho"**. Repita para cada trecho.
3. **Conferir** — Clique em **"Conferir"** (só fica ativo com pelo menos um trecho marcado). Em _"Confira com um contato e com o pior caso antes de aprovar"_, veja a aba **"Um contato"** (escolha um contato real) e a aba **"Pior caso"** (valores muito compridos, para ver como o documento se ajusta). Cada dado usado mostra o valor aplicado ou **"Em branco"**. Se algo estiver errado, clique em **"Voltar aos trechos"**.
4. **Aprovar** — Clique em **"Aprovar"**. O modelo continua em "Modelos de PDF", passa a **"Aprovado"** e pode ser enviado e citado com @.
5. **Dizer quando enviar** — Na linha do modelo, preencha **"Quando enviar"** (até 500 caracteres), por exemplo: _"enviar quando o contato pedir para ver funcionando"_. Ou cite o modelo com **@** nas **"Instruções ao LLM"**, escolhendo o tipo **Mídias**. É a mesma regra dos arquivos comuns: o campo é gravado quando você clica em "Salvar" na tela do agente.

Cada modelo mostra na linha o nome do arquivo, a etiqueta "modelo", o tamanho e a contagem de trechos (_"Nenhum trecho marcado"_, _"1 trecho"_ ou _"N trechos"_).

**Marcar os trechos: o que a tela oferece**

- **Dado** — Seletor que já abre com "Nome completo" escolhido, com busca (**"Buscar dado"**). Grupo **"Contato"**: "Nome completo", "Primeiro nome", "Telefone" e "E-mail". Grupo **"Campos personalizados"**: um item para cada campo personalizado da empresa. Sem resultado: _"Nenhum dado encontrado."_
- **Marcar os N lugares onde este trecho aparece** — Aparece quando o mesmo texto está em mais de um lugar do documento. Vem marcada por padrão. Desmarque para marcar só o trecho que você selecionou.
- **Cancelar / Marcar trecho** — "Cancelar" descarta. "Marcar trecho" confirma (ao editar, o botão vira "Salvar").
- **Trechos que mudam** — Lista na lateral. Vazia: _"Nenhum trecho marcado"_ e _"Selecione no documento o texto que muda de pessoa para pessoa."_ Cada item mostra _"No modelo: …"_, quantos lugares ele ocupa, e os ícones **"Editar trecho"** e **"Remover trecho"**.

Cada marcação grava na hora. Não existe botão de salvar nessa tela. Para sair, use a seta **"Voltar para Mídias"**.

> **Marcar só no computador**
>
> Em tela estreita (menos de 900 px de largura), a tela de marcação mostra apenas _"Abra no desktop para marcar os trechos do documento."_ Para marcar, conferir e aprovar um modelo, use um computador.

## Rascunho e aprovado

**Estado de cada modelo**

- **Rascunho** (amber) — _"Marque o que muda para cada contato, confira e aprove. Até lá o agente não envia este modelo."_ Não aparece no @ das instruções. Como resolver: clique em Continuar, marque os trechos, confira e aprove.
- **Aprovado** (green) — o agente pode enviar. Pode ser citado com @ e tem o botão **"Editar trechos"**.

> **Mudar um trecho volta o modelo para rascunho**
>
> _"Aprovado. Mudar um trecho volta o modelo para rascunho."_ Depois de qualquer mudança nos trechos de um modelo aprovado, confira e aprove de novo. Enquanto isso o agente não envia o modelo.

## Como o agente envia

O agente decide enviar pelo campo **"Quando enviar"** ou pela citação com @ nas instruções, igual aos arquivos comuns. Na hora, ele gera o PDF com os dados do contato da conversa e envia.

**Dados vazios, maiúsculas e nome do arquivo**

- **Dado vazio:** se o contato não tem aquele dado, o trecho sai em branco.
- **Maiúsculas automáticas:** se o texto original do trecho estava todo em MAIÚSCULAS, o valor também entra em maiúsculas, para combinar com o resto da linha. Texto original com alguma minúscula, ou sem letras (uma data, um número), não muda.
- **Nome do arquivo:** o PDF enviado mantém o nome do original, trocando nele os mesmos trechos marcados. Por exemplo, um modelo _"Protocolo\_FULANO.pdf"_ com "FULANO" marcado como **"Primeiro nome"** sai como _"Protocolo\_Maria.pdf"_. No nome do arquivo não há conversão para maiúsculas.
- **Testar:** no teste do agente (**"Testar"**) não há contato real: o envio aparece só com o nome do arquivo, sem gerar o PDF preenchido.
- **Falha na geração:** se o PDF não puder ser gerado, o agente não avisa o contato de que enviou.

## Remover um modelo

> **Não dá para desfazer**
>
> O ícone de lixeira **"Remover modelo"** abre a confirmação _"Remover mídia?"_, com o aviso _"Não dá para desfazer."_ Onde o modelo estava citado com @, o agente deixa de enviar.

## Erros e avisos esperados

- “Só PDF pode ser modelo.” — o arquivo escolhido não é um PDF. Resolver: envie um arquivo em PDF.
- “Arquivo vazio.” — o arquivo tem 0 bytes. Resolver: escolha um arquivo que tenha conteúdo.
- “O limite é de 15 páginas e 20 MB.” — o PDF passa de 15 páginas ou de 20 MB. Resolver: reduza o PDF ou divida em partes menores.
- “Este PDF não pode ser modelo. As páginas são imagens, sem texto para trocar. Exporte como PDF de texto e envie de novo.” — o PDF é feito de imagens (escaneado), sem texto para marcar. Resolver: exporte como PDF de texto e envie de novo.
- “Este PDF não pode ser modelo. Exporte de novo pela ferramenta em que foi feito e envie outra vez.” — o arquivo tem uma estrutura que a Convergefy não consegue ler. Resolver: exporte de novo pelo programa em que o documento foi feito e envie outra vez.
- “Não foi possível enviar o modelo de PDF.” — o envio do arquivo não foi concluído. Resolver: tente enviar de novo.
- “Não foi possível salvar os trechos do modelo.” — a marcação não foi gravada. Resolver: refaça a marcação e confira se ela aparece na lista Trechos que mudam.
- “Não foi possível abrir o modelo.” — a tela de marcação não conseguiu carregar o documento. Resolver: clique em Tentar de novo.
- “Não foi possível gerar a prévia. Tente de novo.” — a prévia não foi gerada. Resolver: clique em Tentar de novo.
- “Não foi possível aprovar o modelo.” — a aprovação não foi concluída. Resolver: tente aprovar de novo.
- “Selecione um trecho dentro de uma mesma linha.” — a seleção atravessa mais de uma linha. Resolver: selecione só o texto de uma linha.
- “Este trecho já está marcado.” — a seleção se sobrepõe a um trecho já marcado. Resolver: edite ou remova a marcação existente.
