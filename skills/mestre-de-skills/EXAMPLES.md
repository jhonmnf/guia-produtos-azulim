# Exemplos de Autoria de Skills

Este arquivo demonstra a diferença entre uma skill mal projetada e uma skill "Mestre".

## Exemplo 1: Descrição da Skill

### ❌ Ruim (Primeira Pessoa / Genérico)
`description: Eu posso te ajudar a revisar seus arquivos Python e sugerir melhorias de performance.`
**Por que é ruim?** Usa a primeira pessoa ("Eu") e é vaga sobre o que realmente faz.

### ✅ Excelente (Terceira Pessoa / Específico)
`description: Analisa a complexidade ciclomática de arquivos Python e sugere refatorações para reduzir o custo computacional.`
**Por que é excelente?** Descrição objetiva, em terceira pessoa, define exatamente a métrica analisada (complexidade ciclomática).

---

## Exemplo 2: Estrutura de Documentação

### ❌ Ruim (Tudo em um único arquivo gigante)
Um único `SKILL.md` com 1.500 linhas contendo instruções, exemplos, tabelas de erros e guias de instalação.
**Problema:** Sobrecarga de contexto. O agente pode ignorar instruções no meio do texto.

### ✅ Excelente (Divulgação Progressiva)
- `SKILL.md` (200 linhas): Fluxo de trabalho e regras principais.
- `REFERENCE.md` (300 linhas): Tabela de flags do comando `grep` e `sed` utilizados.
- `EXAMPLES.md` (150 linhas): Três exemplos de refatoração de loops `for` para `list comprehensions`.
**Vantagem:** O agente carrega apenas o que precisa, economizando tokens e aumentando a precisão.
