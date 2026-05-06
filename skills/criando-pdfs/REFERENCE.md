# Referência Técnica de Layout PDF

Este guia define os padrões técnicos para a renderização de documentos PDF.

## 1. Padrões de Página
- **A4:** 210mm x 297mm (Padrão)
- **Letter:** 8.5in x 11in
- **Margens:** Padrão 25.4mm (1 polegada) em todos os lados.

## 2. Hierarquia Tipográfica (Sugerida)
| Elemento | Fonte | Tamanho | Estilo | Cor |
| :--- | :--- | :--- | :--- | :--- |
| Título Principal | Helvetica/Arial | 24pt | Bold | #000000 |
| Subtítulo | Helvetica/Arial | 16pt | Bold | #333333 |
| Corpo de Texto | Times New Roman | 12pt | Regular | #000000 |
| Legendas/Notas | Times New Roman | 10pt | Italic | #666666 |

## 3. Elementos Estruturais
- **Quebras de Página:** Devem ocorrer obrigatoriamente antes de cada novo Capítulo ou Seção Principal.
- **Tabelas:** Devem ter bordas sutis (#CCCCCC) e cabeçalhos destacados em cinza claro.
- **Imagens:** Devem ser centralizadas com legenda logo abaixo.

## 4. Ferramentas Recomendadas (Dependendo do Ambiente)
- **Python:** `ReportLab` (Alta performance/Baixo nível) ou `FPDF2`.
- **Node.js:** `Puppeteer` (HTML $\rightarrow$ PDF) ou `pdfkit`.
- **CLI:** `Pandoc` (Markdown $\rightarrow$ LaTeX $\rightarrow$ PDF).
