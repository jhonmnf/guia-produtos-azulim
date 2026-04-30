# Referência Técnica de Web Design e CSS

Este guia serve como manual de consulta para a implementação de interfaces web de alta performance.

## 1. Paletas de Cores e Contraste
Para garantir a acessibilidade (WCAG), siga as proporções de contraste:
- **Texto sobre fundo:** Mínimo de 4.5:1 para texto normal.
- **Cores de Ação (Botões):** Devem ter contraste claro com o fundo para serem identificáveis instantaneamente.

## 2. Guia de Layouts (CSS Grid & Flexbox)
- **Flexbox:** Use para distribuições unidimensionais (uma linha ou uma coluna).
    - Ex: Menus de navegação, alinhamento de ícones.
- **CSS Grid:** Use para distribuições bidimensionais (linhas e colunas simultaneamente).
    - Ex: Grids de produtos, layouts de dashboard, estruturas de página complexas.

## 3. Escala Tipográfica
Para manter a harmonia visual, utilize uma escala multiplicadora (ex: 1.25) para definir tamanhos de fonte:
- H1: 2.5rem $\rightarrow$ H2: 2rem $\rightarrow$ H3: 1.6rem $\rightarrow$ P: 1rem.

## 4. Metodologia de Nomeação BEM
Estrutura: `bloco__elemento--modificador`
- **Bloco:** O componente principal (ex: `.card-produto`).
- **Elemento:** Parte do bloco (ex: `.card-produto__titulo`).
- **Modificador:** Versão diferente do bloco ou elemento (ex: `.card-produto--destaque`).

## 5. Performance e Otimização
- **Critical CSS:** Coloque os estilos essenciais do "above the fold" (topo da página) no `<head>`.
- **Sizing:** Use `box-sizing: border-box` globalmente para evitar que paddings alterem a largura total dos elementos.
