# SuperApp

SuperApp é uma aplicação React Native que contém vários MiniApps. Este repositório utiliza a arquitetura de Monorepo para gerenciar esses MiniApps.

## Estrutura e Arquitetura

Este SuperApp é estruturado como um Monorepo, o que significa que todos os MiniApps são mantidos em um único repositório Git, mas são projetados para funcionar de forma independente. Este projeto utiliza Nome do gerenciador de pacotes, como Lerna, Yarn Workspaces, NX Monorepo ou outro para gerenciar o Monorepo.

A estrutura do repositório é a seguinte (Apenas ilustrativa):

```bash
.
├── packages/
│   ├── Core/
│   ├── MiniApp1/
│   ├── MiniApp2/
│   ├── MiniApp3/
│   └── ...
│   ├── shared-components/
│   ├── shared-logic/
│   └── ...
```

Exemplo:
Cada MiniApp reside dentro da pasta `packages/`. Eles são independentes e podem ser executados separadamente, mas também podem compartilhar componentes e lógicas, que estão presentes em `shared-components/` e `shared-logic/`, respectivamente.

## Como executar

Dependendo do gerenciador de pacotes que você está utilizando, os comandos para instalar as dependências e executar o SuperApp podem variar. Aqui estão os comandos de exemplo usandos neste projeto:

```bash
# Instalar as dependências (na raiz do projeto)
# comando para instalar as dependências

yarn install

# Executar o SuperApp (Core)
# comando para executar o SuperApp
# Você também pode executar MiniApps individualmente:

yarn workspace @superapp/core start

# Executar o MiniApp1
# comando para executar o MiniApp1 (ex: apphome)

yarn workspace @superapp/apphome start


```

## Contato

William Robson Mendonça

williamrmendonca@icloud.com

