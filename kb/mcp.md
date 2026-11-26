# Conectar uma IA (MCP)

Como ligar o Claude, o Codex, o Gemini ou outra IA aos seus dados na Convergefy para fazer perguntas sobre contatos, negócios, conversas e campanhas. Só leitura.

Na Central de Ajuda: https://docs.convergefy.com.br/#/mcp

## Em resumo

MCP é um padrão aberto que deixa uma IA consultar outro sistema. Com ele, você pergunta à sua IA, por exemplo, _"quantos negócios ganhei este mês?"_, e ela busca a resposta na Convergefy.

- **Só leitura.** A IA consulta, mas não cria, altera nem exclui nada.
- **Com o seu acesso.** A IA vê só o que você vê no sistema, com as permissões que você tem em cada empresa.
- **Por pessoa.** Cada membro conecta a própria IA. A conexão é sua e vale em todas as suas empresas.

> **O que a IA consultar fica com ela**
>
> O que a IA consultar fica guardado no histórico dela, no provedor que você usa (por exemplo, o Claude). Ao criar um token, a janela lembra disso. No modo Login não há aviso, mas vale o mesmo. Conecte só uma IA em que você confia para guardar dados dos seus clientes.

### Algo deu errado?

| O que você vê                                               | O que fazer                                                                                                                      |
| ----------------------------------------------------------- | -------------------------------------------------------------------------------------------------------------------------------- |
| A IA diz que a assinatura não está ativa                    | A assinatura da empresa está vencida. Regularize em Configurações para voltar a consultar.                                       |
| A IA não encontra dados do Rastreamento                     | Essas consultas pedem o nível Ver no Rastreamento. Veja quantas consultas você pode usar em **"Ver o que a IA pode consultar"**. |
| A sua conta do Claude não mostra "Cabeçalhos de requisição" | Use o modo **Login**.                                                                                                            |
| A IA pede para entrar de novo                               | Passou muito tempo sem uso. Entre com a sua conta da Convergefy e clique em **"Permitir"**.                                      |
| Um token parou de funcionar                                 | Ele venceu (vale 1 ano) ou foi revogado. Crie outro.                                                                             |

## Conectar a sua IA

A tela fica em **Configurações → MCP** (grupo "Integrações") e também em **Minha conta → MCP**. Cada empresa tem um endereço próprio. Em Configurações → MCP, vale a empresa em que você está. Em Minha conta → MCP, quem tem mais de uma empresa escolhe primeiro para qual vai conectar. Empresa com assinatura inativa aparece desligada, com _"Assinatura inativa"_.

1. **Escolher como conectar** — Em "Escolha como conectar":

   - **Login** (_"Recomendado"_): _"A IA abre a tela do Convergefy, você entra e permite. Sem token para guardar."_
   - **Token**: _"Você cria um token e cola na IA, sem entrar pelo navegador."_ No modo Token, aparece o passo "Crie um token de MCP".
2. **Seguir o passo a passo da sua IA** — Em "Adicione na sua IA", escolha a aba da sua IA: **Claude**, **Claude Code**, **Codex** ou **Gemini CLI**. Cada aba traz os passos e o endereço para copiar.
3. **Permitir o acesso** — No modo Login, a IA abre a tela de autorização da Convergefy. Entre com a sua conta e clique em **"Permitir"**. A IA passa a aparecer em "Conexões".

**Passo a passo no Claude (modo Login)**

1. No Claude, pelo site ou pelo app do computador, abra Personalizar > Conectores.
2. Clique em Adicionar > Adicionar conector personalizado, dê um nome e cole o endereço mostrado na tela.
3. Entre com a sua conta da Convergefy e clique em Permitir. O conector também passa a valer no app do celular.

Nos planos Team e Enterprise do Claude, quem adiciona o conector é o administrador da organização. Depois, cada pessoa clica em Conectar.

**Passo a passo no Claude (modo Token)**

