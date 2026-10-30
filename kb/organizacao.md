# Dados da empresa

A tela Dados da empresa reúne as informações do seu negócio na Convergefy e os detalhes da assinatura — plano, período de experiência grátis e pagamento. É onde você renomeia a empresa, vê quanto falta do teste e abre o portal para mexer no cartão ou no plano.

Na Central de Ajuda: https://docs.convergefy.com.br/#/organizacao

## Em resumo

Toda empresa na Convergefy é um **espaço de trabalho** próprio. Esta tela, _"Gerencie os dados da sua empresa e detalhes da assinatura."_, é a ficha desse espaço: o nome que aparece para os atendentes, o plano que mantém tudo ativo e os dados de pagamento que vêm do cartão cadastrado.

É uma área de Administrador: o item "Dados da empresa" só aparece no menu para quem é Administrador. No acesso direto pelo endereço, quem não é vê "Você não tem acesso a esta área" (_"O acesso de cada membro é definido pelo administrador da empresa. Fale com ele se você precisar entrar aqui."_). Ajustar a assinatura (trocar plano, cartão ou cancelar) só faz sentido aqui. Para o Administrador, Configurações abre direto nesta tela; para os demais membros, abre em Membros.

### Algo deu errado?

Procure o que você está vendo e siga a coluna da direita. O detalhe de cada caso está mais abaixo.

