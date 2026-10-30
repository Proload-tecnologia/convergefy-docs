# Automações: Gatilhos

O gatilho é o que dá a partida na automação. Aqui estão os tipos de gatilho, como cada um se comporta e como ajustar.

Na Central de Ajuda: https://docs.convergefy.com.br/#/automacoes-gatilhos

## Gatilhos: quando o fluxo começa

Os gatilhos ficam no bloco verde "Gatilhos", que mostra quantas entradas a automação tem (ex.: _2 entradas_). Cada gatilho aparece numerado, com um resumo dos ajustes (ex.: _Conexão: Qualquer conexão_). Sem gatilho: _"Escolha o que faz esta automação começar."_

### Algo deu errado?

Procure o que você está vendo e siga a coluna da direita. O detalhe de cada caso está mais abaixo.

| O que você vê                                                                            | O que fazer                                                                                                                                                        |
| ---------------------------------------------------------------------------------------- | ------------------------------------------------------------------------------------------------------------------------------------------------------------------ |
| Duas automações passando o contato uma para a outra sem parar                            | O "Máximo de vezes" vale dentro de uma execução, não entre execuções. Filtre o Departamento ou o Atendente de destino e não transfira de volta para o mesmo lugar. |
| A automação dispara demais com uma palavra curta (ex.: "oi" também dispara com "depois") | Use "Igual à mensagem inteira" na palavra-chave.                                                                                                                   |
| A palavra-chave com acento não dispara (ex.: "promoção" não casa com "promocao")         | Cadastre as duas grafias.                                                                                                                                          |
| Contato que chegou por formulário de anúncio da Meta não dispara "Contato criado"        | Use o gatilho "Formulário da Meta".                                                                                                                                |
| URL do webhook não aparece: "Salve a automação para gerar a URL do webhook."             | Salve a automação.                                                                                                                                                 |
| Webhook responde "Automação não está ativa." (erro 404)                                  | Só automações Ativas aceitam chamadas. Ative a automação.                                                                                                          |
| Webhook responde "Método X não permitido neste webhook." (erro 405)                      | Chame com o método escolhido no gatilho.                                                                                                                           |
| Webhook responde erro 413 ou 415                                                         | 413: o corpo passou de 256 KB. 415: o Content-Type não combina com o formato escolhido.                                                                            |
| Webhook recusa chamadas                                                                  | O limite é de 60 chamadas por minuto por URL; as excedentes são recusadas.                                                                                         |
| "Conecte um gateway em Configurações > Gateways de pagamento para usar este gatilho."    | Conecte um gateway em Configurações → Integrações → Gateways de pagamento.                                                                                         |
| A lista de produtos do gatilho de Gateway de pagamento está vazia                        | Importe os produtos na tela do gateway.                                                                                                                            |
| Carrinho abandonado não inicia a automação                                               | Confira se o evento de abandono de checkout está marcado no postback do gateway e se o checkout tem telefone utilizável. Venda de teste não inicia nada.           |
| A mensagem de boleto chega de madrugada                                                  | Ligue o evento a um bloco Espera antes da mensagem. Veja "Boleto para vencer".                                                                                     |

1. **Abrir os gatilhos** — Clique no título do bloco **"Gatilhos"**. O painel "Gatilhos" (_"Tudo que pode iniciar esta automação."_) lista as ENTRADAS.
2. **Adicionar outro gatilho** — Clique em **"Adicionar gatilho"** e escolha em "Escolha um gatilho" (_"Como esta automação deve começar?"_).
3. **Ajustar um gatilho** — Clique no gatilho para abrir os ajustes. No rodapé ficam "Trocar tipo de gatilho" e "Remover gatilho".

**Uma saída para cada gatilho**

Por padrão, todos os gatilhos seguem pela mesma saída (o rodapé do bloco mostra "Saída única"): _"Desligado, todos entram no mesmo fluxo."_

Com "Uma saída para cada gatilho" ligado, cada gatilho ganha a própria saída: _"Cada gatilho vai para o bloco que você escolher."_ Assim, quem chegou por uma mensagem e quem chegou por um negócio criado seguem caminhos diferentes.

Voltar para saída única desfaz essas ligações. Se as saídas iam para blocos diferentes, o editor pergunta antes: "Desfazer as ligações de saída?". Com um gatilho de Gateway de pagamento, o modo fica fixo: _"Gatilho de pagamento tem uma saída para cada evento."_

