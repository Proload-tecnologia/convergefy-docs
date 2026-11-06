# Cobrança

A Convergefy é um serviço por assinatura. Aqui você entende onde ver a situação da assinatura da empresa e como assinar, trocar de plano, atualizar o cartão ou cancelar, tudo por um portal seguro da Stripe.

Na Central de Ajuda: https://docs.convergefy.com.br/#/cobranca

## Em resumo

A Convergefy é um serviço contínuo (servidores, WhatsApp, suporte) e funciona por **assinatura**: enquanto a assinatura está em dia, sua empresa fica ativa e com acesso. Sem ela, o acesso é bloqueado.

Assinar, trocar de plano, cadastrar o cartão ou cancelar é feito em um portal seguro hospedado pela Stripe (a empresa de pagamentos). A Convergefy nunca vê nem guarda o número do seu cartão. Planos e valores vigentes ficam no site da Convergefy e no próprio portal.

### Algo deu errado?

Procure o que você está vendo e siga a coluna da direita. O detalhe de cada caso está mais abaixo.

| O que você vê                                                           | O que fazer                                                                                                                                                       |
| ----------------------------------------------------------------------- | ----------------------------------------------------------------------------------------------------------------------------------------------------------------- |
| Tela "Assinatura indisponível" com o selo "Expirada"                    | A empresa está bloqueada até assinar. O Administrador clica em "Gerenciar assinatura" e assina. Quem não é Administrador pede a ele.                              |
| Aviso "Faltam X dias para o fim do período de experiência."             | Ainda há tempo. Quando chegar o dia, assine para não perder o acesso.                                                                                             |
| Aviso "Seu período de experiência acaba hoje."                          | É o último dia. Assine para não perder o acesso.                                                                                                                  |
| Mais de 15 dias sem assinatura ativa                                    | As conexões do WhatsApp Web foram desligadas. Depois que a assinatura voltar, reconecte pelo QR Code (ver [Conexões](https://docs.convergefy.com.br/kb/conexoes.md)). |
| Medo de ser cobrado no período de experiência                           | A data de "Próxima renovação" é quando a primeira cobrança aconteceria, se você não cancelar antes.                                                               |
| O botão "Gerenciar assinatura" não aparece                              | Ele só aparece para o Administrador, com assinatura pela Stripe e status Ativo. Com a assinatura encerrada, use a tela de bloqueio.                               |
| Você clicou em "Gerenciar assinatura" e nada abriu                      | O portal abre numa aba nova. O navegador pode estar bloqueando pop-ups: libere para o endereço da Convergefy e clique de novo.                                    |
| "Não foi possível abrir o portal de pagamento."                         | Clique em "Gerenciar assinatura" de novo. Se persistir, recarregue a página.                                                                                      |
| "Esta empresa ainda não tem cadastro de pagamento. Fale com o suporte." | Fale com o suporte da Convergefy (WhatsApp ou e-mail do rodapé desta página).                                                                                     |

Você gerencia tudo em Configurações → Organização → Dados da empresa → Informações do plano. É uma área exclusiva do **Administrador** da empresa: nenhum nível de acesso da aba "Acesso" dos membros libera esta tela nem o botão "Gerenciar assinatura" (ver [Equipe e permissões](https://docs.convergefy.com.br/kb/equipe-permissoes.md)). Quem não é Administrador não vê o item no menu.

**Conceitos rápidos**

- **Assinatura** — O plano que mantém a empresa ativa. A Convergefy é um serviço contínuo, então o acesso depende de uma assinatura em dia; sem ela, a empresa fica bloqueada.
- **Período de experiência** — Quando a empresa está nele, a assinatura já aparece como ativa e a primeira cobrança fica marcada para o fim do período. A tela "Dados da empresa" mostra quanto falta (ver abaixo).
- **Portal de pagamento (Stripe)** — A tela segura, hospedada pela própria Stripe, onde você assina, troca de plano, cadastra/atualiza o cartão ou cancela. Como é da Stripe, o número do cartão fica com a empresa de pagamentos; a Convergefy nunca o vê.
- **Renovação** — A data da próxima cobrança, conforme a periodicidade do plano escolhido.

## Quando o acesso é bloqueado

A única tela de cobrança da própria plataforma é a de bloqueio. Ela aparece quando o período de experiência ou a assinatura termina sem um plano ativo:

- **Assinatura indisponível (Expirada)** (red) — A tela mostra o selo "Expirada", o título "Assinatura indisponível" e o texto _"A empresa {nome} não tem acesso ao Convergefy neste momento. O período de experimentação ou a assinatura da sua empresa terminou."_ A empresa fica bloqueada até assinar. Como resolver: clique em “Gerenciar assinatura” e assine para liberar. Quem não é Administrador deve pedir a ele.

O botão "Gerenciar assinatura" (mostra _"Abrindo..."_ enquanto carrega) só aparece para o Administrador. Os demais membros leem, no fim do texto, _"peça ao administrador da empresa para renovar a assinatura."_

> **Depois de 15 dias sem assinatura, o WhatsApp Web desliga**
>
> Se a empresa passar de 15 dias sem assinatura ativa, as conexões do WhatsApp Web são desligadas. Depois que a assinatura voltar, é preciso reconectá-las pelo QR Code (ver [Conexões](https://docs.convergefy.com.br/kb/conexoes.md)).

Todo o pagamento acontece dentro do portal da Stripe: você sai dele de volta para a mesma tela em que estava, sem passar por nenhuma tela de confirmação da Convergefy.

## Informações do plano e de pagamento

Em "Dados da empresa", dois cartões mostram o estado real da assinatura. Os dados vêm direto da Stripe e se atualizam sozinhos depois que você mexe no portal. O cartão "Informações de pagamento" só existe se a empresa já tem cadastro de pagamento na Stripe.

- **Informações do plano** — Mostra o Plano (o nome do plano contratado) e o Status (Ativo em verde ou Encerrado). Os demais campos só aparecem quando existem: Próxima renovação (data) e Valor do plano. Se a assinatura tiver uma segunda data, aparece outra Próxima renovação (assinatura ativa) ou Encerrado em (assinatura encerrada).
- **Limite de membros** — Vagas usadas / total do plano (ex.: _1 / 3_); sem limite no plano, aparece só "Membros" e a quantidade. Como as vagas são contadas e o que fazer quando acabam: [Limite de vagas do plano](https://docs.convergefy.com.br/kb/equipe-permissoes.md). Para subir de plano, use o portal.
- **Gerenciar assinatura** — O botão "Gerenciar assinatura" fica no fim do cartão do plano. Só aparece para o Administrador, com assinatura pela Stripe e status Ativo. Com a assinatura encerrada, ele não aparece aqui (use a tela de bloqueio, acima).
- **Informações de pagamento** — Mostra Email, Telefone, Cartão (ex.: _Visa •••• 4242_ ou _"Não informado"_) e Validade (ex.: _12/2034_, só quando há cartão). Se a Stripe tiver o documento do cliente, aparece também CNPJ ou CPF.

### Aviso de período de experiência

Quando a empresa está em período de experiência, "Dados da empresa" mostra o aviso "Período de experiência" (_"A sua empresa está em modo de experiência."_) com a contagem regressiva:

- **Faltam X dias** (amber) — _"Faltam X dias para o fim do período de experiência."_ (no singular, _"Faltam 1 dia para o fim do período de experiência."_). Ainda há tempo.
- **Acaba hoje** (amber) — _"Seu período de experiência acaba hoje."_ É o último dia; assine para não perder o acesso.

Nesse período a assinatura já aparece como "Ativo" e o plano mostra a data da primeira renovação: é quando a primeira cobrança aconteceria, **se** você não cancelar antes. Sem cartão cadastrado, o campo Cartão mostra _"Não informado"_.

Na tela de escolher empresa, a situação aparece mais curta, como um selo ao lado do nome, sem a contagem de dias:

- Ativo: assinatura em dia.
- Trial: ainda no período de experiência.
- Expirado: assinatura encerrada.
- Inativo: os demais casos.

## Gerenciar a assinatura

O botão "Gerenciar assinatura" (em "Dados da empresa") abre o portal da Stripe em outra aba, uma página segura hospedada pela própria Stripe, onde fica tudo da assinatura.

1. **Abrir o portal** — Clique em **"Gerenciar assinatura"**. Enquanto carrega, o botão mostra _"Abrindo..."_. A página da Stripe abre numa nova aba (título _"Assinatura e Pagamento"_, com um link de retorno para a Convergefy num canto; o texto exato desse link varia).
2. **Fazer o que precisar** — No portal você assina, troca de plano, adiciona/atualiza o cartão, edita os dados de cobrança ou cancela (veja os blocos abaixo).
3. **Voltar para a Convergefy** — Use o link de retorno no canto da página. As mudanças que você fez (cartão, plano) refletem sozinhas em "Dados da empresa", sem precisar recarregar nada à mão.

Com a assinatura ativa, o serviço renova sozinho na data de renovação. O cancelamento também é feito no portal e vale até o fim do período já pago: você continua com acesso até lá.

> **Se o portal não abrir e nada acontecer**
>
> O portal abre numa aba nova. Se o navegador estiver bloqueando pop-ups desta página, a aba simplesmente não abre e nenhuma mensagem aparece: libere os pop-ups para o endereço da Convergefy e clique de novo.

**O que dá para fazer no portal da Stripe**

O portal reúne quatro blocos:

- **Assinatura atual** — Mostra o plano, o valor e a periodicidade. No período de experiência, exibe ainda o aviso _"Free trial ends …"_ e _"Depois que seu teste grátis terminar em {data}, este serviço continua automaticamente."_ Botões: "Atualizar assinatura" (trocar de plano) e "Cancelar assinatura".
- **Forma de pagamento** — Mostra _"Sem forma de pagamento"_ quando ainda não há cartão. "Adicionar forma de pagamento" abre o formulário (número do cartão, validade MM/AA, código de segurança, país). O cartão salvo aparece como _Visa •••• 4242 · Expira 12/2034_ com o selo Padrão.
- **Informações de cobrança** — Nome, e-mail e telefone. "Atualizar informações" abre a edição.
- **Histórico de faturas** — A lista de cobranças, com valor, situação (ex.: Pago) e a descrição de cada uma.

Ao adicionar ou atualizar o cartão no portal, a Convergefy reflete a mudança sozinha em "Dados da empresa" → "Informações de pagamento": o campo Cartão passa a mostrar a bandeira e os 4 últimos dígitos.

## Erros esperados

- “Não foi possível abrir o portal de pagamento.” — falha ao abrir o portal da Stripe. Resolver: tente clicar em “Gerenciar assinatura” de novo; se persistir, recarregue a página.
- “Esta empresa ainda não tem cadastro de pagamento. Fale com o suporte.” — a empresa ainda não tem cadastro de cliente na Stripe, então não há portal para abrir. Resolver: fale com o suporte da Convergefy (WhatsApp ou e-mail do rodapé desta página).