1. Abra Personalizar > Conectores e clique em Adicionar > Adicionar conector personalizado.
2. Dê um nome (por exemplo, Convergefy) e cole o Endereço.
3. Em Autenticação, escolha Sem login.
4. Em Cabeçalhos de requisição, clique em Adicionar cabeçalho. Use o nome `Authorization` e o valor `Bearer SEU_TOKEN`, com o seu token no lugar de SEU\_TOKEN.
5. Clique em Adicionar.

Se a sua conta do Claude não mostrar Cabeçalhos de requisição, conecte com Login. Nos planos Team e Enterprise, o token colado pelo administrador vale para todos os membros: prefira Login, em que cada pessoa entra com a própria conta.

As abas Claude Code, Codex e Gemini CLI trazem o comando pronto para colar no terminal, com o endereço da empresa. No modo Login, cada uma entra de um jeito:

- **Claude Code**: depois do comando, digite `/mcp`, escolha o conector e entre com a sua conta.
- **Codex**: rode o segundo comando da aba (`codex mcp login`), que abre o navegador.
- **Gemini CLI**: a primeira consulta abre o navegador. Se não abrir, use `/mcp auth` seguido do nome do conector.

No modo Token, o Codex não usa comando: a aba mostra o trecho para colar no arquivo `~/.codex/config.toml`.

## Criar um token

No modo Token, clique em **"Criar token de MCP"**:

- **Nome do token** — Um nome para reconhecer o token depois (_"Ex.: Claude Desktop do escritório"_).
- **Não expira** — Desmarcado, o token _"Vale 1 ano a partir de hoje."_ Marcado, _"Funciona até você revogar."_ A tela avisa: _"Se o token vazar, quem tiver ele consegue ler os seus dados até você revogar."_

Clique em **"Criar token"**. Abre "Token criado", com o botão **"Copiar token"**.

> **Copie o token na hora**
>
> _"Copie agora. Por segurança, o token não aparece de novo depois que você fechar esta janela."_ Perdeu o token? Revogue e crie outro. O token vale para todas as suas empresas, então trate-o como uma senha.

## O que a IA pode consultar

Clique em **"Ver o que a IA pode consultar"**. A janela lista as 13 consultas por área e diz quantas você pode usar nesta empresa (_"Você pode usar todas as 13 consultas nesta empresa."_):

- **Contatos** — Buscar contatos, ver um contato e listar tags.
- **Funis e negócios** — Listar funis, buscar negócios e ver as métricas do funil (quantidade e valor por etapa, ganho, perda e desqualificado).
- **Conversas** — Listar conversas e ler uma conversa.
- **Rastreamento** — Resultado por campanha, entrada de contatos e eventos de conversão. Pedem o nível Ver no Rastreamento.
- **Equipe** — Listar membros e departamentos.

Quando falta permissão, a janela mostra quantas consultas estão liberadas e qual acesso falta, por exemplo "Rastreamento: Ver". O acesso é ajustado em [Equipe e permissões](https://docs.convergefy.com.br/kb/equipe-permissoes.md).

## Ver e revogar conexões

Em **"Conexões"** ficam as IAs conectadas, cada uma com o tipo ("Login" ou "Token") e a data: _"Conectado em"_ no Login, e no token _"Criado em"_ com a data em que vence (ou _"não expira"_). Sem nenhuma: _"Nenhuma IA conectada"_.

Para tirar o acesso, clique em **"Revogar"** e confirme em "Revogar acesso?". O efeito é imediato:

- Login: a IA deixa de ler os seus dados na hora. Para usar de novo, conecte outra vez.
- Token: o token para de funcionar na hora, e a IA que usa ele perde o acesso.

**Por quanto tempo o acesso vale**

- Login: a IA renova o acesso sozinha enquanto é usada. Parada por 90 dias, ela pede "Permitir" de novo.
- Token: 1 ano, ou até você revogar se marcou "Não expira".
- A IA pode fazer até 60 consultas por minuto.
- Com a assinatura da empresa inativa, as consultas param até a assinatura ser regularizada.
