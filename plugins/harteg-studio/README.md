# Harteg Studio

Plugin para Claude Cowork que cria **carrosséis de Instagram prontos a publicar** — e já vem com um **editor visual** para ajustar e exportar os slides sem mexer em código.

## O que tem dentro

- **Habilidade `harteg-studio`** — o playbook que o Claude carrega sozinho quando lhe pedes um carrossel. Descobre a marca, propõe o sistema visual (tipografia, paleta, voz), escreve a copy slide a slide e gera um `slides.json`.
- **Harteg Studio (`carousel-studio.html`)** — um editor visual standalone. Abre no navegador, edita textos e cores por um painel lateral (sem quebrar o layout), troca a imagem de fundo de cada slide e exporta os PNGs em 1080x1350 (2x). Funciona com os 8 kits tipográficos e os formatos 4:5, 1:1 e 9:16.

## Como usar

1. Pede um carrossel ao Claude ("cria um carrossel sobre X"). A habilidade conduz as perguntas e gera o `slides.json`.
2. Abre o **Harteg Studio** no navegador.
3. Clica em **Importar JSON** e escolhe o `slides.json` (ou edita o exemplo que já vem carregado).
4. Ajusta no painel lateral, escolhe as cores e clica em **Exportar PNGs**.
5. Para guardar as edições, usa **Guardar JSON** e reimporta depois.

O editor vai buscar os tipos de letra ao Google Fonts e usa internet só para carregar tipos de letra e exportar; ao exportar, os tipos de letra ficam embebidos no PNG.

## Nota técnica

O editor (`carousel-studio.html`) é autossuficiente para render e exportação — é o caminho recomendado. O script Python interno da habilidade é opcional.
