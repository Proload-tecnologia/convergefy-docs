# Rastreamento: Configurar

Os dois passos para ligar os anúncios ao funil: conectar as contas de anúncio e montar o Funil de Compra.

Na Central de Ajuda: https://docs.convergefy.com.br/#/meta-ads-configurar

## Em resumo

Dois passos ligam os anúncios ao funil: conectar as contas de anúncio (Passo 1) e montar o Funil de Compra (Passo 2). Faça nessa ordem. Sem os dois, nada é enviado às plataformas.

### Algo deu errado?

Procure o que você está vendo e siga a coluna da direita. O detalhe de cada caso está mais abaixo.

| O que você vê                                                                | O que fazer                                                                                                                      |
| ---------------------------------------------------------------------------- | -------------------------------------------------------------------------------------------------------------------------------- |
| Selo "Pendente" na linha do pixel (Meta) ou da conta de anúncio (Google)     | Falta o pixel ou a conta de anúncio. Adicione o pixel ou escolha a conta.                                                        |
| "Nenhum pixel adicionado"                                                    | Sem pixel, a Convergefy não envia conversão à Meta e nada aparece em "Eventos". Adicione um pixel.                               |
| _"Sem conexão com a Meta. Os envios deste pixel vão falhar."_                | O pixel não tem token próprio e nenhuma conta do Facebook está conectada. Conecte a Meta ou informe um token.                    |
| _"A Meta recusou o token. Confira se ele tem acesso a este Pixel."_          | Gere um novo token com acesso ao pixel, ou deixe o campo em branco para usar a conexão com a Meta.                               |
| As respostas de formulário não chegam                                        | Veja o aviso "As respostas não chegam?", abaixo: o acesso a leads precisa incluir a Convergefy na Meta.                          |
| Uma conta de anúncio ou Página criada depois não aparece                     | Nada muda sozinho. Conecte de novo escolhendo o mesmo portfólio empresarial.                                                     |
| Um evento de site (ex.: Contact ou Schedule) aparece como falha em "Eventos" | Para contato que veio de anúncio de WhatsApp, a Meta só aceita os eventos de conversa. Escolha outro evento.                     |
| Funil mapeado antes sumiu do mapeamento                                      | Salvar substitui o mapeamento da empresa inteira. Veja o aviso do Passo 2 e mapeie de novo.                                      |
| Mapeamento Google sumiu                                                      | Trocar ou desconectar a conta de anúncio do Google apaga as ações de conversão escolhidas. Mapeie de novo.                       |
| Erro ao conectar a Meta ou o Google                                          | Veja "Erros e avisos esperados", em [Acompanhar](https://docs.convergefy.com.br/kb/meta-ads-acompanhar.md). |

## Passo 1: Contas de Anúncio

A tela "Contas de Anúncio" tem dois blocos, Meta e Google Ads. Com algo configurado, o bloco ganha o botão **"Gerenciar"**. Os selos "Conectado" e "Pendente" aparecem por linha dentro do bloco. "Pendente" marca o que falta: o pixel (Meta) ou a conta de anúncio (Google).

### Conectar a Meta

Sem nada configurado, o bloco mostra o botão **"Configurar Meta"** (sem Administrar, só _"A Meta ainda não foi conectada."_). Depois de conectar, mostra:

- as linhas "Conta do Facebook" e "Pixel · API de Conversões" (com setas ‹ › e _"1 / N"_ quando há mais de um);
- o botão **"Gerenciar"**.

Os dois botões abrem o painel "Configurar Meta", com as seções "Conexão com a Meta" e "Pixel · API de Conversões". Sem Administrar, o painel se chama "Meta" e é só leitura.

#### Conexão com a Meta

Conectar a conta do Facebook que administra seus anúncios é o que permite descobrir de qual campanha veio cada lead. O link "Como conectar suas contas" (só para quem pode alterar) resume estes passos.

1. **Conectar** — Clique em **"Conectar com Facebook"**. Na janela da Meta, entre com a conta que administra seus anúncios, escolha o portfólio empresarial (o agrupamento da Meta que reúne suas contas de anúncio, Páginas e pixels) e marque as contas de anúncio, as Páginas e os pixels que a Convergefy pode usar.
2. **Aguardar** — O painel fica coberto por "Conectando sua conta da Meta" (_"Pode levar alguns segundos. Mantenha esta tela aberta."_), em geral de 5 a 10 segundos. Ao final aparece "Conta da Meta conectada com sucesso." e os pixels compartilhados entram sozinhos.
3. **Pronto** — A conexão vira um card com o nome, o selo "Conectado", o ID, _"Conectada desde {data}"_ e dois links: de contas (ex.: _"3 contas de anúncio liberadas"_) e de Páginas (ex.: _"2 Páginas recebendo Lead Ads"_). Lead Ads são os formulários instantâneos dos anúncios do Facebook e do Instagram.

Cada portfólio empresarial vira um card. Criou uma conta de anúncio depois, ou quer incluir ou tirar uma Página? Nada muda sozinho: conecte de novo escolhendo o mesmo portfólio e ajuste a escolha na Meta. A conexão é atualizada, não duplicada. Conta de anúncio em outro portfólio exige conectar aquele portfólio também.

> **Desconectar revoga o acesso**
>
> O botão **"Desconectar"** (no card) revoga o acesso. Anúncios que só essa conta enxerga deixam de ser atribuídos a novos leads: campanha e anúncio ficam vazios. As Páginas da conexão deixam de enviar respostas de formulário, salvo se outra conexão as incluir. Eventos e atribuições já registrados ficam, e dá para reconectar quando quiser.

**Várias contas e validade do acesso**

Com várias contas do Facebook conectadas, a Convergefy consulta uma a uma, da mais antiga para a mais nova, até alguma enxergar o anúncio. O acesso dura cerca de 60 dias e é renovado sozinho, todo dia, quando faltam 7 dias ou menos.

Se a conexão falhar, veja "Erros e avisos esperados", em [Acompanhar](https://docs.convergefy.com.br/kb/meta-ads-acompanhar.md).

#### Contas liberadas e Páginas

- **N contas de anúncio liberadas** — Lista as contas que a conexão liberou. A busca aparece com mais de 8 contas. Se a Meta tinha mais contas do que coube, um aviso diz que a lista mostra só as primeiras. É um retrato do momento da conexão: contas liberadas ou renomeadas depois só aparecem ao reconectar.
- **N Páginas recebendo Lead Ads** — Lista as Páginas que enviam à Convergefy as respostas dos formulários instantâneos (Lead Ads). Para incluir ou tirar Páginas, reconecte o mesmo portfólio.

> **Respostas novas disparam automações**
>
> Antes de buscar respostas: as que ainda não entraram disparam as automações do gatilho "Formulário da Meta". Por isso o período é curto: buscar semanas atrás pode mandar mensagem a quem preencheu há muito tempo. Ver [Automações](https://docs.convergefy.com.br/kb/automacoes.md).

Nessa lista de Páginas, quem tem Administrar vê "Buscar respostas dos últimos" com o "Período da busca" (24 horas, 7 dias ou 30 dias) e o botão **"Buscar respostas"**. Traz da Meta as respostas que não chegaram sozinhas, de todas as Páginas ligadas, com a barra _"Buscando… N%"_. Ao terminar: "Busca de respostas concluída." (ou "Busca concluída, mas parte das Páginas não respondeu.").

**O que acontece com cada resposta**

Cada resposta vira um contato. A Convergefy procura o contato pelo telefone e, se não achar, pelo e-mail. Se não existir, cria um novo. Resposta sem telefone e sem e-mail falha: não cria contato e não dispara o gatilho "Formulário da Meta". A mesma resposta nunca é processada duas vezes, mesmo que chegue de novo pela busca.

> **As respostas não chegam?**
>
> O portfólio empresarial na Meta pode ter personalizado o acesso a leads, de modo que só os CRMs de uma lista recebem as respostas. Se a Convergefy não está na lista, nenhuma resposta chega. Nas configurações de acesso a leads da Página ou do portfólio, na Meta, volte ao acesso padrão ou inclua a Convergefy na lista de CRMs com acesso. A Convergefy não consegue fazer isso por você.

#### Pixel · API de Conversões

Todos os pixels recebem as conversões do funil e os leads dos formulários dos anúncios. Os pixels compartilhados na conexão entram sozinhos. Sem nenhum, aparece "Nenhum pixel adicionado" e a linha do bloco Meta fica "Pendente".

> **Sem pixel, nada é enviado à Meta**
>
> Sem pixel cadastrado, a Convergefy não envia conversão à Meta, e nada aparece em "Eventos".

Cada pixel mostra nome, selo "CRM" (se for de CRM), ID e a origem do token: "Token próprio" ou "Usa a conexão com a Meta". Pixel sem token próprio e sem nenhuma conta do Facebook conectada mostra _"Sem conexão com a Meta. Os envios deste pixel vão falhar."_

1. **Adicionar um pixel que a Meta enxerga** — Clique em **"Adicionar pixel"**, busque em "Buscar pelo nome ou ID" e clique no pixel. Ele entra na hora, com o nome e a marcação de CRM que vêm da Meta. Os já cadastrados têm o marcador "Adicionado".
2. **Ou adicionar manualmente** — Para um pixel que suas contas conectadas não enxergam, clique em **"Adicionar manualmente"** e preencha "ID do pixel" (só números; na Meta, Gerenciador de Eventos, Fontes de dados), "Nome" e, se quiser, "Token de acesso". Marque "Pixel de CRM" se for o caso. O link "Como obter as credenciais" mostra onde achar o ID e gerar o token.

- **Token de acesso** — Opcional. Sem token, o envio usa as conexões com a Meta. Se preencher, precisa ter ao menos 20 caracteres. Se a Meta recusar: _"A Meta recusou o token. Confira se ele tem acesso a este Pixel."_
- **Pixel de CRM** — Marque se ele já foi convertido em pixel de CRM na Meta. É só uma indicação: não muda quem recebe os envios, que vão para todos os pixels.

O menu ⋯ de cada linha (só com Administrar) traz:

- **Opções avançadas** — Edita o "Nome", o "Token de acesso" e a marcação "Pixel de CRM". O ID fica travado (para usar outro pixel, remova este e adicione o novo). A marcação de CRM vem da Meta só quando o pixel é adicionado: se ele foi convertido em pixel de CRM depois, marque aqui. A Meta nunca exibe o token salvo: preencha só para trocar. Sem token, o pixel envia pelas conexões com a Meta e, se todas forem desconectadas, os envios param.
- **Remover** — Em "Remover pixel", o pixel para de receber conversões na hora. Os eventos já enviados ficam no histórico. Os outros pixels continuam recebendo.

> **Quem recebe as conversões do funil**
>
> A conversão de cada etapa mapeada vai para todos os pixels cadastrados, marcados como "Pixel de CRM" ou não. Só muda o formato para o contato cuja origem mais recente é a resposta a um formulário de anúncio (Lead Ads): as etapas dele, e o próprio lead da resposta, vão como evento de CRM (Conversion Leads), também para todos os pixels.
>
> Cada pixel recebe um envio próprio, e cada envio é uma linha em "Eventos". Com 2 pixels, cada conversão aparece 2 vezes.

### Conectar o Google Ads

Sem nada configurado, o bloco Google Ads mostra o botão **"Conectar com Google"**. O login acontece numa página à parte: você sai da Convergefy, autoriza no Google e volta. Ao voltar aparece _"Conta do Google conectada."_ e o painel abre na escolha da conta. Enquanto não escolher a conta de anúncio que receberá as conversões, a linha "Conta de anúncio" fica "Pendente".

> **Trocar ou desconectar apaga os mapeamentos Google do Funil**
>
> Ao trocar a conta de anúncio, as ações de conversão do Google já escolhidas no Funil de Compra são apagadas. Mapeie-as de novo para a nova conta. Ao desconectar ("Desconectar do Google?"), o acesso é revogado, a conta de anúncio escolhida é removida e os mapeamentos Google do Funil deixam de existir. Dá para reconectar quando quiser.

O botão **"Gerenciar"** abre o painel "Gerenciar Google Ads":

- **Conta Google** — O e-mail conectado, o selo "Conectado" e _"Conectada desde {data}"_, com **"Reconectar"** e **"Desconectar"**.
- **Conta de anúncio** — Um seletor ("Selecionar conta", com busca por nome ou ID e "Atualizar lista"). Com conta escolhida, mostra o nome e o botão **"Trocar conta"**, que pede confirmação.

## Passo 2: Funil de Compra

Aqui você cria o mapeamento: quais etapas viram quais conversões, em cada plataforma configurada. Sempre que um negócio entra numa etapa mapeada, a Convergefy envia a conversão. Vale avançar o negócio até ela e também criá-lo já nessa etapa (inclusive por automação). Reordenar dentro da mesma etapa não envia nada. Se o negócio sair e voltar à etapa, é uma nova conversão.

> **Salvar substitui o mapeamento da empresa inteira: só um funil por vez**
>
> Antes de salvar: a tela mapeia um funil de cada vez, e salvar substitui o mapeamento de toda a empresa pelo do funil na tela. Os mapeamentos de outros funis são removidos: na prática, só um funil tem mapeamento ativo. Salvar sem nenhuma linha apaga tudo, e nenhuma conversão é enviada até você mapear de novo. A configuração é pensada para o seu funil de compra principal.

1. **Escolher o funil** — No campo "Funil", escolha um dos seus funis. Mapeamentos já salvos aparecem preenchidos.
2. **Mapear etapa e conversão** — Cada bloco liga uma "Etapa" a uma conversão em cada provedor, marcado pelo logo:

   - Meta: "Selecionar evento", com o evento oficial da Meta.
   - Google: "Selecionar ação", com a ação de conversão (busca por nome ou ID; "Remover ação" desfaz a escolha).

   Use **"Adicionar etapa"** para mais linhas. Cada etapa só pode ser usada uma vez. Repetir o mesmo evento da Meta (ou a mesma ação do Google) na mesma etapa é recusado, porque dobraria a conversão em todos os pixels. Provedor ainda não configurado não mostra a sua linha, e um aviso no topo diz o que falta em "Contas de Anúncio". A lixeira ("Remover mapeamento") tira a linha, inclusive a última. Sem linhas, a tela mostra "Nenhuma etapa mapeada".
3. **Salvar** — Clique em **"Salvar mapeamento"**. O botão só habilita com mudança válida.

**Eventos da Meta (nomes oficiais)**

Na Meta, o evento é identificado pelo nome oficial, em inglês. A Convergefy mostra uma descrição em português ao lado. Os principais:

| Evento                          | O que significa                                                |
| ------------------------------- | -------------------------------------------------------------- |
| ViewContent                     | Contato viu um produto ou material enviado na conversa.        |
| LeadSubmitted                   | Contato deixou os dados e virou um lead pela conversa.         |
| QualifiedLead                   | Lead com perfil e intenção reais de compra (já triado).        |
| AddToCart                       | Contato escolheu um produto e demonstrou intenção de comprar.  |
| InitiateCheckout                | Contato começou a fechar o pedido (preço, pagamento, entrega). |
| CartAbandoned                   | Demonstrou interesse, mas parou antes de comprar.              |
| OrderCreated                    | Pedido registrado (ainda não pago/enviado).                    |
| Purchase                        | Contato concluiu a compra pela conversa.                       |
| OrderShipped / OrderDelivered   | Pedido despachado / entregue.                                  |
| OrderCanceled / OrderReturned   | Pedido cancelado / devolvido.                                  |
| RatingProvided / ReviewProvided | Contato deu uma nota / deixou um comentário.                   |

A lista inclui também os eventos padrão de site: Lead, CompleteRegistration, Contact, Schedule, SubmitApplication, StartTrial, Subscribe, AddPaymentInfo, AddToWishlist, CustomizeProduct, Search, FindLocation e Donate.

> **Eventos de site não valem para contatos de anúncio de WhatsApp**
>
> Para contatos que chegaram por anúncio de WhatsApp (o que abre a conversa), a Meta só aceita os eventos de conversa da tabela. Um evento de site (ex.: Contact ou Schedule) enviado a esse contato é recusado e aparece como falha em "Eventos". Para contatos vindos do seu site, os eventos de site funcionam.

No Google, você escolhe uma ação de conversão já criada na sua conta. A lista traz só ações ativas, de importação offline ou de site, e mostra só o nome. Havendo nomes parecidos, confira no Google Ads qual é a certa.

**O que cada envio leva e quando acontece**

- Quando: na entrada na etapa mapeada, com o horário dessa entrada.
- Para quem: o contato não precisa ter vindo de anúncio. Com anúncio, o identificador do clique vai junto e melhora a correspondência. Sem anúncio, a plataforma tenta casar pelos dados do contato (telefone, e-mail, nome), enviados com hash (conversão em código que não dá para desfazer). Sem o clique, a Meta pode recusar o evento por falta de dados, e aparece "Falhou" em "Eventos".
- Anúncio de WhatsApp sem o código do clique: se a mensagem chega com o anúncio, mas sem o identificador de clique (ctwa\_clid), ela não conta como vinda de um anúncio que abre o WhatsApp. A conversão vai como a de um contato do site, casada pelos dados do contato, e o anúncio continua aparecendo como origem. No WhatsApp Web o código depende do aparelho de quem escreveu e às vezes não vem.
- Valor: se o negócio tem valor maior que zero, ele vai junto, em reais (BRL), e aparece no detalhe do envio como "Valor".
- Falhou: um envio que falhou não é reenviado sozinho. A próxima entrada na etapa gera um envio novo.
