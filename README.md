# Estrutura padrão para backend Python com Flask

Repositório base para iniciar projetos de backend em Python com Flask. Oferece
uma estrutura de pastas e convenções para manter o código simples, organizado
e fácil de manter.

A organização foi pensada para o desenvolvimento assistido por inteligência
artificial. A separação de responsabilidades e as instruções centralizadas
ajudam a reduzir erros, manter consistência e orientar as alterações no código.

## Estrutura

| Caminho | Finalidade |
| --- | --- |
| `app/src/routes/` | Rotas e suas configurações. |
| `app/src/models/` | Modelagem e estrutura do banco de dados. |
| `app/src/services/` | Serviços, funções e regras de negócio. |
| `app/src/auth/` | Autenticação e processos de segurança. |
| `app/prompt/` | Regras e orientações para o desenvolvimento. |
| `docs/` | Documentação específica de funções, rotas, processos e utilidades. |
| `AGENTS.md` | Instruções de entrada para assistentes de IA. |

## Como utilizar

Use este repositório como ponto de partida para novos backends com Flask e
adicione as funcionalidades conforme as necessidades de cada projeto.

Antes de iniciar qualquer trabalho, consulte as
[regras do projeto](app/prompt/regras.md). Essa leitura é obrigatória para
assistentes de IA. Mantenha os arquivos pequenos, respeite as responsabilidades
de cada pasta e escreva todas as mensagens de commit em português do Brasil.
