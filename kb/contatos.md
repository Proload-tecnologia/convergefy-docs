# Contatos (Leads)

Contatos (ou leads) são os clientes da sua empresa. Cada conversa no Chat e cada negócio no Funil está ligado a um contato. Aqui você cadastra, edita, filtra e organiza essas pessoas.

Na Central de Ajuda: https://docs.convergefy.com.br/#/contatos

## Em resumo

Os **contatos** são as pessoas (ou empresas) com quem você fala. Cada conversa no Chat e cada negócio no Funil aponta para um contato. O telefone identifica o contato e permite falar com ele por WhatsApp.

### Algo deu errado?

Procure o que você está vendo e siga a coluna da direita. O detalhe de cada caso está mais abaixo.

| O que você vê                                                                                         | O que fazer                                                                                        |
| ----------------------------------------------------------------------------------------------------- | -------------------------------------------------------------------------------------------------- |
| "Já existe um contato com esse telefone: {nome}." e o "Salvar" desabilitado                           | Não é erro: o telefone já tem dono. Clique em "Ver contato" para abrir o contato que existe.       |
| Não aparecem "Importar", "Novo Contato" ou a lixeira                                                  | Falta o nível Editar em Contatos. Peça a um Administrador.                                         |
| "Máximo de 10000 linhas por importação. Divida o arquivo."                                            | Separe a planilha em arquivos menores.                                                             |
| Importação com estado "Falhou"                                                                        | Use "Reprocessar" na linha, ou baixe o relatório de erros para corrigir a planilha.                |
| Algumas linhas não entraram na importação                                                             | No menu de três pontinhos da linha, use "Baixar relatório de erros", corrija a planilha e reenvie. |
| "Telefone inválido ou ausente. Número internacional deve ser marcado com +." no relatório             | Escreva o `+` e o código do país nos números de fora do Brasil.                                    |
| "Atendente principal não encontrado: nenhum membro ativo desta empresa tem este e-mail." no relatório | Use, na planilha, o e-mail de um membro ativo da empresa, não o nome.                              |
| A exportação parou no meio                                                                            | Use "Baixar parcial" ou "Tentar de novo".                                                          |
| "Nenhum lead encontrado."                                                                             | Ajuste a busca ou limpe os filtros. "Lead" é o mesmo que contato.                                  |
| "Nenhum contato no filtro atual. Ajuste a busca ou os filtros para exportar."                         | O recorte está vazio. Ajuste a busca ou os filtros.                                                |

Acesse por **barra lateral → Contatos**. O subtítulo, _"Gerencie seus contatos e oportunidades de negócio."_, traz o total (ex.: _"(3321 resultados)"_). À esquerda ficam a busca "Buscar contatos..." e o filtro. À direita ficam estes botões, que aparecem conforme o seu nível de acesso:

- "Campos personalizados";
- "Importar" (traz contatos de uma planilha);
- "Exportar" (leva contatos para uma planilha);
- "Novo Contato".

No celular, os três primeiros viram só ícone.

| O que você quer fazer                                                                              | Nível necessário em Contatos |
| -------------------------------------------------------------------------------------------------- | ---------------------------- |
| Ver a lista, abrir o painel do contato (inclusive a aba "Rastreio") e usar "Exportar"              | **Ver**, que todo membro tem |
| "Novo Contato", "Importar", renomear, editar dados e tags, definir o atendente principal e excluir | **Editar**                   |
| "Campos personalizados" e a aba "Configurações" do contato (bloqueio de mensagens)                 | **Administrar**              |

