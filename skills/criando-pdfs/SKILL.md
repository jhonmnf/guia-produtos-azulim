---
name: criando-pdfs
description: Gera arquivos PDF profissionais a partir de conteúdo markdown, texto plano ou dados estruturados, gerenciando layout, fontes e exportação.
type: document-generation
---

# Criando PDFs

Esta skill automatiza a conversão de conteúdo digital em documentos PDF formatados, garantindo que a estrutura visual seja preservada e profissional.

## Fluxo de Trabalho Obrigatório

Sempre que for solicitado a gerar um PDF, siga estas etapas:

### 1. Definição de Estrutura (Layout)
- Identifique o tipo de documento (Relatório, Fatura, Ebook, Certificado).
- Defina as dimensões da página (A4, Letter, Custom).
- Determine a hierarquia visual: Títulos, Subtítulos, Corpo de Texto e Rodapés.

### 2. Processamento de Conteúdo
- Converta a entrada (Markdown/Texto) para o formato aceito pela ferramenta de renderização.
- Aplique estilos de tipografia (fontes, tamanhos e cores) conforme definido no `REFERENCE.md`.
- Insira elementos visuais (imagens, tabelas, quebras de página) nos locais apropriados.

### 3. Geração e Validação
- Execute o script de conversão para gerar o arquivo `.pdf`.
- Valide a integridade do arquivo:
    - Verifique se não houve quebras de linha inadequadas (estouro de página).
    - Confirme se as fontes foram renderizadas corretamente.
    - Valide se todos os links e sumários estão funcionais.

## Regras de Ouro de Formatação
- **Margens:** Mantenha margens padrão de 2,54cm a menos que especificado o contrário.
- **Acessibilidade:** Garanta que o texto seja selecionável (não gere PDFs como imagens).
- **Encoding:** Utilize obrigatoriamente UTF-8 para evitar erros de caracteres especiais.

## Comando de Saída Esperado
Ao final da geração, entregue:
1. O caminho do arquivo PDF gerada.
2. Um resumo do layout aplicado.
3. Uma sugestão de revisão para o usuário.
