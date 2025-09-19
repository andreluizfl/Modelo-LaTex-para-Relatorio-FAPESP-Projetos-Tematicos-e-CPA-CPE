# Modelo-LaTex-para-Relatorio-FAPESP-Projetos-Tematicos-e-CPA-CPE (ABNT)

Este repositório contém um template LaTeX para relatórios de projetos temáticos e centros de pesquisa aplicada (CPA/CPE) da FAPESP. O template segue as normas ABNT (NBR 14724:2011) e contém estilos, comandos e utilitários para gerar relatórios com layout padronizado.

## Estrutura principal
- `fapesp.sty` — pacote com estilos e comandos personalizados (capa, folhas, contadores, etc.). (Arquivo refatorado e comentado.)
- `fapesp.tex` — exemplo de documento principal que chama `fapesp.sty`.
- `Pré-Textual/`, `Textual/`, `Pós-Textual/` — pastas para organizar os elementos do relatório.
- `Pós-Textual/publicacoes.bib` e `Pós-Textual/referencias.bib` — arquivos de bibliografia.
- `README.md` — este arquivo.

## Principais funcionalidades
- Layout de acordo com ABNT (margens, cabeçalhos, espaçamento).
- Geração de capa, folha de rosto, resumo/abstract.
- Numeração de figuras/tabelas/equações por capítulo.
- Contadores automáticos para **orientações** (IC / ME / DO / Pós-doc).
- Contadores automáticos para **publicações** (baseados em `keywords` nas entradas `.bib`), tanto para:
  - todas as entradas do `.bib` (contagem global); quanto
  - apenas as entradas que foram efetivamente citadas no texto.

## Uso rápido

### Compilação sugerida
Recomenda-se o fluxo com `latexmk` ou manualmente:
