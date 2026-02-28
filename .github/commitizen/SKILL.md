---
name: commitizen
description: Guia de boas práticas para criação de commits seguindo padrões padronizados.
license: MIT
metadata:
  author: heliojff
  version: "1.0"
---

# Commitizen – Boas Práticas de Commits

Esta skill orienta como escrever commits claros, padronizados e úteis.

## Objetivos
- Ensinar padrões de commit consistentes.
- Facilitar rastreabilidade e histórico limpo.
- Padronizar contribuições entre equipes.

## Estrutura de um Commit
```
tipo: descrição

[corpo opcional]

[rodapé opcional]
```

## Tipos Comuns
- feat: Adição de uma nova funcionalidade ao código.
- fix: Correção de um bug ou erro.
- docs: Alterações apenas na documentação (README, comentários).
- style: Mudanças de formatação, espaços, ponto e vírgula, que não afetam o significado do código.
- refactor: Melhoria no código que não altera funcionalidade nem corrige bug.
- perf: Alteração de código para melhoria de desempenho.
- test: Adição ou correção de testes existentes.
- chore: Atualizações de tarefas de build, pacotes, ou ferramentas de desenvolvimento (não altera produção).
- build: Alterações no sistema de build ou dependências externas.
- ci: Mudanças em arquivos/scripts de CI (Continuous Integration).
- revert: Reversão para um commit anterior. 

## Boas Práticas
- Usar verbo no imperativo.
- Título curto e objetivo.
- Commits pequenos e focados.
- Explicar o motivo no corpo quando útil.
- Referenciar issues.

## Exemplos
```
feat: adiciona validação de CPF
```
```
fix: corrige erro no login

O problema ocorria ao validar token expirado.
```

## Erros Comuns
- Títulos vagos.
- Commits grandes demais.
- Misturar alterações sem relação.
