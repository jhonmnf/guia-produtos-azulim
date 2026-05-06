# Referência Técnica de Extração Web

Este guia define as melhores práticas para a conversão de HTML para Markdown e filtragem de conteúdo.

## 1. Mapeamento de Tags HTML $\rightarrow$ Markdown
| Tag HTML | Elemento Markdown | Nota |
| :--- | :--- | :--- |
| `<h1>` até `<h6>` | `#` até `######` | Manter a hierarquia original. |
| `<p>` | Texto simples | Preservar parágrafos. |
| `<ul>`, `<ol>`, `<li>` | `-` ou `1.` | Converter listas aninhadas corretamente. |
| `<a>` | `[Texto](URL)` | Sempre preservar a URL original. |
| `<img>` | `![Alt](URL)` | Preservar o texto alt da imagem. |
| `<table>` | Tabela Markdown | Simplificar tabelas complexas se necessário. |
| `<strong>`, `<b>` | `**Texto**` | Preservar ênfases. |

## 2. Estratégias de Limpeza (Noise Filtering)
Para garantir que apenas o conteúdo relevante seja extraído, ignore as seguintes seletores CSS comuns:
- `.nav`, `.header`, `.footer`, `.sidebar`
- `.ad-container`, `.cookie-banner`, `.popup`
- `header`, footer, nav (tags semânticas)

## 3. Tratamento de Conteúdo Dinâmico
Se o conteúdo for renderizado via JavaScript (Single Page Applications):
- Notificar que a extração pode estar incompleta.
- Priorizar a leitura de meta-tags (`og:description`, `twitter:description`) para obter um resumo rápido.

## 4. Validação de Encoding
- Certificar que o conteúdo é processado em **UTF-8**.
- Corrigir entidades HTML (ex: `&amp;` $\rightarrow$ `&`, `&nbsp;` $\rightarrow$ ` `).
