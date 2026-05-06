# Referência Técnica para Skills

Este guia serve como consulta rápida para garantir a consistência entre todas as skills do repositório.

## 1. Padrões de Nomeação
- **Formato:** `lowercase-kebab-case`
- **Estilo:** Use gerúndios para descrever a ação.
- **Exemplos:**
    - ✅ `refatorando-codigo`
    - ✅ `gerando-documentacao`
    - ❌ `RefactorCode` (CamelCase)
    - ❌ `ajuda_com_docs` (snake_case)

## 2. Estrutura de Metadados (Frontmatter)
Todo `SKILL.md` deve começar com:
```markdown
---
name: nome-da-skill
description: Descrição curta em 3ª pessoa.
type: categoria-da-skill
---
```

## 3. Hierarquia de Arquivos (Monorepo)
Siga a estrutura de "Divulgação Progressiva":

- **`SKILL.md`**: O ponto de entrada. Contém o "O QUÊ" e o "COMO" básico.
- **`REFERENCE.md`**: Contém o "DETALHE". Documentação técnica, tabelas de comandos, regras de sintaxe.
- **`EXAMPLES.md`**: Contém o "EXEMPLO". Casos de uso reais e comparativos "Certo vs Errado".

## 4. Checklist de Qualidade (QA)
| Item | Critério |
| :--- | :--- |
| Descrição | Terceira pessoa, sem "Eu" ou "Você". |
| Tamanho | `SKILL.md` < 500 linhas. |
| Dependências | Caminhos de arquivos explicitamente definidos. |
| Testes | Pelo menos 3 cenários de teste validados. |