| O que você vê                                                               | O que fazer                                                                                                                                                                             |
| --------------------------------------------------------------------------- | --------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------- |
| "Não foi possível abrir o portal de pagamento."                             | Aguarde alguns segundos e clique em "Gerenciar assinatura" de novo. Se persistir, recarregue a página e confira se o navegador não está bloqueando a abertura de novas abas ou pop-ups. |
| "Esta empresa ainda não tem cadastro de pagamento. Fale com o suporte."     | Fale com o suporte para que o cadastro de pagamento da empresa seja criado. Depois, tente abrir o portal de novo.                                                                       |
| Aviso "Período de experiência" com "Seu período de experiência acaba hoje." | Último dia. Assine hoje para continuar sem interrupção (ver [Cobrança](https://docs.convergefy.com.br/kb/cobranca.md)).                                                                     |
| Não dá para convidar mais ninguém                                           | O limite de membros foi atingido. Revogue um convite, remova um membro ou suba de plano (ver [Equipe e permissões](https://docs.convergefy.com.br/kb/equipe-permissoes.md)).                |
| "Não informado" no cartão                                                   | Ainda não há cartão cadastrado, por exemplo durante o período de experiência.                                                                                                           |

**Conceitos rápidos**

- **Empresa / Organização** — O espaço de trabalho do seu negócio dentro da Convergefy. Cada empresa tem seus próprios contatos, conexões e equipe.
- **Assinatura** — O plano pago que mantém a empresa ativa. Sem assinatura ativa (depois do teste), o acesso fica em risco.
- **Período de experiência (trial)** — Período em que a empresa criada junto com o seu cadastro já usa a plataforma antes da primeira cobrança da assinatura.

## Como chegar

Barra lateral → Configurações → seção ORGANIZAÇÃO → "Dados da empresa". Quem é Administrador cai aqui ao abrir Configurações.

## Renomear a empresa

O nome fica no topo da tela e é editável no próprio lugar. Não há botão de "salvar" separado.

1. **Clicar no nome** — Clique sobre o nome da empresa (o campo mostra _"Nome da empresa"_).
2. **Digitar o novo nome** — Apague e digite o nome que quiser.
3. **Confirmar ou cancelar** — **Clique fora do campo** (ou pressione Tab) para salvar. Para desistir sem mudar nada, pressione **Esc**.

## Período de experiência

A empresa criada junto com o seu cadastro pode começar num **período de experiência** (quem se cadastra pela primeira vez com um login social também). Enquanto ele vale, a tela mostra o aviso "Período de experiência" (_"A sua empresa está em modo de experiência."_) junto com a contagem regressiva.

- **Faltam X dias para o fim do período de experiência.** — Ainda há tempo. Você pode usar tudo normalmente; assine antes do fim para não perder o acesso (ver [Cobrança](https://docs.convergefy.com.br/kb/cobranca.md)).
- **Seu período de experiência acaba hoje.** — Último dia. Assine hoje para continuar sem interrupção.

> **Por que esse aviso existe**
>
> Ele aparece com antecedência justamente para você não ser pego de surpresa quando o teste terminar. Os detalhes de planos e pagamento ficam em [Cobrança](https://docs.convergefy.com.br/kb/cobranca.md).

**Quem não ganha período de experiência e como a empresa nasce**

Algumas situações não ganham período de experiência: uma empresa adicional, criada depois por quem já tem conta, e quem entra por convite (essa pessoa entra na empresa de quem convidou, não cria uma nova).

Se você não informar o nome, a empresa nasce como "Empresa de {nome}". Como o nome de quem se cadastra vem da parte do e-mail antes do `@`, pode ficar algo como _"Empresa de joao.silva"_; renomeie logo acima. Toda empresa nova também já vem com um departamento chamado "Atendimento", com quem a criou dentro (ver [Tags e Departamentos](https://docs.convergefy.com.br/kb/tags-departamentos.md)).

## Informações do plano

Esse bloco resume sua assinatura. Alguns campos só aparecem quando a informação existe (a data de renovação, o valor do plano); quando falta o dado, a tela mostra "Não informado".

- **Plano** — Básico, Premium ou Business. Empresas com contrato fora do fluxo padrão de assinatura mostram "Não informado".
- **Status** — Ativo (em verde) enquanto a assinatura está em dia, ou Encerrado se ela terminou.
- **Próxima renovação** — A data da próxima cobrança. Se a assinatura já terminou, aparece como "Encerrado em" + a data.
- **Valor do plano** — Quanto você paga por ciclo (ex.: R$ 197,00). Só aparece quando o valor é conhecido.
- **Limite de membros** — Vagas usadas / total do plano (ex.: 1 / 3); sem limite no plano, aparece só "Membros" e a quantidade. Como as vagas são contadas e o que fazer quando acabam: [Limite de vagas do plano](https://docs.convergefy.com.br/kb/equipe-permissoes.md).

**Botão “Gerenciar assinatura”**

Aparece só para o Administrador e só quando a empresa tem uma assinatura ativa com pagamento pelo portal. Abre o **portal de pagamento** (Stripe) em outra aba do navegador. É lá que você troca de plano, atualiza o cartão ou cancela a assinatura. Enquanto a aba carrega, o botão mostra _"Abrindo..."_.

Como assinar, trocar de plano, pagar e o que acontece quando o pagamento atrasa estão em [Cobrança](https://docs.convergefy.com.br/kb/cobranca.md).

## Informações de pagamento

Mostra para onde vão as cobranças e qual cartão está cadastrado. O bloco só aparece depois que a empresa tem um cadastro de pagamento; antes disso, a seção inteira não é exibida.

- **Email · Telefone · CNPJ ou CPF** — Os dados de cobrança da empresa. O rótulo do documento muda entre CNPJ e CPF conforme o que foi cadastrado, e só aparece se houver documento.
- **Cartão** — A bandeira + os 4 últimos dígitos (ex.: Visa •••• 4242). Antes de cadastrar um cartão (por exemplo, durante o período de experiência), mostra "Não informado".
- **Validade** — Mês/ano do cartão (ex.: 12/2034).

> **Esses dados se atualizam sozinhos**
>
> O cartão, a validade e os dados de cobrança vêm do portal de pagamento e se atualizam automaticamente depois que você cadastra ou troca o cartão por lá. Você não digita o número do cartão dentro da Convergefy.

## Erros e avisos esperados

- “Não foi possível abrir o portal de pagamento.” — a Convergefy não conseguiu abrir o portal de pagamento (Stripe) em outra aba. Resolver: aguarde alguns segundos e clique em “Gerenciar assinatura” de novo; se persistir, recarregue a página. Confira também se o navegador não está bloqueando a abertura de novas abas/pop-ups.
- “Esta empresa ainda não tem cadastro de pagamento. Fale com o suporte.” — a empresa ainda não tem cadastro no portal de pagamento, então não há o que abrir. Resolver: fale com o suporte para que o cadastro de pagamento da empresa seja criado; depois, tente abrir o portal de novo.
