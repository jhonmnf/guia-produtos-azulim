---
name: lendo-sites
description: Extrai, processa e resume conteúdo de URLs web, convertendo páginas HTML em formatos legíveis (Markdown) e filtrando ruídos como anúncios e menus.
type: information-extraction
---

# Lendo Sites

Esta skill transforma o Claude em um especialista em extração de dados web, focado em converter o caos de uma página HTML em informações estruturadas e úteis.

## Fluxo de Trabalho Obrigatório

Sempre que for solicitado a ler ou analisar um site, siga estas etapas:

### 1. Análise de URL e Acesso
- Valide se a URL é válida e acessível.
- Identifique a natureza do site (Artigo, Documentação, E-commerce, Rede Social).
- Verifique a necessidade de cabeçalhos específicos (User-Agent) para evitar bloqueios.

### 2. Extração e Limpeza (Noise Reduction)
- Extraia o conteúdo principal do corpo da página (`main`, `article` ou tags de conteúdo).
- Remova "ruídos" irrelevantes:
    - Banners de cookies e pop-ups.
    - Menus de navegação e rodapés repetitivos.
    - Links de redes sociais e anúncios laterais.
- Converta o HTML limpo para Markdown para preservar a semântica (Títulos, Listas, Links).

### 3. Processamento de Informação
- Organize o conteúdo extraído logicamente.
- Identifique elementos chave: Autor, Data de Publicação, Títulos Principais e Pontos Chave.
- Se houver múltiplos links internos relevantes, liste-os como "Leituras Adicionais".

## Regras de Ouro de Extração
- **Fidelidade:** Não altere o sentido do texto original durante a conversão para Markdown.
- **Integridade de Links:** Preserve os URLs originais de referências e fontes citadas no texto.
- **Tratamento de Erros:** Se o site estiver bloqueado ou for dinâmico (JS pesado), informe claramente ao usuário e sugira alternativas (como fornecer o HTML salvo).

## Comando de Saída Esperado
Ao finalizar a leitura, entregue:
1. Um resumo executivo do conteúdo do site.
2. O conteúdo principal convertido em Markdown estruturado.
3. Uma lista de insights ou dados específicos solicitados pelo usuário.