Cada nível inclui os de baixo, e o administrador da empresa tem todos. O nível fica na aba "Acesso" do membro (ver [Equipe e permissões](https://docs.convergefy.com.br/kb/equipe-permissoes.md)). Sem Editar, o painel abre só para leitura e somem "Importar", "Novo Contato" e a lixeira.

**Conceitos rápidos**

- **Contato / Lead** — Dois nomes para a mesma coisa: a pessoa (ou empresa) cliente.
- **Tag** — Etiqueta colorida (ver [Tags e Departamentos](https://docs.convergefy.com.br/kb/tags-departamentos.md)).
- **ID Externo** — Identificador opcional para casar o contato com outro sistema seu, como o código do cliente no ERP (o sistema de gestão da empresa) ou na loja.

## Preciso cadastrar todo mundo na mão?

**Não.** Quando um cliente manda mensagem para um número seu, a Convergefy cria o contato sozinha, com o nome do perfil do WhatsApp. Se o perfil não tiver nome, o telefone vira o nome.

> **Quando cadastrar à mão**
>
> Só para falar primeiro com quem ainda não te escreveu ou pré-organizar a base (tags, dados, ID externo) antes do contato chegar. Para muita gente de uma vez, use "Importar".

## A lista de contatos

A tabela mostra 20 contatos por página.

| Coluna              | O que mostra                                                                                                                                                  |
| ------------------- | ------------------------------------------------------------------------------------------------------------------------------------------------------------- |
| Nome                | Avatar e nome. Sem nome, mostra o telefone.                                                                                                                   |
| Contato             | Telefone formatado e, abaixo, o e-mail.                                                                                                                       |
| Negócios            | Negócios do contato em todos os funis: "Total" (só a quantidade) e "Em aberto", "Ganho" e "Perda", cada um com valor em R$ e quantidade (ex.: _"1 negócio"_). |
| ID Externo          | O identificador externo, ou "—".                                                                                                                              |
| Tags                | As etiquetas coloridas, ou "—".                                                                                                                               |
| Atendente principal | Avatar e nome, ou "—". O ícone de informação explica o campo.                                                                                                 |
| Criado em           | A data de cadastro.                                                                                                                                           |
| Ações               | Lixeira para excluir (só com Editar). Para ver ou editar, clique na linha.                                                                                    |

## Criar um contato

Clique em **"Novo Contato"**. Abre um painel lateral: _"Preencha os dados do contato abaixo."_

1. **Preencher os dados** — O único campo obrigatório é o Telefone, e o botão "Salvar" só habilita com ele preenchido. Se a empresa tem campos personalizados, eles aparecem numa seção "Campos personalizados".
2. **Salvar** — Clique em **"Salvar"** (mostra _"Salvando..."_). Aparece "Contato criado com sucesso!"

- **Telefone \*** — _"Ex: +55 (11) 99999-9999"_. Obrigatório (é por ele que o WhatsApp encontra a pessoa) e precisa ser válido.
- **Nome** — _"Nome do contato"_. Opcional, até 255 caracteres.
- **E-mail** — _<email@exemplo.com>_. Opcional, com formato válido, até 255 caracteres.
- **Documento (CPF/CNPJ)** — _"Apenas números"_. Opcional. Atenção: o sistema pode gravar o número diferente do digitado, sem avisar (veja "Limites e regras").
- **Tags** — Clique nas etiquetas para marcar ou desmarcar. O campo só aparece se a empresa já tem tags.
- **Endereço** — _"Endereço completo"_. Opcional, até 500 caracteres.
- **ID Externo** — _"ID externo (opcional)"_.
- **Atendente principal** — Opcional. Vem com _"Sem atendente principal"_.

> **Telefone que já existe não duplica**
>
> Ao digitar um telefone que já pertence a um contato, aparece logo abaixo do campo _"Já existe um contato com esse telefone: {nome}."_ com o botão "Ver contato", e o "Salvar" fica desabilitado. Isso não é erro. "Ver contato" fecha o cadastro e abre o painel do contato que já existe, onde dá para editar ou excluir.

Quando o mesmo telefone chega por mensagem recebida ou por importação, o contato existente é reaproveitado (a importação atualiza os campos da planilha).

## Atendente principal

É o membro que você marca como referência de um contato: um dado do contato, não da conversa. Serve para automações e pode ser o público de uma campanha de [Disparo em massa](https://docs.convergefy.com.br/kb/disparo-em-massa.md).

> **Não é quem atende a conversa**
>
> _"Serve de referência para automações. Não altera quem está atendendo as conversas deste contato."_ Não muda o responsável de nenhuma conversa, não distribui atendimento e não esconde nada de ninguém. O texto aparece no ícone de informação ao lado do campo.

Todo membro vê o campo; editar exige Editar. Ele aparece:

- no "Novo Contato";
- na coluna e no filtro da lista;
- na importação ("Atendente principal (e-mail)");
- no painel do contato.

No painel, um botão abaixo do nome mostra o atendente ou _"Sem atendente principal"_ ("Definir atendente principal" se vazio, "Alterar atendente principal" se preenchido). Para limpar, escolha _"Sem atendente principal"_. Salva sozinho, com _"Contato atualizado com sucesso."_

## Importar contatos de uma planilha

O botão **"Importar"** abre um painel lateral com o histórico das 20 importações mais recentes ("Importar contatos"). Clique em **"Nova importação"**. São três passos.

> **Contato que já existe é atualizado**
>
> Telefone que já existe atualiza o contato, sem duplicar. Os campos mapeados sobrescrevem os atuais, célula vazia não apaga nada e as tags da importação são somadas às dele. Telefone repetido na planilha: só a primeira linha entra, as outras contam como duplicadas.

> **Não precisa de planilha modelo**
>
> Suba a sua planilha, como está, e diga no passo seguinte qual coluna é o quê. A Convergefy adivinha (coluna "Celular" vira Telefone, "E-mail" vira E-mail…) e você ajusta o que errou.

1. **Subir o arquivo** — Arraste a planilha ou clique para escolher. A área diz _"csv, xlsx, ods · máximo 10.000 linhas"_; txt também vale. O arquivo pode ter até 20 MB e só a primeira aba é lida. Mostra _"Lendo a planilha…"_ enquanto lê.
2. **Mapear as colunas** — Em "Mapeamento de colunas", cada "Coluna da planilha" vira um "Campo no Convergefy", com exemplos (_"Ex.: …"_). Exatamente uma coluna vira Telefone. O que não quiser trazer fica em "Ignorar". Em "Tags a aplicar (opcional)", escolha etiquetas para todos os contatos da importação. "Redefinir" refaz o palpite; **"Continuar"** só habilita com o mapeamento válido.
3. **Confirmar e importar** — O resumo mostra "Arquivo", "Colunas mapeadas", "Tags a aplicar" (se houver) e "Automações", com a caixa "Disparar automações" (veja abaixo). Clique em **"Importar contatos"**: _"Importação iniciada. Ela roda em segundo plano."_ Pode fechar o painel.

O contador do passo 2 avisa _"{X} de {Y} colunas mapeadas. Telefone é obrigatório."_

**Limite de linhas**

As 10.000 linhas contam só as que têm dados. Somando as vazias, o limite é de 20.000 linhas lidas.

**Regras da planilha**

- **Destinos das colunas:** Telefone (obrigatório), Nome, E-mail, Documento, Endereço, ID externo, Atendente principal (e-mail) e os campos personalizados, cada um com uma coluna. Colunas sem nome são descartadas; duas colunas com o mesmo nome impedem a importação.
- **Telefone brasileiro** vale como estiver, com ou sem código do país, parênteses, hífen ou espaço: `(11) 98765-4321`, `11987654321` e `+55 11 98765-4321` são o mesmo contato.
- **Telefone de outro país** precisa do `+` (ex.: `+1 212 555-1234`); sem ele, é tratado como brasileiro. Se a planilha apagar o `+`, escreva um apóstrofo antes: `'+1 212 555-1234`. O apóstrofo não é gravado, só faz a célula virar texto.
- **Atendente principal:** use o e-mail do membro, não o nome. A tela avisa: _"A coluna deve conter o e-mail do membro da empresa no Convergefy — não o nome. Linhas com e-mail que não corresponda a um membro ativo não são importadas."_ A linha vai para o relatório de erros e o contato não entra.
- **Campos personalizados:** o valor tem que combinar com o tipo, senão a linha vai para o relatório de erros. Número: numérico. Data: `AAAA-MM-DD` (ex.: `2026-12-31`), não `31/12/2026`; para outro formato, use um campo Texto. Seleção única: igual a uma das opções.

**Por que uma linha não entra**

Os motivos mais comuns no relatório de erros:

- _"Telefone inválido ou ausente. Número internacional deve ser marcado com +."_
- _"Telefone duplicado no arquivo."_
- _"Linha sem dados nas colunas mapeadas."_
- _"Atendente principal não encontrado: nenhum membro ativo desta empresa tem este e-mail."_
- _"Valor excede o limite de 255 caracteres."_ (Nome, E-mail ou Documento.)

### Disparar automações na importação

> **Cuidado com bases grandes**
>
> Milhares de contatos com a caixa marcada podem disparar milhares de automações de uma vez.

A caixa "Disparar automações" (_"Os contatos desta importação disparam as automações."_) vem desmarcada: assim, nenhuma automação é acionada. Marcada:

- cada contato novo conta como contato criado e pode acionar automações com esse gatilho;
- cada tag da importação que o contato ainda não tinha conta como tag adicionada e pode acionar automações com esse gatilho (ver [Automações](https://docs.convergefy.com.br/kb/automacoes.md)).

Quem já existia não conta como contato criado, e quem já tinha a tag não a recebe de novo. Por isso, importar a mesma planilha outra vez não repete essas automações para esses contatos.

**Sobre o cancelamento**

O cancelamento é conferido a cada 500 linhas (50 com a caixa marcada) e pode demorar alguns instantes.

### Acompanhar a importação

Roda em segundo plano; com uma em andamento, o botão "Importar" ganha um pontinho pulsando. No histórico, cada linha mostra o progresso (_"{X}% de {Y} linhas"_) e o estado:

- **Na fila** (gray) — aguardando começar.
- **Processando** (blue) — importando as linhas.
- **Concluída** (green) — terminou. Resumo (ex.: _"{n} importados · {n} com erro · {n} duplicadas"_); "com erro" e "duplicadas" só aparecem se houver.
- **Falhou** (red) — a importação não completou. A linha mostra o motivo. Como resolver: use “Reprocessar” na linha, ou baixe o relatório de erros para corrigir a planilha.
- **Cancelada** (gray) — você interrompeu. Os contatos já importados ficam.

O resultado chega no sino de notificações, não em um aviso que some (ver [Notificações](https://docs.convergefy.com.br/kb/notificacoes.md)).

Na linha aparecem "Cancelar" (em andamento: _"Cancelar importação?"_ / _"Os contatos já importados serão mantidos."_) e "Reprocessar" (se falhou; não duplica contatos). O menu de três pontinhos traz:

- **Baixar relatório de erros** — Só aparece se houve linhas com erro ou duplicadas. Baixa um csv com linha, tipo, motivo e valores, para corrigir e reenviar.
- **Baixar planilha original** — O arquivo que você subiu. Fica guardado enquanto o registro estiver no histórico.
- **Excluir** — Remove o registro e a planilha original: _"Isto remove apenas o registro. Os contatos importados não são apagados."_ Indisponível na fila ou processando.

## Ver e editar um contato

Clique na linha do contato para abrir o painel lateral. No topo ficam o nome (lápis para renomear), o atendente principal e _"Criado em {data}"_. O "+" ao lado do nome adiciona tags; o × que surge ao passar o mouse sobre uma tag a remove.

A edição é direto no lugar, sem "Salvar": cada campo salva ao confirmar (Enter ou clique fora), com _"Contato atualizado com sucesso."_ Sem Editar, o painel é só leitura e campos vazios mostram _"Não informado"_.

> **As abas do painel**
>
> "Informações" (os dados abaixo) aparece sempre que há abas. "Rastreio" aparece se o contato tem origem rastreada ou respostas de formulário de anúncio da Meta, para todos os membros. "Configurações" (bloqueio de mensagens) aparece só com Administrar. Sem nenhuma delas, só os dados.

- **Informações de Contato** — Telefone, E-mail, CPF/CNPJ, Endereço e ID Externo. Clique no lápis para editar; onde está vazio aparece "Adicionar".
- **Campos personalizados** — Logo abaixo, se a empresa tiver, preenchidos do mesmo jeito.

> **A aba “Rastreio”**
>
> Traz a seção "Origem do contato": a plataforma (Meta Ads, Google Ads ou Outra origem), o anúncio e a campanha do clique que trouxe o contato, os "Detalhes da origem" (com as UTMs, os códigos que marcam de onde veio o clique) e as respostas de formulário. É a mesma seção do painel do Chat. Detalhes em [Rastreamento](https://docs.convergefy.com.br/kb/meta-ads.md).

O painel direito da conversa no [Chat](https://docs.convergefy.com.br/kb/chat.md) edita o mesmo contato: mudou num lugar, vale no outro.

## Campos personalizados

Crie campos próprios (cargo, empresa, aniversário…). Eles aparecem em todos os contatos, na lista e no painel do Chat.

> **Quem gerencia os campos**
>
> O botão "Campos personalizados" só aparece com Administrar. Quem tem Editar preenche os valores, mas não cria nem apaga campos.

### Criar e organizar

> **O tipo não muda depois de criado**
>
> _"O tipo não pode ser alterado após a criação."_ Para outro tipo, crie um campo novo.

O botão abre um painel lateral: _"Crie campos para enriquecer seus contatos. Arraste para reordenar."_ Cada campo mostra o nome e o selo do tipo (_Texto_, _Número_, _Data_ ou _Seleção_). Ao passar o mouse aparecem o lápis (editar) e a lixeira.

1. **Novo campo** — Clique em **"Novo campo"**. Informe o Nome (_"Ex: Cargo, Empresa, Aniversário"_, sem repetir um nome já usado) e o Tipo.
2. **Opções (só para “Seleção única”)** — Aparece o bloco "Opções": clique em "Adicionar opção" para cada escolha. É preciso ao menos uma (_"Adicione ao menos uma opção."_) e nenhuma pode ficar em branco (_"A opção não pode ficar em branco."_).
3. **Salvar** — Clique em **"Salvar"**. Para reordenar, arraste pela alça (⋮⋮).

Os tipos são Texto (livre), Número, Data (com hora) e Seleção única (lista de opções fixas; o contato recebe uma).

### Preencher e excluir

> **Excluir um campo não tem volta**
>
> Apagar um campo remove o valor dele de todos os contatos e não pode ser desfeito. A lixeira pede confirmação: _"Excluir campo?"_ / _"Isso remove o campo e seu valor de todos os contatos. Não dá para desfazer."_

O valor é preenchido por contato: no "Novo Contato" ou no painel do contato (na lista ou no Chat). Onde está vazio aparece "Adicionar"; nos campos de data e de seleção dá para "Limpar valor".

## Bloquear as mensagens de um contato

> **As mensagens bloqueadas não voltam**
>
> O que chega com o bloqueio ligado é perdido para sempre; desligar não recupera nada.

Na aba "Configurações" do painel (nível Administrar) fica "Bloquear mensagens recebidas": _"Para contatos que trafegam dado sensível. As mensagens que ele enviar não são armazenadas."_

Ligado, tudo que o contato enviar é bloqueado na chegada e descartado: não entra no Chat, não notifica ninguém, não dispara automações e não registra origem de anúncio/UTM. O envio para ele continua funcionando e o histórico existente é preservado.

Ligar pede confirmação ("Bloquear as mensagens deste contato?", ação "Bloquear mensagens"). Com o bloqueio ativo, o cabeçalho ganha o selo "Bloqueado", visível para todos os membros.

> **“Bloquear” aqui = descartar o que ele envia**
>
> Não é um bloqueio do WhatsApp e não impede você de enviar mensagens para ele.

## Filtrar e encontrar contatos

A busca "Buscar contatos..." procura por nome, e-mail, ID externo, telefone ou documento. O botão de filtro abre "Filtrar por" (com "Limpar") e combina quatro critérios:

- **Departamentos** — Contatos com conversa no departamento. Escolha um; clicar de novo limpa.
- **Atendente principal** — Pelo atendente principal do contato, não por quem atende a conversa. Tem busca por nome e a opção "Sem atendente principal" no topo (some enquanto você digita). Escolha um.
- **Status** — "Aguardando", "Em atendimento" ou "Finalizado". Escolha um.
- **Tags** — Dá para marcar várias: traz quem tem ao menos uma.

O filtro por quem atende a conversa não existe aqui; fica no [Chat](https://docs.convergefy.com.br/kb/chat.md).

> **“Status” é o da conversa, não do cadastro**
>
> Um contato não fica "aguardando" como pessoa: é a conversa que está aguardando, em atendimento ou finalizada (ver [Atendimento / Chat](https://docs.convergefy.com.br/kb/chat.md)). O contato aparece se ao menos uma conversa dele está no estado escolhido.

A paginação fica acima da tabela: _"Página X de Y"_ à esquerda e as páginas numeradas, com "…" e setas, à direita.

## Limites e regras

> Telefone é o único campo obrigatório. Nome, e-mail e documento aceitam até 255 caracteres; endereço, até 500. O documento só é conferido na edição pelo painel (11 dígitos de CPF ou 14 de CNPJ). Em qualquer caminho o sistema recalcula os dois dígitos verificadores (os dois últimos, que ele calcula sozinho), então um número errado pode ser gravado diferente do digitado, sem aviso.

## Excluir um contato

> **Excluir apaga também as conversas e os negócios dele**
>
> Somem junto, de forma permanente, todo o histórico de conversa no Chat, todos os negócios do Funil e as mensagens agendadas do contato. Para só tirar da lista, prefira remover as tags.

Exige Editar. Use a lixeira da coluna "Ações" ou o botão "Excluir contato" no rodapé do painel. A confirmação "Excluir contato" diz: _"Tem certeza que deseja excluir o contato {nome}? Esta ação não pode ser desfeita."_ Depois aparece _"Contato excluído com sucesso!"_

## Exportar contatos

"Exportar" leva para uma planilha o recorte da tela: tudo que casa com a busca e os filtros, inclusive as outras páginas. Não existe seleção de linhas.

> **Não feche a aba durante a exportação**
>
> Fechar ou atualizar a aba recomeça do zero. Se parar no meio, dá para "Baixar parcial" (o arquivo leva `-parcial` no nome) ou "Tentar de novo".

1. **Escolher as informações** — Clique em **"Exportar"**. Abre "Exportar contatos" com _"{N} contatos no filtro atual."_ e os grupos de informação (veja abaixo). Tudo vem marcado; cada grupo tem "Marcar todos" / "Desmarcar todos", e a escolha fica lembrada.
2. **Exportar** — Clique em **"Exportar"** de novo. O CSV (`contatos-AAAA-MM-DD-HHMM.csv`) é gerado no seu computador: _"Você pode continuar usando o sistema, mas fechar a aba recomeça a exportação do zero."_ O botão mostra _"Exportando X%"_; clique nele para reabrir o progresso, onde há "Cancelar".
3. **Baixar** — No fim aparece _"{N} contatos exportados."_ com "Baixar novamente", caso o download não tenha começado sozinho.

**Quais informações entram no arquivo**

- **Contato:** nome, telefone, e-mail, CPF/CNPJ, endereço, tags, ID externo.
- **Atendimento:** "Atendente responsável" (que é o atendente principal), "Criado em", "Atualizado em".
- **Negócios:** quantidade e valor por situação, ex.: "Negócios em aberto (qtd)" e "Negócios em aberto (R$)", o mesmo para ganhos e perdidos.
- **Origem do contato** e **Campos personalizados**.

**Como o arquivo é formatado**

O CSV abre direto no Excel em português. Ele usa `;` como separador, separa as tags de uma célula com `|` e traz os valores de negócios em reais, com vírgula e sem "R$" (ex.: `1250,50`).

> **Filtro vazio não exporta**
>
> Sem ninguém no recorte, a tela avisa _"Nenhum contato no filtro atual. Ajuste a busca ou os filtros para exportar."_ e o botão fica desativado.

## Erros e mensagens esperados

- “O telefone é obrigatório” — salvou sem telefone. Resolver: preencha o Telefone.
- “Telefone inválido. Verifique o número informado.” — número inválido. Resolver: confira DDD e dígitos, com DDI (ex.: +55 (11) 99999-9999).
- “Digite um e-mail válido” — formato inválido. Resolver: use nome\@dominio.com ou deixe em branco.
- “Informe um CPF (11 dígitos) ou CNPJ (14 dígitos), ou deixe em branco.” — dígitos que não são de CPF/CNPJ. Resolver: corrija o número ou apague o campo.
- “Não foi possível criar o contato.” — falha ao criar. Resolver: tente de novo; se persistir, confira a internet e recarregue.
- “Não foi possível salvar o nome.” — falha ao salvar o nome. Resolver: tente de novo; se persistir, recarregue e reabra o contato.
- “Não foi possível salvar as informações de contato.” — falha ao salvar telefone, e-mail, documento, endereço ou ID externo. Resolver: tente de novo; se persistir, recarregue.
- “Não foi possível salvar os campos personalizados.” — falha ao salvar um campo personalizado. Resolver: preencha de novo. No cadastro, se vier junto com “Contato criado com sucesso!”, o contato existe: abra-o e preencha os campos.
- “Não foi possível salvar o atendente principal.” — falha ao salvar. Resolver: escolha de novo; se persistir, recarregue.
- “Não foi possível excluir o contato.” — falha ao excluir. Resolver: tente de novo; se persistir, recarregue.
- “Não foi possível atualizar as tags do contato.” — falha ao alterar as tags. Resolver: tente de novo; se persistir, recarregue.
- “Nenhum lead encontrado.” — lista vazia ou busca sem resultado. A tela diz "lead", que é o mesmo que contato. Resolver: ajuste a busca ou limpe os filtros.
- “Já existe um campo com esse nome.” — nome já usado por outro campo. Resolver: escolha outro nome.
- “Revise as opções da lista: nenhuma pode ficar vazia.” — opção vazia ou longa demais no campo de seleção única. Resolver: preencha ou remova as opções em branco.
- “Não foi possível ler a planilha. Confira se o arquivo não está corrompido.” — arquivo ilegível. Resolver: salve de novo como csv, xlsx ou ods e reenvie.
- “Máximo de 10000 linhas por importação. Divida o arquivo.” — passou do limite de linhas. Resolver: separe em arquivos menores.
- “A planilha tem linhas vazias demais. Remova as linhas em branco e tente novamente.” — muitas linhas sem dado. Resolver: apague as linhas em branco e reenvie.
- “A planilha não tem linhas de dados para importar.” — só o cabeçalho foi encontrado. Resolver: inclua ao menos uma linha abaixo do cabeçalho.
- “Mapeie exatamente uma coluna para telefone.” — nenhuma coluna, ou mais de uma, como telefone. Resolver: aponte uma (e só uma) coluna para Telefone.
- “Cada campo só pode ser mapeado por uma coluna.” — duas colunas no mesmo campo. Resolver: deixe uma coluna por destino; as demais, “Ignorar”.
- “A planilha mudou ou tem colunas com nomes repetidos. Envie o arquivo de novo.” — colunas com o mesmo nome, ou o arquivo deixou de valer. Resolver: renomeie as colunas repetidas e suba a planilha de novo.
- “Não foi possível iniciar a importação.” — falha ao iniciar. Resolver: confirme de novo; se persistir, confira a internet e reabra a importação.
- “Só dá para cancelar uma importação pendente ou em andamento.” — importação que já terminou. Resolver: veja o estado no histórico: o que já terminou não cancela.
- “Só dá para reprocessar uma importação que falhou.” — importação que não falhou. Resolver: use “Reprocessar” só em linhas “Falhou”.
- “Cancele a importação antes de excluir.” — importação na fila ou processando. Resolver: clique em “Cancelar” e depois exclua.
- “Não foi possível baixar o arquivo.” — falha ao baixar a planilha ou o relatório. Resolver: tente de novo; se persistir, recarregue.
- “Não foi possível salvar a configuração.” — falha ao salvar o bloqueio. Resolver: tente de novo; se persistir, recarregue e reabra o contato.
