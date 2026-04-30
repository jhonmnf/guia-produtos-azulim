# Exemplos de Leitura de Sites

Este arquivo demonstra a diferença entre uma extração rasa e uma extração profissional.

## Exemplo 1: Artigo de Blog Técnico

### ❌ Ruim (Extração Bruta)
Um dump de texto que inclui "Login", "Siga-nos no Twitter", "Termos de Uso", misturado com o texto do artigo.
**Problema:** Excesso de ruído (noise) que polui o contexto do agente.

### ✅ Excelente (Extração Limpa)
- **Cabeçalho:** Título do Artigo, Nome do Autor e Data.
- **Conteúdo:** Texto fluido em Markdown, com subtítulos claros e blocos de código formatados.
- **Links:** Referências externas preservadas como `[Nome](URL)`.
- **Rodapé:** Removido completamente.

---

## Exemplo 2: Página de Produto E-commerce

### ❌ Ruim (Lista de Links)
Apenas uma lista de todos os links da página, incluindo "Carrinho", "Minha Conta" e "Produtos Relacionados".
**Problema:** Não identificou a entidade principal (o produto).

### ✅ Excelente (Extração Estruturada)
- **Produto:** Nome do Produto, Preço e Avaliação (Estrelas).
- **Descrição:** Texto detalhado das especificações técnicas.
- **Disponibilidade:** "Em estoque" ou "Esgotado".
- **Imagens:** Lista de URLs das fotos principais do produto.
