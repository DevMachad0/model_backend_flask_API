# Regras do projeto

## Consulta obrigatória

Todos os modelos LLM e assistentes de IA devem consultar esta pasta e ler suas
instruções antes de qualquer ação no projeto, incluindo análise, planejamento,
execução de comandos e alterações de arquivos. Não inicie o trabalho sem essa
leitura, independentemente do modelo, fornecedor ou ferramenta utilizada.

## Commits em português do Brasil

Todas as mensagens de commit devem ser escritas em português do Brasil (pt-BR),
incluindo título e descrição, quando houver. Essa regra vale para todos os
repositórios do projeto e para alterações em quaisquer arquivos, sem exceção.
Nomes técnicos, identificadores e caminhos podem manter sua grafia original.

Exemplo: `Adiciona validação de credenciais na autenticação`.

## Simplicidade do código

- Utilize código simples, legível e direto.
- Evite sintaxes complexas e abstrações desnecessárias.
- Mantenha os arquivos pequenos e com responsabilidades bem definidas.
- Divida arquivos que estiverem crescendo em módulos menores e coesos.
- Evite concentrar responsabilidades diferentes no mesmo arquivo.

## Organização do sistema

O código da aplicação fica em `app/src/`. As três pastas principais são
`routes`, `models` e `services`. A pasta `auth` organiza a área de segurança.

### routes

Contém apenas as rotas e suas configurações. As rotas devem encaminhar o
processamento para os serviços ou para os módulos de autenticação adequados.
Não concentre regras de negócio ou modelagem de banco de dados nesta pasta.

### models

Contém a modelagem do banco de dados: definição e criação dos modelos, campos,
relacionamentos, restrições e demais componentes relacionados à estrutura dos
dados. Mantenha as definições organizadas por responsabilidade.

### services

Contém os serviços, as funções e as regras de negócio relacionados ao projeto.
Pode conter serviços simples ou mais complexos, mantendo funções claras e
módulos pequenos. As rotas devem utilizar esses serviços quando necessário.

### auth

Contém todos os processos relacionados à autenticação e à segurança, incluindo
criptografia, tratamento de credenciais, autorização e demais mecanismos de
proteção. Centralize nesta pasta a lógica de segurança do projeto. As declarações
e configurações das rotas de autenticação permanecem em `routes`, utilizando
os processos definidos em `auth`.

## Documentação de funções e utilidades

A pasta de documentação na raiz, atualmente chamada `docs/`, serve para
documentar funções e utilidades do sistema. Explique principalmente o que cada
rota e processo faz, com descrições objetivas de sua finalidade, entradas,
saídas e comportamento, quando aplicável.

Mantenha essa documentação específica em arquivos próprios, sem concentrá-la
na documentação geral do projeto. Ao criar ou alterar uma função, rota,
processo ou utilidade, mantenha sua documentação correspondente atualizada.

Utilize nomes descritivos para os arquivos, como `rotas.md`, `autenticacao.md`
ou `utilidades.md`. Não utilize `README.md` para as regras da pasta `prompt`
nem para essa documentação de utilidades. Reserve esse nome para a
apresentação geral do repositório.

