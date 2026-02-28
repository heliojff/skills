---
name: criador-skills
description: Guia de melhores práticas para criar skills de alta qualidade seguindo a Agent Skills Specification. Use quando for desenvolver, estruturar ou validar uma nova skill.
license: MIT
metadata:
  author: helio
  version: "1.0"
---

# Criador de Skills – Melhores Práticas

Este guia orienta como criar skills eficientes, robustas e compatíveis com a **Agent Skills Specification**.

## Objetivos da Skill
- Ajudar desenvolvedores a criar skills padronizadas.
- Garantir conformidade com os requisitos obrigatórios do SKILL.md.
- Sugerir estrutura de diretórios organizada.
- Dar exemplos claros de boas práticas.

## Estrutura Recomendada
Uma skill deve conter ao menos:
```
.github/
  └── skill-name/
      └── SKILL.md
```

Estrutura estendida recomendada:
```
skill-name/
  ├── SKILL.md
  ├── scripts/
  ├── references/
  └── assets/
```

## Boas Práticas Essenciais
- **Frontmatter obrigatório**: sempre incluir `name` e `description` válidos.
- **Nome da skill**: apenas minúsculas, números e hífens; deve corresponder ao nome do diretório.
- **Descrição**: detalhar o que a skill faz e quando deve ser utilizada.
- **Tamanho do SKILL.md**: manter abaixo de 500 linhas.
- **Referências separadas**: mover material extenso para `references/`.
- **Scripts autocontidos**: documentar dependências e comportamentos.
- **Progressive Disclosure**: evitar sobrecarregar o contexto.

## Passo a Passo para Criar uma Skill
1. Criar um diretório com nome válido dentro de `.github/`.
2. Criar o arquivo `SKILL.md` com frontmatter completo.
3. Escrever instruções claras no corpo do arquivo.
4. Adicionar exemplos de uso quando útil.
5. (Opcional) Criar scripts auxiliares bem documentados.
6. (Opcional) Adicionar arquivos de referência.
7. Validar a skill usando `skills-ref`.

## Exemplos de Conteúdos Úteis
- Como estruturar tarefas passo a passo.
- Estratégias para lidar com erros comuns.
- Exemplos de entrada e saída.
- Regras ou padrões específicos do domínio.

## Erros Comuns a Evitar
- Nome da skill inválido.
- Descrição vaga ou curta.
- SKILL.md com tamanho excessivo.
- Scripts sem documentação.
- Referências profundas demais.

## Validação
Para validar sua skill:
```
skills-ref validate ./minha-skill
```

Use este guia sempre que iniciar a criação de uma nova skill.