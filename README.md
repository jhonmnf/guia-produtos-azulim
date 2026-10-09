# Guia de Produtos Azulim

Catálogo web de produtos Azulim com busca por nome ou descrição, organização por categoria e visualização de detalhes.

## Executar localmente

A página carrega `products_data.json` pelo navegador, por isso use um servidor HTTP em vez de abrir o HTML diretamente.

Com Python instalado, execute na raiz do repositório:

```bash
python -m http.server 8000
```

Acesse `http://localhost:8000`. O site é estático e também pode ser publicado no GitHub Pages.

## Estrutura

- `index.html`: catálogo, busca e detalhes dos produtos.
- `products_data.json`: base do catálogo.
- `fotos/`: imagens dos produtos.
- `fotos de erros ou info/`: imagens de referência.
- `skills/`: materiais e instruções auxiliares.

## Manutenção

Ao atualizar o catálogo, mantenha cada caminho de imagem correspondente a um arquivo em `fotos/`. Confira a pesquisa, a abertura dos detalhes e a exibição em celular antes de publicar.

A página do catálogo foi recuperada da versão `adf40af`, anterior à substituição por conteúdo pessoal. A versão pessoal continua preservada no histórico Git.

Não há processo de build ou testes automatizados configurados.
