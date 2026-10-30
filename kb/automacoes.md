# Automações

Uma automação é um fluxo que reage sozinho a um evento e executa passos, sem ninguém fazer à mão. Você monta uma vez (gatilhos, blocos e ligações) e ela roda em cada contato.

Na Central de Ajuda: https://docs.convergefy.com.br/#/automacoes

## Em resumo

Uma **automação** reage sozinha a um evento e executa passos. Exemplo: _quando o cliente manda a primeira mensagem, responder com uma saudação, aplicar uma tag e criar um negócio no funil._

Gatilhos dão a partida, blocos fazem o trabalho e ligações dizem a ordem. Tudo fica na barra lateral → Automações.

### Algo deu errado?

Procure o que você está vendo e siga a coluna da direita.

| O que você vê                                                                                                                  | O que fazer                                                                                                            |
| ------------------------------------------------------------------------------------------------------------------------------ | ---------------------------------------------------------------------------------------------------------------------- |
| "Somente leitura: você não tem permissão para editar automações." no editor, ou sem os botões "Criar automação" e "Nova pasta" | Peça a um Administrador o nível Administrar em Automações, na aba Acesso do seu membro.                                |
| "Não foi possível criar a automação."                                                                                          | Tente de novo.                                                                                                         |
| "A automação foi criada, mas o gatilho não foi salvo. Escolha o gatilho no editor."                                            | Abra a automação e escolha o gatilho no editor. Veja [Gatilhos](https://docs.convergefy.com.br/kb/automacoes-gatilhos.md). |
| "O passo de ramificação deve ser o último. Crie um novo bloco ligado a uma das saídas."                                        | Mova o passo para o fim do bloco e continue o fluxo num bloco novo, ligado a uma das saídas.                           |

### Os termos desta página

- **Gatilho** — O evento que inicia o fluxo (ex.: "o contato mandou uma mensagem"). A automação pode ter vários, e cada um a inicia sozinho.
- **Bloco** — Cada caixa do quadro. Mensagem, Ações e Espera guardam uma sequência de passos. Os demais fazem uma coisa só (decidir um caminho, chamar um agente, encerrar o fluxo…).
- **Passo** — Cada item dentro de um bloco: um texto, um áudio, aplicar uma tag, esperar uma resposta…
- **Ligação** — A linha que liga a saída de um bloco à entrada do próximo.
- **Saída** — Ponto de onde sai uma ligação. Blocos que decidem ou esperam têm várias (ex.: _Encontrado_ / _Não encontrado_, _Tempo esgotado_).
- **Execução** — Uma "rodada" da automação para um contato. Cada disparo gera uma.
- **Variável** — Texto que a automação preenche sozinha, como o nome ou o telefone do contato.

## Quem pode ver e quem pode editar

Qualquer pessoa da empresa vê a lista, as pastas e o editor (em somente leitura), acompanha as execuções e dispara pelo Chat as automações com o gatilho "Execução manual".

Criar e alterar exige o nível **"Administrar" em Automações**, definido na aba Acesso do membro (ou ser Administrador da empresa; veja [Equipe e permissões](https://docs.convergefy.com.br/kb/equipe-permissoes.md)). Esse nível libera:

- criar, editar, ativar, pausar, arquivar, duplicar e excluir automações;
- gerenciar pastas;
- cancelar uma execução.

Sem ele, não aparecem "Criar automação", "Nova pasta", a alça de arrastar, o **+** da pasta, o menu de três pontos nem o botão de cancelar execução. O editor avisa _"Somente leitura: você não tem permissão para editar automações."_

> **Por que o nível é separado**
>
> As automações rodam como sistema: quem as edita consegue agir em conexões fora da própria restrição de conexões. Dê esse nível só a quem você confia para isso.

## A lista de automações

Na barra lateral, clique em **Automações**. Na lista você vê:

- o ponto colorido do status e o nome de cada automação;
- no topo, a busca "Buscar por nome…", que só aparece com ao menos uma automação;
- ao passar o mouse, para quem administra: a alça de arrastar (à esquerda) e o menu de ações (à direita);
- no rodapé, "Criar automação" e "Nova pasta" (também só para quem administra).

### Pastas

Pastas agrupam automações do jeito que você preferir.

1. **Criar a pasta** — Clique em **"Nova pasta"**: _"Agrupe as automações do jeito que fizer sentido para você."_ Informe o "Nome da pasta" (ex.: _"Ex.: Pós-venda"_) e clique em **"Criar pasta"**.
2. **Colocar automações nela** — Arraste a automação pela alça até a pasta. Pasta sem nada mostra _"Pasta vazia. Arraste uma automação para cá."_ Automações fora de pasta ficam em "Sem pasta"; para tirar uma da pasta, arraste-a até ele (_"Solte aqui para tirar da pasta."_).

**Renomear, excluir e criar direto numa pasta**

- O botão **+** ao lado do nome da pasta cria uma automação já dentro dela.
- No menu da pasta: "Renomear" e "Excluir pasta".
- Excluir a pasta não exclui as automações: elas voltam para "Sem pasta". O diálogo pergunta _"Excluir a pasta Pós-venda?"_ (com o nome da pasta) e avisa quantas automações ficam sem pasta (_"A pasta está vazia."_ se não houver nenhuma).
- Durante uma busca, o arrastar fica desligado.

## Criar uma automação

1. **Nova automação** — Clique em **"Criar automação"**. Abre "Nova automação": _"Dê um nome e escolha o gatilho inicial."_
2. **Nome, pasta e gatilho** — Preencha o "Nome da automação" (até 80 caracteres; ex.: _"Ex.: Triagem de atendimento"_). Se a empresa tem pastas, aparece também "Pasta" (_"Sem pasta"_ por padrão). Em "Gatilho inicial", escolha um gatilho (veja [Gatilhos](https://docs.convergefy.com.br/kb/automacoes-gatilhos.md)). Dá para adicionar outros depois.
3. **Editor aberto** — Clique em **"Criar automação"**. Aparece _"Criando automação…"_ e "Automação criada" (_"Abrindo o editor…"_), já no editor visual com o gatilho posicionado.

Para partir de uma automação pronta, use "Duplicar" (veja _Ativar, pausar e arquivar_ em [Ativar e acompanhar](https://docs.convergefy.com.br/kb/automacoes-ativar.md)). Se algo falhar na criação, veja "Algo deu errado?" no começo desta página.

## O editor visual

O fluxo é um quadro visual: cada bloco é uma caixa ligada ao próximo por uma ligação. O bloco verde "Gatilhos" fica no início.

Para crescer o fluxo, arraste a partir da bolinha de saída de um bloco até um espaço vazio. Abre o painel "Adicionar bloco" (com a busca "Buscar blocos…") e o bloco escolhido já nasce ligado. Para ligar dois blocos existentes, arraste da saída de um até a entrada do outro.

Para remover uma ligação, clique nela e use a lixeira ("Excluir ligação"), ou a tecla Delete/Backspace com a ligação selecionada. Em automação arquivada não dá para excluir.

**Blocos com vários passos (Mensagem, Ações e Espera)**

Três blocos guardam vários passos: **Mensagem** (_"Envie e receba mensagens"_), **Ações** (_"Executar ações no CRM"_) e **Espera** (_"Aguardar tempo ou evento"_). Em vez de um bloco para cada coisa, você empilha passos no mesmo bloco (ex.: _Texto_, _Áudio_, _Aguardar resposta_).

Sem passo de ramificação, o bloco tem uma saída só, "Próximo passo". O painel da direita mostra "Adicione o primeiro passo:" com a grade de passos, que podem ser arrastados para mudar a ordem. Um passo que cria saídas (Menu, Menu interativo, Aguardar resposta, Aguardar evento, Randomizador) precisa ser o último do bloco: _"O passo de ramificação deve ser o último. Crie um novo bloco ligado a uma das saídas."_

Os demais blocos fazem uma coisa só:

- Contato existente
- Negócio existente
- É do atendente principal
- Tipo do anexo da mensagem
- Horário de funcionamento
- Status do atendimento
- Agente de automação
- Encerrar fluxo
- Cancelar execuções do contato

**Tratamento de erro e "Máximo de vezes"**

Em Mensagem, Ações e Espera, o rodapé do painel tem a seção recolhível "Controle":

- **"Tratamento de erro"**: _"Adiciona uma saída de erro ao bloco. Falha em qualquer passo segue por ela."_ Já vem ligado em todo bloco novo. Ligue essa saída a um caminho alternativo para a falha não encerrar a execução.
- **"Máximo de vezes"**: só aparece quando o bloco está num laço (o fluxo volta para ele). _"Quantas vezes este bloco pode rodar na mesma execução do contato."_ Padrão: 10.

Nos blocos que decidem o caminho (e nos demais de uma coisa só), a saída "Tratamento de erro" é fixa, sem interruptor, e o "Máximo de vezes" (também só num laço) fica sob o cabeçalho "Execução".

O Agente de automação tem a própria seção "Controle" (veja [o bloco Agente de automação](https://docs.convergefy.com.br/kb/automacoes-acoes.md)) e não tem "Máximo de vezes": a conversa só termina pela Inatividade ou pelo Limite de respostas.

**Salvar, desfazer, organizar e recarregar**

- **"Salvar"** grava; depois o botão mostra "Salvo" (com um "Salvo!" rápido).
- Há desfazer / refazer e **"Organizar"**, que arruma o desenho do fluxo.
- O status no topo (ex.: _● Ativa_) também é um botão: _"Clique para recarregar a versão salva"_. Com mudanças não salvas, ele pergunta "Descartar as alterações?": _"Recarregar a versão salva apaga o que você mudou e ainda não salvou."_ ("Continuar editando" ou "Descartar e recarregar"). Recarregar zera o desfazer.
- Ao sair com alterações não salvas, o navegador pergunta se quer mesmo sair. Ao trocar de tela dentro do Convergefy, a pergunta é _"Você tem alterações não salvas. Deseja sair sem salvar?"_

**Ajuda e atalhos de teclado**

O ícone **?** ao lado de "Organizar" abre "Como usar o editor": guia em 13 tópicos animados (_Comece aqui_, _Montar_, _Ativar_, _Acompanhar_) e a lista de "Atalhos de teclado".

No Windows/Linux use Ctrl; no Mac, Cmd (⌘):

| Atalho                      | O que faz                                                                      |
| --------------------------- | ------------------------------------------------------------------------------ |
| Ctrl/Cmd + S                | Salvar (só age com mudança e automação não arquivada).                         |
| Ctrl/Cmd + Shift + Z        | Desfazer.                                                                      |
| Ctrl/Cmd + Shift + Y        | Refazer.                                                                       |
| Ctrl/Cmd + Shift + S        | Organizar o fluxo.                                                             |
| Ctrl/Cmd + C / Ctrl/Cmd + V | Copiar / colar o bloco selecionado.                                            |
| Delete ou Backspace         | Apagar o bloco ou a ligação selecionada (não funciona em automação arquivada). |
| Esc                         | Fecha o painel lateral (não fecha enquanto você digita num campo).             |

Atenção: desfazer e refazer usam Shift, não o Ctrl+Z "puro" de outros programas.
