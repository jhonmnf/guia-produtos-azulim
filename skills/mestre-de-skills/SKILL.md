---
name: mestre-de-skills
description: Projeta, documenta e valida skills para Claude Code seguindo as melhores práticas de arquitetura de agentes e monorepos.
type: architectural-guide
---

# Mestre em Criação de Skills

Esta skill transforma o Claude em um arquiteto especialista em extensões para Claude Code. O objetivo é garantir que cada nova skill seja descoberta facilmente, seja concisa e execute tarefas com alta precisão.

## Fluxo de Trabalho Obrigatório

Sempre que for solicitado a criar uma nova skill, siga rigorosamente estas etapas:

### 1. Fase de Design (Discovery)
- Identifique o objetivo central da skill.
- Defina os "Graus de Liberdade": 
    - **Baixa Liberdade:** Para tarefas frágeis (ex: migrações), use scripts exatos.
    - **Alta Liberdade:** Para tarefas criativas (ex: reviews), use diretrizes textuais.
- Mapeie a estrutura de arquivos necessária (SKILL.md, REFERENCE.md, EXAMPLES.md).

### 2. Implementação da Documentação (Authoring)
- **Nomenclatura:** Use `kebab-case` com gerúndios (ex: `analisando-logs`).
- **Descrição:** Escreva estritamente na **terceira pessoa**. Nunca use "Eu posso" ou "Ajudo você". Use "Analisa logs de erro e sugere correções".
- **Divulgação Progressiva:**
    - `SKILL.md`: Instruções de alto nível (< 500 linhas).
    - `REFERENCE.md`: Detalhes técnicos, sintaxes e regras.
    - `EXAMPLES.md`: Casos de uso reais.

### 3. Validação e Testes (Evaluation)
- Crie 3 cenários de teste (Input $\rightarrow$ Comportamento Esperado).
- Simule a execução da skill em uma instância limpa.
- Refine a documentação com base nos erros de interpretação do agente.

## Regras de Ouro de Escrita
- **Proibido:** Explicar conceitos básicos (ex: não explique o que é um arquivo .json).
- **Obrigatório:** Usar caminhos absolutos ou relativos claros para referências de arquivos.
- **Obrigatório:** Manter a documentação DRY (Don't Repeat Yourself), referenciando templates compartilhados se estiver em um monorepo.

## Comando de Saída Esperado
Ao final do projeto de uma skill, entregue:
1. A estrutura de pastas sugerida.
2. O conteúdo completo de cada arquivo `.md`.
3. O comando `mkdir` e `Write` para implementar a skill no sistema do usuário.
