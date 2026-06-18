# Harteg Studio

Harteg Studio é uma ferramenta para criação, gestão e otimização de carrosséis e conteúdos visuais, mantida pela Harteg.

Na prática, é um plugin para **Claude Cowork / Claude Code** que cria carrosséis de Instagram prontos a publicar e entrega um **editor visual** já preenchido com o carrossel gerado — para ajustar textos, tipografia, cores, imagem de fundo, cantos e exportar os PNGs em ZIP.

---

## Funcionalidades

- Sistema visual da marca de raiz (tipografia, paleta, voz) com 8 kits tipográficos.
- Copy slide a slide, com gancho que para o scroll, em português.
- Editor visual standalone (HTML offline) para ajustar fundo, posição dos textos, overlay, logótipo e exportar.
- PNGs retina 2x (1080x1350) prontos a publicar, exportados em ZIP.
- Formatos 4:5, 1:1 e 9:16; logótipo embebido; legenda + hashtags na voz da marca.
- Sistema visual guardado para reutilizar nos próximos carrosséis.

## Instalar

### Claude Cowork (app desktop)
1. Definições -> Plugins -> **Adicionar marketplace**.
2. Fonte **GitHub** -> indica: `AfonsoNunes03/harteg-studio`
3. Instala o plugin **harteg-studio** no catálogo.

### Claude Code (terminal)
```bash
/plugin marketplace add AfonsoNunes03/harteg-studio
/plugin install harteg-studio@harteg-studio-marketplace
```

## Utilização

Depois de instalar, pede: **"cria um carrossel sobre X"** (ou invoca a skill **/harteg-studio**). A habilidade conduz as perguntas, escreve a copy e entrega o `carrossel-editor.html` já preenchido. Abre-o no navegador, ajusta e clica em **Exportar ZIP**.

## Comando principal

```
/harteg-studio
```

Invoca o Harteg Studio diretamente. Em alternativa, basta pedir em linguagem natural ("cria um carrossel sobre X") que a habilidade é carregada automaticamente.

---

## Para o mantenedor (atualizar o plugin)

Edita o que quiseres em `plugins/harteg-studio/` (ex.: `carousel-studio.html` ou `skills/harteg-studio/SKILL.md`) e corre:

```bash
./atualizar.sh          # sobe o patch (1.9.2 -> 1.9.3) e faz push
./atualizar.sh minor    # 1.9.2 -> 1.10.0
./atualizar.sh 2.0.0    # versão exata
```

O script atualiza a versão no `plugin.json` e no `marketplace.json`, faz commit e push. Quem já instalou recebe a atualização ao atualizar o marketplace (Cowork: refresh; Claude Code: `/plugin marketplace update`).

## Estrutura

```
harteg-studio/
├── .claude-plugin/marketplace.json   # catálogo
├── plugins/harteg-studio/            # o plugin (habilidade + editor)
├── atualizar.sh                      # sobe versão e publica
└── README.md
```

## Autor

Desenvolvido e mantido por **Afonso Nunes** — Harteg.
Repositório: https://github.com/AfonsoNunes03/harteg-studio

## Licença

MIT. Ver [LICENSE](LICENSE).
