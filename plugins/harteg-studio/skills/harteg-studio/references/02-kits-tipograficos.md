# 02 — KITS TIPOGRÁFICOS
## 8 sistemas pré-curados, prontos a usar offline

---

## Porquê kits pré-curados

Escolher o tipo de letra é o mais difícil para o intermédio — são milhares de famílias e misturar mal arruína o design. Por isso há 8 kits onde Display + Body + Mono já foram testados como conjunto. Não mistures tipos de letra entre kits sem um motivo forte.

Cada kit tem 3 papéis:
- **Display** — títulos/capa, o tipo de letra "estrela" com personalidade.
- **Body** — corpo de texto, legível.
- **Mono** — kicker, índice, detalhes editoriais e o botão de CTA.

Cada kit corresponde a um conjunto de tipos de letra do Google Fonts. O editor (`assets/carousel-studio.html`) carrega o kit certo sozinho a partir do Google Fonts — tu só indicas o `kit` no JSON; ao exportar, os tipos de letra ficam embebidos nos PNGs.

---

## Árvore de decisão (por arquétipo)

| Arquétipo | Kit recomendado | Alternativa |
|---|---|---|
| Sábio | `serif-classic` | `editorial` |
| Inocente | `clean-sans` | `warm` |
| Explorador | `brutalist` | `tech` |
| Herói | `brutalist` | `corporate` |
| Fora-da-lei | `brutalist` | `editorial` |
| Mago | `editorial` | `playful` |
| Pessoa comum | `clean-sans` | `corporate` |
| Amante | `editorial` | `serif-classic` |
| Bobo da corte | `playful` | `clean-sans` |
| Cuidador | `warm` | `clean-sans` |
| Criador | `playful` | `editorial` |
| Soberano | `corporate` | `serif-classic` |

Para nicho de **tech / startup / IA / vibe coding**, o default mais seguro é `tech`. Para B2B sério, `corporate`. Para marca pessoal acolhedora, `warm`.

---

## Os 8 kits

### `editorial` — revista/moda, ousado
- Display: Anton (condensada, pesada) · Serif de apoio: Instrument Serif (itálico)
- Body: Inter · Mono: JetBrains Mono
- **Quando:** marca que quer impacto de capa de revista, contraste forte.

### `tech` — startup/SaaS/IA, moderno e limpo
- Display: Space Grotesk · Body: Inter · Mono: IBM Plex Mono
- **Quando:** produto digital, conteúdo técnico, vibe coding. Equilibra moderno + legível.

### `brutalist` — cru, alto impacto
- Display + Body: Archivo (até peso 900) · Mono: Space Mono
- **Quando:** marca que provoca, gancho agressivo, herói/fora-da-lei.

### `serif-classic` — livro de capa dura, autoridade
- Display: Playfair Display · Body: EB Garamond · Mono: Courier Prime
- **Quando:** consultoria, premium, conteúdo de profundidade. Sensação "NY Times".

### `clean-sans` — minimal, simpático
- Display + Body: Manrope · Mono: DM Mono
- **Quando:** marca que quer clareza e simpatia sem firulas. Ótimo default neutro.

### `warm` — humana, calorosa (sem cliché)
- Display: Fraunces · Body: Karla · Mono: DM Mono
- **Quando:** coaching, bem-estar, marca pessoal próxima.

### `playful` — criativo, enérgico
- Display: Syne · Body: Manrope · Mono: DM Mono
- **Quando:** marca jovem, divertida, criativa.

### `corporate` — corporativo, confiança
- Display + Body: Red Hat Display · Mono: Red Hat Mono
- **Quando:** B2B, serviço sério, soberano.

---

## Paletas iniciais sugeridas (ajusta à marca)

A paleta vai no JSON em `paleta`. Tokens: `bg` (fundo), `fg` (texto principal), `muted` (texto secundário), `accent` (cor da marca), `surface` (cards/contorno do número fantasma), `cream` (fundo claro de slides "respiro").

| Vibe | bg | fg | muted | accent | surface |
|---|---|---|---|---|---|
| Dark tech | #0A0A0A | #FFFFFF | #8A8A8A | #7C5CFF | #161616 |
| Dark quente | #0E0B08 | #F7F2EA | #9A8E7E | #FF6B35 | #1A1510 |
| Claro minimal | #F7F6F2 | #111111 | #6B6B6B | #2E5BFF | #E7E5DE |
| Premium escuro | #0C0C0E | #F2EBDD | #8E8A82 | #C9A24B | #18181C |

Regras: contraste alto entre `bg` e `fg`; `accent` usado com parcimónia (kicker, régua, número, CTA); slides "respiro" usam `cream` para dar ritmo no meio do carrossel (`"breather": true`).

---

## Como mostrar opções

Se o utilizador pedir para ver, monta o slide de capa com 2 kits candidatos no editor e mostra-os. Compara em tabela: kit, vibe, porque encaixa. Deixa-o escolher com critério.