**Trocar o tipo ou remover um gatilho**

- "Trocar tipo de gatilho": _"A configuração atual é descartada e as ligações de saída deste gatilho são desfeitas."_
- "Remover gatilho": pede confirmação em "Excluir este gatilho?". A automação deixa de começar por ele, e as execuções antigas deixam de mostrar que entraram por ali. Se ele usava "Somente na primeira vez", a contagem recomeça do zero: um gatilho novo, mesmo do mesmo tipo, dispara de novo para todas as conversas que já rodaram.

**Conexão dos gatilhos**

Essa seção só aparece no painel "Gatilhos" com 2 ou mais gatilhos: _"Cada gatilho pode ouvir uma conexão diferente, e alguns não têm conexão. Os blocos de envio em Auto saem pela conexão do gatilho que iniciou a execução."_

### Catálogo de gatilhos

Campo em branco em geral significa "qualquer" (sem filtro).

- **Mensagem recebida** — O contato manda uma mensagem. Ajustes: Conexão (_"Filtra disparos vindos desta conexão. Vazio = qualquer conexão."_), Palavras-chave (vazio = qualquer mensagem) e Quando disparar (abaixo).
- **Mensagem enviada** — O atendente envia uma mensagem. Mesmos ajustes da Mensagem recebida.
- **Negócio criado** — Ajustes: Funil e Etapa (_Qualquer funil_ / _Qualquer etapa_).
- **Negócio movido** — Um negócio muda de etapa. Ajustes: Funil, De etapa e Para etapa.
- **Negócio finalizado** — _"Inicia quando um negócio é marcado como ganho ou perda."_ Ajustes: Funil e Resultado (_Ganho_ / _Perda_ / _Qualquer resultado_).
- **Contato criado** — Um novo contato entra no sistema. Sem ajustes. Contato que chega por formulário de anúncio da Meta não dispara este gatilho; para ele, use o Formulário da Meta.
- **Formulário da Meta** — _"Inicia a cada resposta nova de formulário de anúncio da Meta, para contato novo ou que já existia. Sem filtros adicionais."_
- **Conversa criada** — Uma nova conversa é criada com o contato. Ajustes: Conexão (_"Dispara só quando a conversa nasce nesta conexão."_), Departamento e Atendente.
- **Status do contato alterado** — Ajustes: Status de origem e Status de destino, cada um entre _Aguardando_, _Em atendimento_, _Finalizado_ ou _Qualquer status_ (_"Vazio em ambos = qualquer mudança de status dispara."_).
- **Atendimento transferido** — O atendimento vai para outro departamento ou atendente. Ajustes: Departamento e Atendente (de/para). Vazio = qualquer. Veja o aviso logo abaixo sobre transferências em sequência.
- **Tag adicionada** — Ajuste: a Tag (obrigatória).
- **Execução manual** — Um atendente dispara a automação no chat. Ajuste: só Quando disparar (_Sempre_ ou _Se não estiver em execução_). Veja "Disparar à mão pelo Chat" em [Ativar e acompanhar](https://docs.convergefy.com.br/kb/automacoes-ativar.md).
- **Webhook recebido** — Um sistema externo chama uma URL exclusiva (webhook é o endereço que um sistema chama para avisar a Convergefy de que algo aconteceu). Veja o detalhe abaixo.
- **Gateway de pagamento** — O gateway (a plataforma que processa o pagamento) avisa um evento: uma compra muda de situação (boleto gerado, pix pago, cartão recusado…) ou um carrinho é abandonado. Veja o detalhe abaixo.

> **Atendimento transferido: cuidado com o laço**
>
> Transferências feitas por outra automação (ou pela própria) também disparam este gatilho. Transferir para onde o contato já está não conta como transferência e não dispara de novo. Mas, se duas automações passam o contato uma para a outra, o ciclo não para sozinho: o "Máximo de vezes" vale dentro de uma execução, não entre execuções. Para evitar, filtre o Departamento ou o Atendente de destino e não transfira de volta para o mesmo lugar.

> **Importação de contatos também dispara automações**
>
> No último passo da importação de contatos há a seção "Automações", com a caixa "Disparar automações" (_"Os contatos desta importação disparam as automações."_), desmarcada por padrão. Marcada, cada contato novo dispara "Contato criado" e cada tag da importação que o contato ainda não tinha dispara "Tag adicionada". Desmarcada, nada dispara. Veja [Contatos](https://docs.convergefy.com.br/kb/contatos.md).

**Quando disparar (Mensagem recebida e Mensagem enviada)**

- **Sempre**: dispara toda vez que o evento ocorrer.
- **Somente na primeira vez**: _"Se esta conversa já passou por esta automação antes, ela não inicia de novo."_
- **Se não estiver em execução**: _"Evita iniciar a automação duas vezes para a mesma conversa ao mesmo tempo."_
- **Só no início do atendimento**: na Mensagem recebida, _"Quando o contato envia a primeira mensagem da conversa, ou volta a escrever após o atendimento ser finalizado."_; na Mensagem enviada, quando o atendente escreve para uma conversa em espera ou já finalizada.

A Execução manual só tem "Sempre" e "Se não estiver em execução".

**Palavras-chave: contém ou igual**

Cada palavra-chave vale de um destes jeitos:

- **Contém no texto**: dispara se a palavra aparecer em qualquer parte da mensagem. Cuidado com palavras curtas: _"oi"_ também dispara com _"depois"_.
- **Igual à mensagem inteira**: só dispara se a mensagem for exatamente aquela palavra. Melhor para palavras curtas.

Nos dois, maiúsculas e minúsculas não importam (_"Oi"_ = _"oi"_), mas acentos importam: _"promoção"_ não casa com _"promocao"_. Cadastre as duas grafias. Espaços no começo e no fim da palavra são ignorados.

**Webhook recebido (para quem integra um sistema)**

> **Este gatilho não identifica o contato**
>
> Use logo depois um bloco Contato existente ou Negócio existente.

Ajustes:

- "Método HTTP aceito": _Qualquer (GET ou POST)_ / _GET_ / _POST_. Outro método é bloqueado.
- "Formato do corpo (POST)": _JSON_ / _Formulário (x-www-form-urlencoded)_ / _Texto bruto_.
- "Parâmetros da URL": o interruptor "Usar parâmetros da URL" (_"Ligado, os parâmetros viram variáveis nos próximos passos."_).
- "Headers a expor": _"Por privacidade, apenas os headers listados ficam disponíveis nos próximos passos."_

A URL só aparece depois de salvar (_"Salve a automação para gerar a URL do webhook."_), com botão de copiar e os exemplos "Copiar exemplo GET" / "Copiar exemplo POST".

Limites (valem para o sistema que chama):

- **Tamanho:** corpo de até 256 KB; acima disso, erro 413.
- **Frequência:** até 60 chamadas por minuto por URL; as excedentes são recusadas.
- **Tipo do conteúdo:** num POST com corpo, o Content-Type precisa combinar com o formato: _application/json_ para JSON, _application/x-www-form-urlencoded_ para Formulário. Senão, erro 415. Texto bruto aceita qualquer tipo.
- **Método:** com método diferente do escolhido, a resposta é _"Método X não permitido neste webhook."_ (erro 405).
- **Automação desativada:** só automações Ativas aceitam chamadas. As demais respondem _"Automação não está ativa."_ (erro 404).
- **Chamada repetida:** o cabeçalho opcional X-Idempotency-Key evita duplicar. A mesma chave em até 10 minutos devolve a mesma execução em vez de criar outra. A resposta de sucesso traz o execution\_id.

**Gateway de pagamento (Payt e outros)**

Este gatilho reage aos avisos de um gateway de pagamento integrado em Configurações → Integrações → Gateways de pagamento. Sem gateway conectado, o formulário só mostra _"Conecte um gateway em Configurações > Gateways de pagamento para usar este gatilho."_ e não lista produtos.

Ajustes:

- "Tipo de evento" (obrigatório): Cartão, Pix, Boleto ou Outros. Eventos de cada tipo:
  - Cartão: _Aprovado_, _Recusado ou cancelado_, _Estornado_.
  - Pix: _Gerado_, _Cancelado_, _Pago_, _Estornado_.
  - Boleto: _Gerado_, _Vence amanhã_, _Vence hoje_, _Vencido_, _Pago_, _Estornado_.
  - Outros: _Carrinho abandonado_ (a pessoa saiu do checkout antes de pagar).
- "Eventos": marque ao menos um. _"Cada evento marcado é uma saída do gatilho."_
- "Produtos": _"Sem produto escolhido, vale para qualquer produto."_ Os produtos vêm do gateway; com a lista vazia, importe-os na tela do gateway.
- "Conexão" (obrigatória): _"As mensagens desta automação saem por esta conexão."_

Para cobrir dois tipos de evento, use um gatilho de Gateway para cada tipo.

Regras contra mensagem repetida ou fora de hora:

- Uma confirmação por pedido: a confirmação (_Aprovado_ no cartão, _Pago_ no pix ou boleto) sai uma vez por pedido em cada automação, mesmo com vendas em formas de pagamento diferentes (upsell).
- Pedido já pago: com uma venda paga no pedido, só a confirmação e o _Estornado_ disparam. Gerado, recusado, cancelado e vencimento de venda extra ficam de fora, para não tratar quem já comprou como se a compra tivesse falhado.
- Gatilhos que se sobrepõem: se dois gatilhos de pagamento da mesma automação casam com o mesmo evento, dispara só um. Vence o que tem filtro de produto; no empate, o primeiro do bloco "Gatilhos". Automações diferentes não interferem.

Quando a situação da venda muda, a régua (a sequência de mensagens da cobrança) muda junto:

- Mudou a situação, acabou a régua antiga: quando o status de uma venda muda (ex.: o pix foi pago), as execuções em andamento ou em espera daquela mesma venda são canceladas, mesmo que a nova situação não tenha evento marcado no gatilho. Assim, quem pagou não recebe mais a cobrança do "pix gerado". Se a venda muda para uma situação do mesmo evento (ex.: cartão recusado e depois cancelado), a régua em curso segue.
- Compra nova encerra as cobranças das anteriores: quando entra uma compra nova do mesmo contato e do mesmo produto, as réguas das compras anteriores que não foram pagas são canceladas. Assim, o boleto esquecido para de cobrar quando a pessoa paga no pix. As réguas de compras já pagas continuam.
- Aviso fora de ordem é ignorado: se chega um aviso atrasado de uma situação que a venda já deixou (ex.: "pix gerado" depois de "pago"), ele não dispara a automação nem cancela nada.

**Boleto para vencer.** O gateway não avisa que um boleto está para vencer. Por isso, todo dia às 00h01 o sistema verifica os boletos em aberto e inicia a automação para _Vence amanhã_ / _Vence hoje_ / _Vencido_. _Vencido_ é o dia seguinte ao vencimento, sem pagamento (_"os que venceram ontem e ainda não foram pagos"_).

Para a mensagem não chegar de madrugada, ligue a saída do evento a um bloco Espera com "Aguardar tempo" e, depois, à mensagem. Em "Quanto tempo aguardar?", use "Outro…" (8 horas, por exemplo, envia por volta das 8h).

**Carrinho abandonado.** Quando alguém sai do checkout sem comprar, o gateway avisa e a automação começa para essa pessoa.

- Precisa estar ligado no gateway: _"O gateway só avisa o carrinho abandonado se o evento de abandono de checkout estiver marcado no postback dele."_ O postback é o aviso automático que o gateway envia à Convergefy. Na Payt, o evento se chama "Abandono de Checkout".
- Precisa de telefone: sem telefone utilizável no checkout, ou em venda de teste, nada é iniciado.
- Vira contato: quem abandonou e ainda não era contato passa a ser, para a mensagem poder sair. Automações de "Contato criado" também rodam para essa pessoa.
- Uma vez por carrinho: o mesmo carrinho abandonado de novo não recomeça a automação. Se a pessoa abandonar outro carrinho, a automação do anterior para e começa a do novo.
- Para quando a pessoa compra: qualquer compra nova dela no mesmo gateway, paga ou não, encerra a automação de carrinho abandonado. Um aviso de abandono que chega depois de ela comprar não inicia nada.
- Dê tempo antes da mensagem: _"A pessoa pode voltar e comprar logo depois. Um bloco Espera antes da mensagem dá esse tempo: se ela comprar no meio, a mensagem não sai."_

Com este gatilho, as mensagens ganham as variáveis do grupo "Dados da compra" (veja _Variáveis_ em [Ações, espera e decisões](https://docs.convergefy.com.br/kb/automacoes-acoes.md)).
