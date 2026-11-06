# Rastreamento: Acompanhar

Onde conferir o que foi enviado às plataformas de anúncio, o dashboard de resultados e o que fazer quando um envio falha.

Na Central de Ajuda: https://docs.convergefy.com.br/#/meta-ads-acompanhar

## Em resumo

Duas telas mostram o que a Convergefy enviou às plataformas de anúncio: "Eventos" (o histórico de cada conversão enviada) e "Dashboard" (o resumo do período, com todas as plataformas juntas). Ambas só têm dados depois de configurar as contas e o Funil de Compra, em [Configurar](https://docs.convergefy.com.br/kb/meta-ads-configurar.md).

### Algo deu errado?

Procure o que você está vendo e siga a coluna da direita. O detalhe de cada caso está mais abaixo.

| O que você vê                                                                                     | O que fazer                                                                                                                                                                               |
| ------------------------------------------------------------------------------------------------- | ----------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------- |
| "Eventos" vazio                                                                                   | Sem pixel cadastrado, a Convergefy não envia conversão à Meta e nada aparece. A lista só tem envios já tentados. Veja [Configurar](https://docs.convergefy.com.br/kb/meta-ads-configurar.md). |
| Status "Falhou" (vermelho) em um envio                                                            | Abra os detalhes do envio para ver o motivo (HTTP Status e payloads). Confira se o pixel e a conexão com a Meta (ou a conta e a ação do Google) continuam válidos em "Contas de Anúncio". |
| _"Lead sem identificadores enviáveis (sem e-mail, telefone, endereço completo ou click Google)."_ | O contato não tinha nenhum dado para a plataforma casar a conversão. Preencha telefone ou e-mail do contato.                                                                              |
| Um traço (—) no detalhe do envio                                                                  | É dado não registrado. O envio aconteceu normalmente.                                                                                                                                     |
| O Dashboard não mostra envios ou contatos novos                                                   | O painel guarda o resultado por até 15 minutos, então "Atualizar" pode demorar a refletir. Salvar o mapeamento do Funil de Compra atualiza na hora.                                       |
| O calendário bloqueia as datas (_"Intervalo máximo de 90 dias."_)                                 | Escolha um intervalo de até 90 dias.                                                                                                                                                      |
| Os números do Dashboard não batem com os painéis da Meta ou do Google                             | É esperado. Cada plataforma atribui a conversão com janelas próprias.                                                                                                                     |
| O total no título do painel de contatos é menor que o número clicado                              | É esperado: o total conta contatos distintos, e o número clicado conta eventos.                                                                                                           |
| "Resumo por Campanha" e "Etapas do funil" sumiram                                                 | O filtro está em "Outras origens" ou "Não rastreados": não há campanha de anúncio nem conversão a mostrar.                                                                                |
| A coluna "Contatos" de uma campanha mudou com o tempo                                             | A origem segue o último clique. Se o contato clicar depois num anúncio de outra campanha, passa a contar nela.                                                                            |
| Erro ao conectar a Meta ou o Google                                                               | Veja "Erros e avisos esperados", no fim desta página.                                                                                                                                     |

## Acompanhar: Eventos

A tela "Eventos" é o histórico de cada conversão enviada, de todas as plataformas. Colunas:

- **Plataforma** — Meta ou Google.
- **Contato** — De quem é a conversão.
- **Destino** — O nome do evento (Meta) ou a ação de conversão (Google).
- **Etapa do Funil** — A etapa que disparou o envio (ou _"Etapa inexistente ou excluída"_ se já não existe).
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
> O intervalo vai até 90 dias: mais que isso, o calendário bloqueia as datas (_"Intervalo máximo de 90 dias."_). O painel guarda o resultado por até 15 minutos, então "Atualizar" pode demorar a refletir envios e contatos novos. Salvar o mapeamento do Funil de Compra atualiza na hora.

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

- "Contatos": contatos cuja campanha de origem é essa, isto é, a do último anúncio clicado. Aparece mesmo sem etapa mapeada. Nesse caso a tabela tem só "Campanha" e "Contatos".
- Colunas de evento (uma por etapa mapeada): quantidade de eventos enviados, não de contatos, pois um contato pode gerar vários. Contam envios feitos, inclusive os que falharam (veja o status em "Eventos"). Cada pixel gera um envio: com 2 pixels, cada venda conta 2 vezes.

Uma campanha pode ter "Contatos" maiores que zero com os eventos zerados. O que não tem campanha identificada cai em "Sem campanha". O "Total" soma cada coluna. A coluna "Contatos" e cada célula de evento são clicáveis e abrem o painel de contatos.

> **A origem segue o último clique**
>
> A campanha de origem é o clique mais recente. Por isso a coluna "Contatos" pode mudar com o tempo: se o contato clicar depois num anúncio de outra campanha, passa a contar nela, inclusive num período já passado.

### Etapas do funil

O card "Etapas do funil" desenha um funil com as etapas mapeadas e a quantidade de eventos enviados em cada uma (também contando os que falharam). Passe o mouse para ver o total, a divisão por plataforma e os "Eventos de destino". Clique numa etapa para ver os contatos que enviaram aquela conversão.

Ao filtrar por "Outras origens" ou "Não rastreados", o "Resumo por Campanha" e as "Etapas do funil" somem, porque não há campanha de anúncio nem conversão a mostrar.

### Contatos por trás de um número

Clicar num tile, numa etapa do funil ou numa célula do resumo abre um painel lateral com os contatos daquele número. O título mostra a origem (ex.: "Contatos · Meta Ads"), a etapa ("Etapa · {evento}") ou a campanha ("Campanha · Contatos", "Campanha · {evento}").

O total no título conta contatos distintos e pode ser menor que o número clicado, que conta eventos. Dá para buscar por nome ou telefone e filtrar por Departamentos, Atendentes, Status e Tags. Cada contato traz o botão "Conversas" e a origem do anúncio.

## Erros e avisos esperados

- “Login cancelado. Tente novamente.” — Você fechou a janela da Meta antes de terminar. Resolver: clique de novo em “Conectar com Facebook” e conclua o login sem fechar a janela.
- “Conexão cancelada. Você não autorizou o acesso ao Google Ads.” — Você recusou a autorização do Google. Resolver: clique em “Conectar com Google” e autorize o acesso.
- “É preciso conceder todas as permissões solicitadas para conectar.” — Faltou alguma permissão. Resolver: refaça a conexão e marque todas as permissões pedidas pelo Google.
- “A sessão expirou durante a conexão. Tente novamente.” — Demorou demais entre iniciar e concluir o login do Google. Resolver: recomece a conexão com o Google.
- “Não foi possível concluir a conexão com o Google. Tente novamente.” — Falha genérica ao voltar do login do Google. Resolver: refaça a conexão; se persistir, confira se a conta Google tem acesso ao Google Ads e procure o suporte.
- “Não foi possível carregar suas contas do Google Ads.” — A lista de contas de anúncio do Google não carregou. Resolver: use “Tentar de novo”; se persistir, confira se a conta Google conectada tem acesso a contas do Google Ads.
- “Esta conta de anúncio não está mais disponível na sua conexão com o Google.” — A conta escolhida deixou de estar acessível ao login conectado. Resolver: escolha outra conta no seletor ou reconecte o Google.
- “Nenhuma ação de conversão nesta conta. Crie uma no Google Ads.” — A conta Google escolhida não tem ação de conversão para receber os envios. Resolver: crie a ação no Google Ads e volte a mapear a etapa.
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
