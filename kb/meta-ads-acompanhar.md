# Rastreamento: Acompanhar

Onde conferir o que foi enviado às plataformas de anúncio, o dashboard de resultados e o que fazer quando um envio falha.

Na Central de Ajuda: https://docs.convergefy.com.br/#/meta-ads-acompanhar

## Em resumo

Duas telas mostram o que a Convergefy enviou às plataformas de anúncio: "Eventos" (o histórico de cada conversão enviada) e "Dashboard" (o resumo do período, com todas as plataformas juntas). Ambas só têm dados depois de configurar as contas e o Funil de conversão, em [Configurar](https://docs.convergefy.com.br/kb/meta-ads-configurar.md).

### Algo deu errado?

Procure o que você está vendo e siga a coluna da direita. O detalhe de cada caso está mais abaixo.

| O que você vê                                                                                     | O que fazer                                                                                                                                                                               |
| ------------------------------------------------------------------------------------------------- | ----------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------- |
| "Eventos" vazio                                                                                   | Sem pixel cadastrado, a Convergefy não envia conversão à Meta e nada aparece. A lista só tem envios já tentados. Veja [Configurar](https://docs.convergefy.com.br/kb/meta-ads-configurar.md). |
| Status "Falhou" (vermelho) em um envio                                                            | Abra os detalhes do envio para ver o motivo (HTTP Status e payloads). Confira se o pixel e a conexão com a Meta (ou a conta e a ação do Google) continuam válidos em "Contas de Anúncio". |
| _"Lead sem identificadores enviáveis (sem e-mail, telefone, endereço completo ou click Google)."_ | O contato não tinha nenhum dado para a plataforma casar a conversão. Preencha telefone ou e-mail do contato.                                                                              |
| Um traço (—) no detalhe do envio                                                                  | É dado não registrado. O envio aconteceu normalmente.                                                                                                                                     |
| O Dashboard não mostra envios ou contatos novos                                                   | O painel guarda o resultado por até 15 minutos, então "Atualizar" pode demorar a refletir. Salvar o Funil de conversão atualiza na hora.                                                  |
| Datas desabilitadas no calendário (_"Intervalo máximo de 90 dias."_)                              | Escolha um intervalo de até 90 dias.                                                                                                                                                      |
| Os números do Dashboard não batem com os painéis da Meta ou do Google                             | É esperado. Cada plataforma atribui a conversão com janelas próprias.                                                                                                                     |
| O total no título do painel de contatos é menor que o número clicado                              | É esperado: o painel lista contatos (um por contato, mesmo com mais de um negócio), e o número da etapa conta negócios.                                                                   |
| Uma etapa do "Seu funil" mostra menos do que você enviou                                          | Só contam negócios com evento aceito pela plataforma no período. Envio com status "Falhou" não entra. Veja o status em "Eventos".                                                         |
| "Resumo por Campanha" e "Seu funil" sumiram                                                       | O filtro está em "Outras origens" ou "Não rastreados": não há campanha de anúncio nem conversão a mostrar.                                                                                |
| O card "Seu funil" pede para montar as etapas                                                     | Ainda não há etapa salva. Monte-as em "Funil de conversão" ([Configurar](https://docs.convergefy.com.br/kb/meta-ads-configurar.md)).                               |
| A coluna "Contatos" de uma campanha mudou com o tempo                                             | A origem segue o último clique. Se o contato clicar depois num anúncio de outra campanha, passa a contar nela.                                                                            |
| Erro ao conectar a Meta ou o Google                                                               | Veja "Erros e avisos esperados", no fim desta página.                                                                                                                                     |

## Acompanhar: Eventos

A tela "Eventos" é o histórico de cada conversão enviada, de todas as plataformas. Colunas:

- **Plataforma** — Meta ou Google.
- **Contato** — De quem é a conversão.
- **Destino** — O nome do evento (Meta) ou a ação de conversão (Google).
- **Etapa do Funil** — A coluna do funil em que o negócio entrou e que disparou o envio, com a cor dela (ou _"Etapa inexistente ou excluída"_ se a coluna já não existe).
- **Status** — Enviado ou Falhou.
- **Enviado em** — Data e hora do envio.

Dá para filtrar por texto (contato ou destino), período, plataforma e status ("Enviados", "Falhas"), e abrir os detalhes de cada envio.

**O que significa cada status de envio**

- **Enviado** (green) — A plataforma respondeu OK: a conversão chegou.
- **Falhou** (red) — A plataforma não respondeu OK. Inclui falha de conexão ou de credencial. Como resolver: abra os detalhes do envio para ver o motivo (HTTP Status e payloads); confira se o pixel e a conexão com a Meta (ou a conta e a ação do Google) continuam válidos em Contas de Anúncio.

A lista só tem envios já tentados.

**O que traz o detalhe de um envio**

O painel mostra:

- Contato;
- Negócio (com "Valor", se houver);
- Envio ("Enviado em", "HTTP Status" e o erro, se houver). O "HTTP Status" é o código de resposta da plataforma;
- Origem do anúncio. Na Meta: Campanha, Conjunto, Anúncio e Conta de anúncio, mais o Destino (Pixel e ID do Pixel). No Google: gclid, gbraid e wbraid, mais o Destino (Conta e Ação de conversão).

O bloco "Detalhes técnicos" traz o Transaction ID (o código que identifica o envio) e os payloads (o conteúdo técnico enviado e o recebido) da requisição e da resposta, com o botão **"Copiar JSON"**. São úteis para o suporte.

Um traço (—) significa dado não registrado: contato criado só pelo número, ainda sem nome, ou envio Google antigo, de antes de a Convergefy guardar o nome da conta e da ação. O envio aconteceu normalmente.

No Google, um envio pode falhar com _"Lead sem identificadores enviáveis (sem e-mail, telefone, endereço completo ou click Google)."_ O contato não tinha nenhum dado para a plataforma casar a conversão. Preencha telefone ou e-mail do contato.

## Acompanhar: Dashboard

O Dashboard resume o período escolhido, com todas as plataformas juntas. No topo:

- **Origem** — O filtro "Todas as origens" recorta o painel inteiro por Meta Ads, Google Ads, Outras origens ou Não rastreados.
- **Período** — Presets ("Hoje", "Ontem", "Esta semana", "Última semana", "Este mês", "Último mês") ou um intervalo no calendário, com **"Aplicar"**.
- **Atualizar** — Recarrega os números do período.

> **Limites do período e atualização**
>
> O intervalo vai até 90 dias: as datas além disso ficam desabilitadas no calendário, que avisa ao lado do "Aplicar": _"Intervalo máximo de 90 dias."_ O painel guarda o resultado por até 15 minutos, então "Atualizar" pode demorar a refletir envios e contatos novos. Salvar o Funil de conversão atualiza na hora.

> **Números diferentes dos painéis da Meta e do Google**
>
> Cada plataforma atribui a conversão com janelas próprias: a Meta em dias após o clique, o Google por ação de conversão. Por isso os números do Dashboard podem não bater com os dos painéis delas.

### Origem dos contatos

O bloco "Origem dos contatos" conta os contatos criados no período. À direita fica o total (clique para listar). Abaixo, um tile (quadro) por origem, com número e percentual, clicável:

- **Rastreados** — Subtotal de Meta Ads + Google Ads + Outras origens (_"{X}% do total"_): contatos que a Convergefy conseguiu ligar a alguma origem.
- **Meta Ads** — Vieram de um anúncio do Facebook ou Instagram.
- **Google Ads** — Vieram de um anúncio do Google.
- **Outras origens** — Origem só por UTMs, sem anúncio ligado.
- **Não rastreados** — Sem origem conhecida.

Um gráfico de barras empilhadas mostra os contatos ao longo do período (por dia, ou por hora em intervalos curtos), uma cor por origem. Com filtro de origem, o bloco mostra só aquela.

### Resumo por Campanha

O card "Resumo por Campanha" tem uma aba por plataforma, "Meta Ads" e "Google Ads" (com filtro de origem Meta ou Google, as abas somem). Cada linha é uma campanha:

- "Contatos": contatos cuja campanha de origem é essa, isto é, a do último anúncio clicado. Aparece mesmo sem etapa com evento naquela plataforma. Nesse caso a tabela tem só "Campanha" e "Contatos".
- Colunas de etapa (uma por etapa com evento naquela plataforma): negócios distintos com evento aceito pela plataforma no período, pela campanha do anúncio que gerou o evento. Envio que falhou não conta, e vários pixels não multiplicam: o mesmo negócio vale 1. Descrição na tela: _"Contatos que vieram de cada campanha e, por etapa, os negócios com evento enviado à plataforma."_

Uma campanha pode ter "Contatos" maiores que zero com as etapas zeradas. O que não tem campanha identificada cai em "Sem campanha". No "Total", a coluna "Contatos" é a soma das linhas; nas colunas de etapa, cada negócio conta uma vez, então o total pode ser menor que a soma das campanhas. A coluna "Contatos" e cada célula de etapa são clicáveis e abrem o painel de contatos.

> **A origem segue o último clique**
>
> A campanha de origem é o clique mais recente. Por isso a coluna "Contatos" pode mudar com o tempo: se o contato clicar depois num anúncio de outra campanha, passa a contar nela, inclusive num período já passado.

### Seu funil

O card **"Seu funil"** desenha as etapas que você montou em "Funil de conversão" (veja [Configurar](https://docs.convergefy.com.br/kb/meta-ads-configurar.md)), na mesma ordem:

- no topo, a faixa **"Contatos"** (_"Chegaram no período"_): todos os contatos criados no período, respeitando o filtro de origem;
- abaixo, uma faixa por etapa, com o nome dela e o número;
- entre as faixas, a taxa de avanço, **"% avançam"**. Passe o mouse no percentual para ler _"Dos que chegaram em {A}, quantos chegaram em {B}"_.

> **O que o número de cada etapa conta**
>
> O número de uma etapa é de **negócios distintos** cujo evento foi **aceito pela plataforma** no período.
>
> - Envio que falhou não conta (veja o status em "Eventos").
> - Vários pixels não multiplicam: o mesmo negócio vale 1, mesmo enviado a todos os pixels.
> - Meta e Google para o mesmo negócio também contam 1.
> - Evento sem negócio ligado não entra.
> - A etapa sem evento escolhido aparece com 0.
>
> O "Contatos" do topo é de contatos criados no período. Cada "% avançam" compara uma faixa com a imediatamente anterior.

Sem etapas salvas, o card mostra _"Monte as etapas em Funil de conversão para ver seu funil aqui."_ Ao filtrar por "Outras origens" ou "Não rastreados", o "Resumo por Campanha" e o "Seu funil" somem, porque não há campanha de anúncio nem conversão a mostrar.

No Funil (quadro de vendas), as colunas ligadas a uma etapa com evento mostram um ícone de mira. Detalhes em [Funis e CRM](https://docs.convergefy.com.br/kb/funis.md).

### Contatos por trás de um número

Clicar numa faixa do "Seu funil" (cada uma tem o rótulo "Ver contatos de {nome}"), num tile de origem ou numa célula do resumo abre um painel lateral com os contatos daquele número. O que o painel mostra no topo:

| Clique                            | Título e descrição                                                                                                                                                |
| --------------------------------- | ----------------------------------------------------------------------------------------------------------------------------------------------------------------- |
| Faixa "Contatos"                  | Título _"Contatos"_, com _"Seu funil"_ acima e _"Contatos que chegaram no período."_                                                                              |
| Faixa de uma etapa                | Título com o nome da etapa, com _"Seu funil"_ acima e _"Contatos com negócio em {etapa} no período. Cada contato aparece uma vez, mesmo com mais de um negócio."_ |
| Coluna "Contatos" de uma campanha | _"Campanha · Contatos"_ acima do título                                                                                                                           |
| Célula de etapa de uma campanha   | _"Contatos com negócio em {etapa} por esta campanha no período. Cada contato aparece uma vez, mesmo com mais de um negócio."_                                     |
| Tile de origem                    | A origem, por exemplo _"Contatos · Meta Ads"_                                                                                                                     |

O painel lista **contatos**, um por contato, enquanto o número da etapa conta **negócios**. Por isso o total no título do painel pode ser menor que o número clicado: um contato com dois negócios na mesma etapa aparece uma vez. Dá para buscar por nome ou telefone e filtrar por Departamentos, Atendentes, Status e Tags. Cada contato traz o botão "Conversas" e a origem do anúncio.

## Erros e avisos esperados

- “Login cancelado. Tente novamente.” — Você fechou a janela da Meta antes de terminar. Resolver: clique de novo em “Conectar com Facebook” e conclua o login sem fechar a janela.
- “Conexão cancelada. Você não autorizou o acesso ao Google Ads.” — Você recusou a autorização do Google. Resolver: clique em “Conectar com Google” e autorize o acesso.
- “É preciso conceder todas as permissões solicitadas para conectar.” — Faltou alguma permissão. Resolver: refaça a conexão e marque todas as permissões pedidas pelo Google.
- “A sessão expirou durante a conexão. Tente novamente.” — Demorou demais entre iniciar e concluir o login do Google. Resolver: recomece a conexão com o Google.
- “Não foi possível concluir a conexão com o Google. Tente novamente.” — Falha genérica ao voltar do login do Google. Resolver: refaça a conexão; se persistir, confira se a conta Google tem acesso ao Google Ads e procure o suporte.
- “Não foi possível carregar suas contas do Google Ads.” — A lista de contas de anúncio do Google não carregou. Resolver: use “Tentar de novo”; se persistir, confira se a conta Google conectada tem acesso a contas do Google Ads.
- “Esta conta de anúncio não está mais disponível na sua conexão com o Google.” — A conta escolhida deixou de estar acessível ao login conectado. Resolver: escolha outra conta no seletor ou reconecte o Google.
- “Nenhuma ação de conversão nesta conta. Crie uma no Google Ads.” — A conta Google escolhida não tem ação de conversão para receber os envios. Resolver: crie a ação no Google Ads e volte a escolhê-la em “Enviar como”, no Funil de conversão.
- “Não foi possível carregar o conector da Meta. Um bloqueador de anúncios, extensão de privacidade ou a rede da sua empresa pode estar bloqueando connect.facebook.net.” — O componente de login da Meta não carregou. Resolver: desative o bloqueador ou a extensão nesta página (ou peça liberação de connect.facebook.net na rede) e use “Tentar novamente”.
- “O conector da Meta demorou demais para responder. Verifique sua conexão — ou se a rede bloqueia connect.facebook.net — e tente de novo.” — O mesmo componente demorou demais. Resolver: confira a internet e use “Tentar novamente”.
- “O conector da Meta foi carregado de forma incompleta, provavelmente por uma extensão do navegador. Desative-a nesta página e tente de novo.” — Uma extensão interferiu no carregamento. Resolver: desative extensões de privacidade nesta página e use “Tentar novamente”.
- “A integração com a Meta não está configurada neste ambiente. Fale com o suporte.” — Falta configuração no ambiente. Tentar de novo não adianta. Resolver: não há o que fazer do seu lado: acione o suporte.
- “Não conseguimos abrir a janela da Meta. Verifique se o navegador bloqueou o pop-up desta página e tente de novo.” — O navegador bloqueou a janela de login da Meta. Resolver: libere pop-ups para o endereço da Convergefy e repita a conexão.
- “A Meta não liberou o acesso ao Business. Refaça a conexão e aceite as permissões.” — A Meta não devolveu o acesso ao portfólio empresarial. Resolver: conecte de novo e aceite todas as permissões pedidas pela Meta.
- “Não foi possível concluir a conexão com a Meta.” — Falha ao salvar a conexão depois do login. Resolver: tente conectar de novo; se persistir, procure o suporte.
- “A Meta autorizou o acesso mas não devolveu o código de conexão. Tente de novo; se persistir, fale com o suporte.” — A autorização voltou incompleta. Resolver: repita a conexão; persistindo, acione o suporte.
- “Este Pixel já está cadastrado.” — O ID já foi cadastrado nesta empresa. Resolver: edite o pixel existente em vez de adicionar de novo.
- “Nenhum perfil da Meta conectado à empresa tem acesso a este Pixel.” — Nenhuma conta conectada consegue ver o pixel informado. Resolver: conecte a Meta com um perfil que enxergue o pixel, ou informe um token de acesso próprio.
- “A Meta recusou o token. Confira se ele tem acesso a este Pixel.” — O token informado não tem acesso ao pixel. Resolver: gere um novo token com acesso ao pixel, ou deixe o campo em branco para usar a conexão com a Meta.
- “Não foi possível buscar os pixels na Meta. Tente de novo.” — A lista de pixels que a Meta enxerga não carregou. Resolver: abra “Adicionar pixel” de novo; se persistir, use “Adicionar manualmente”.
- “Dê um nome para a etapa.” — A etapa ficou sem nome. Resolver: digite um nome no campo da etapa antes de salvar.
- “Já existe uma etapa com esse nome.” — Duas etapas do Funil de conversão não podem ter o mesmo nome. Resolver: use um nome diferente. O mesmo vale para “Já existe uma etapa com este nome.”, que vem do servidor.
- “Esta coluna já foi usada em uma etapa.” — Cada coluna só pode estar em uma etapa. Resolver: tire a coluna da outra etapa ou escolha outra coluna em “Onde acontece”.
- “Este evento já foi usado em uma etapa.” — Cada evento da Meta e cada ação do Google só valem em uma etapa. Resolver: tire o evento (ou a ação do Google) da outra etapa ou escolha outro em “Enviar como”.
- “Escolha ao menos uma coluna para enviar este evento.” — A etapa tem evento, mas nenhuma coluna que o dispare. Resolver: adicione um funil e uma coluna em “Onde acontece” na etapa, ou tire o evento.
- “Não foi possível carregar o funil de conversão.” — A tela Funil de conversão não carregou. Resolver: use “Tentar de novo”; se persistir, procure o suporte.
