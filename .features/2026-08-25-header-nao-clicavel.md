---
data: 2026-08-25
titulo: Cabeçalho animado sem navegação ao clicar
tipo: melhoria
escopo: raiz
ferramenta: codex
arquivos:
  - README.md
---

## O que mudou

O cabeçalho animado passou a ser renderizado dentro de `<picture>`. O GitHub preserva a animação do SVG, mas deixa de adicionar automaticamente um link que abria o arquivo ao clicar na imagem.

## Por que

O renderizador do GitHub envolve elementos `<img>` isolados em um link para o arquivo original. Esse comportamento fazia o cabeçalho parecer um elemento interativo sem existir uma ação útil para o visitante.

## Como usar

Nenhuma ação é necessária. O README do perfil renderiza o cabeçalho normalmente e cliques sobre ele não navegam para o SVG.

## Notas

A solução foi confirmada pela API oficial de renderização Markdown do GitHub antes da publicação.
