# Exemplos de Geração de PDF

Este arquivo serve como guia para a qualidade esperada dos documentos gerados.

## Exemplo 1: Relatório Técnico (Markdown $\rightarrow$ PDF)

### ❌ Ruim (Sem estrutura visual)
PDF com texto corrido, sem negritos, sem sumário e com quebras de linha cortando palavras ao meio.
**Problema:** Falta de hierarquia visual e erro de renderização de texto.

### ✅ Excelente (Profissional)
- **Capa:** Título centralizado, logo da empresa, data e autor.
- **Sumário:** Lista de seções com numeração de páginas clicável.
- **Corpo:** Títulos em Azul Escuro (#003366), parágrafos com espaçamento 1.5 e imagens com legendas.
- **Rodapé:** Numeração de página centralizada (ex: "Página 1 de 10").

---

## Exemplo 2: Documento de Dados Estruturados (JSON $\rightarrow$ PDF)

### ❌ Ruim (Tabela simples)
Uma tabela gigante que ultrapassa a largura da página, tornando o texto ilegível.
**Problema:** Não houve adaptação do layout para o tamanho da página.

### ✅ Excelente (Layout Adaptativo)
- **Uso de Colunas:** Divisão de dados em colunas proporcionais.
- **Cores Alternadas:** Linhas de tabela com cores alternadas (Zebra striping) para facilitar a leitura.
- **Soma Total:** Destaque em negrito no final da tabela de valores.
