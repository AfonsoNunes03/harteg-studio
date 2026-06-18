# HARTEG STUDIO

Diretor de arte + redator que produz carrosséis de Instagram prontos a publicar, construindo de raiz o sistema visual da tua marca. Em português de Portugal, **100% autónomo** — sem depender de nenhum conector externo.

## O que entrega
- Sistema visual da tua marca (tipografia, paleta, voz) de raiz
- **O teu logótipo embebido** nos slides (só na capa ou como marca de água em todos)
- Copy slide a slide, com gancho que para o scroll
- HTML standalone que funciona offline (tipos de letra embebidos)
- PNGs retina 2x (1080×1350) prontos a publicar
- **Editor visual** (HTML offline) para ajustar fundo, posição dos textos, overlay e exportar
- Legenda + hashtags na voz da tua marca
- Um sistema visual guardado para reutilizar nos próximos carrosséis

## Como ativar
Diz algo como:
- "Quero fazer um carrossel de Instagram para a minha marca"
- "Ajuda-me com slides para IG sobre [tema]"
- "Usa a skill harteg-studio para criar um carrossel sobre [tema]"

## Estrutura
```
harteg-studio/
├── SKILL.md
├── references/        # base de conhecimento (marca, kits, voz, frameworks, técnico, workflow)
└── assets/
    └── carousel-studio.html   # o editor visual (única fonte de verdade)
```

## Requisitos
- **Ficheiros / artifacts:** para receber o `carrossel-editor.html`.
- **Navegador:** o editor abre no navegador; a exportação dos PNGs (botão **Exportar ZIP**) acontece do lado do cliente, sem Code Execution.
- **Internet:** só para carregar os tipos de letra do Google Fonts; ao exportar, ficam embebidos nos PNGs.

## Tipos de letra
Todos open-source (Google Fonts — licenças OFL/Apache). O editor carrega-os a partir do Google Fonts e embebe-os nos PNGs ao exportar.

## Os 8 kits
editorial · tech · brutalist · serif-classic · clean-sans · warm · playful · corporate
