# VERTIC // MASTER CONTEXT v2
**Data:** 13 de junho de 2026
**Status:** Fonte única da verdade. Substitui o backup anterior (`transicao_outro_agente_prompt.md`), que continha inconsistências já resolvidas aqui.

---

## 1. Ecossistema & Posicionamento

A **VERTIC** é uma holding integradora no modelo *Full Stack Advisor* — posicionada como o "Sistema Operacional do empresário de alto valor (HNWIs)". A holding é o portal/núcleo; as entregas acontecem em vértices autônomas, cada uma com identidade própria mas herdando o DNA visual da holding.

---

## 2. Arquitetura de Marcas — DECISÃO B (4 vértices)

**Holding VERTIC** — o portal/OS. Cor **Neon Cyan**. O ciano é **reservado exclusivamente para a holding**; nenhuma vértice usa ciano como assinatura.

As 4 vértices autônomas:

1. **Vertic Marketing** — *Creative Purple* `#a855f7`. Crescimento, funis, branding, copy, tráfego. Tema base **claro** (`#f8fafc`) + roxo, com a transição *The Dark Choice* no fechamento. A **Fotografia/produção audiovisual** vive aqui como *capability* interna, não como marca separada.

2. **Vertic Consultoria** — *Trust Blue* `#3b82f6`. Diagnóstico, mapeamento de processos, otimização de margens, cultura e governança. É a camada que **descobre o problema e desenha a solução**. Tema escuro Finance Noir. Alimenta a Vertic Tech.

3. **Vertic Tech** — *Robotics Orange* `#f97316`. Plataformas sob medida, automações e engenharia de software. É a camada que **constrói o que a Consultoria diagnosticou**. Tema escuro Finance Noir. O material comercial já existente (proposta Strivo, assinado "VERTIC TECH" / "Vertic OS") pertence a esta vértice. As **Automações** são uma linha de entrega da Tech, não uma marca separada.

4. **Vertic Wealth** — *Champagne Gold*. Planejamento patrimonial + investimentos. Tema base **claro** + dourado, com a transição *The Ascension*. **PGR LAW é o braço jurídico parceiro** — empresa separada (regulada pela OAB), não uma sub da Vertic. A Wealth indica/integra com a PGR LAW; não a absorve.

**Pipeline natural entre vértices:** Consultoria (diagnóstico) → Tech (construção) → operação. Marketing e Wealth atendem demandas distintas (captação/marca e patrimônio/investimento).

**Cores aposentadas como marca:** Coral Red `#f43f5e` (era Fotografia → virou capability de Marketing). Permanece disponível só como acento terciário/ilustrativo se necessário.

---

## 3. Sistema de Cores (tokens)

### Base Finance Noir (holding e vértices escuras)
| Token | Hex | Uso |
|---|---|---|
| Obsidian Black | `#04070c` | Fundo absoluto (tema escuro) |
| Obsidian Light | `#f8fafc` | Fundo absoluto (tema claro) |
| Slate Gray | `#71717a` | Hastes do V-Node, texto secundário |
| Zinc Light | `#e4e4e7` | Texto/divisórias em escuro |
| Borda (escuro) | `rgba(63,63,70,0.35)` | Divisórias finas |

### Ciano — depende do fundo
| Token | Hex | Uso |
|---|---|---|
| Neon Cyan | `#06b6d4` | Canônico. Acento da holding em **tema escuro** |
| Deep Cyan | `#0e7490` | Ciano em **tema claro** (contraste sobre `#f8fafc`) |
| Pure Neon | `#00f0ff` | **Só FX/glow** no escuro (pulso, hover). Nunca em texto |

### Dourado — depende do fundo
| Token | Hex | Uso |
|---|---|---|
| Champagne Gold | `#B89454` | Assinatura Wealth em **tema claro** (sobre `#f8fafc`) |
| Luxury Gold | `#E5C158` | Acento/glint dourado em **tema escuro** (sobre obsidiana) |

*Lógica:* fundo claro exige metal mais escuro; fundo escuro exige metal mais claro. Mesma regra para os dois.

### Cores de vértice (assinatura)
| Vértice | Hex |
|---|---|
| Marketing | `#a855f7` |
| Consultoria | `#3b82f6` |
| Tech | `#f97316` |
| Wealth | `#B89454` / `#E5C158` (ver acima) |

### Tema Claro — texto & borda (Marketing e Wealth)
Marketing e Wealth operam sobre `#f8fafc`. Tokens Finance Noir substituídos por:

| Token | Hex | Uso |
|---|---|---|
| Text Dark | `#04070c` | Texto primário sobre fundo claro |
| Text Dark Sec | `#3f3f46` | Texto secundário sobre fundo claro |
| Slate Gray | `#71717a` | Texto muted (compartilhado escuro/claro) |
| Border Light | `#e4e4e7` | Divisórias finas no tema claro |

### Tema Claro — acentos de vértice
| Token | Valor | Uso |
|---|---|---|
| Marketing Border | `rgba(168,85,247,.12)` | Borda de card/painel sobre claro |
| Marketing Glow | `rgba(168,85,247,.06)` | Sombra/glow suave sobre claro |
| Wealth Border | `rgba(184,148,84,.15)` | Borda de card/painel sobre claro |
| Wealth Glow | `rgba(184,148,84,.06)` | Sombra/glow suave sobre claro |

*Pure Neon e Luxury Gold não se aplicam ao tema claro — exigem fundo escuro.*

---

## 4. Tipografia
- **Inter** — títulos e marca. Pesos Bold/ExtraBold, `letter-spacing: -0.05em`.
- **JetBrains Mono** — subtítulos, tags, números, tech data. `letter-spacing: 0.25em`, uppercase.

---

## 5. Os dois símbolos V-Node (geometria canônica)

> Geometria validada a partir do código real da proposta Strivo. A descrição do backup antigo (“inclinação 2, nó em 60,80, raio 9”) estava **incorreta** e foi descartada.

### Mark A — V-Node Icon (logotipo / lockup)
V único de traço grosso. Usado em logos, headers, favicons e nos lockups de todas as vértices.
```svg
<svg viewBox="0 0 100 100" fill="none" xmlns="http://www.w3.org/2000/svg">
  <path d="M20 25 L50 75 L80 25" stroke="#71717a" stroke-width="8"
        stroke-linecap="round" stroke-linejoin="round"/>
  <circle cx="50" cy="75" r="10" fill="VAR(--cor-vertice)"/>
</svg>
```
- **Haste:** sempre Slate Gray `#71717a` (neutra, funciona em fundo claro e escuro).
- **Nó:** a cor da vértice (ciano holding, roxo Marketing, azul Consultoria, laranja Tech, dourado Wealth).
- **Wordmark:** "VERTIC" em Inter ExtraBold (preto em fundo claro / branco em fundo escuro) + descritor da vértice na cor da vértice.

### Mark B — Triple V-Node (sistema / decorativo)
Três Vs aninhados (NÃO paralelos — inclinações 1.62 / 1.83 / 2.25, afunilando para dentro). Usado em preloader, loading screen e watermark do hero.
```svg
<svg viewBox="0 0 100 100" fill="none" xmlns="http://www.w3.org/2000/svg">
  <path d="M10 20 L50 85 L90 20" stroke-width="2"/>   <!-- externo -->
  <path d="M20 20 L50 75 L80 20" stroke-width="1.5"/> <!-- médio (acento) -->
  <path d="M30 20 L50 65 L70 20" stroke-width="1"/>   <!-- interno -->
  <circle cx="50" cy="75" r="4"/>                      <!-- nó: vértice do V médio -->
</svg>
```
- **Preloader (escuro):** externo branco, médio ciano `#06b6d4`, interno branco, nó ciano. Anima por `path-draw` (traços desenhando) + `circle-grow` (nó crescendo).
- **Watermark hero (escuro):** externo branco tracejado (`stroke-dasharray: 2 2`, baixa opacidade), médio e interno brancos, nó ciano.
- **Versão clara:** hastes navy `#1e293b`, médio e nó em Deep Cyan `#0e7490`.

---

## 6. The Shift (transições de tema)

Conceito-guarda-chuva com **dois membros direcionalmente opostos**:

- **The Ascension** (Wealth): escuro/ciano → **claro/dourado**. O cliente *sobe* ao status de patrimônio protegido. Gatilho: entrada na vértice Wealth.
- **The Dark Choice** (Marketing): claro/roxo → **escuro Finance Noir**. A página *mergulha* no tom rigoroso de negócios para o fechamento. Gatilho: fim da Fase 3 da landing de Marketing.

Wealth ascende para a luz; Marketing desce para a sombra.

---

## 7. Stack técnico (padrão herdado do Strivo)
- **CSS:** Tailwind (via CDN no Strivo; migrar para build local no site definitivo).
- **Fontes:** Inter + JetBrains Mono (Google Fonts).
- **JS:** vanilla (sem framework). Animações via scroll listeners, Intersection Observer (reveals), `path-draw`/`circle-grow` no SVG.
- **Componentes de UI já validados:** preloader animado, header sticky no scroll, navegação por dots laterais, efeito typing, reveals de seção.

---

## 8. Inventário de assets (13/06/2026)
- **Localização:** pasta `logos/` na raiz do projeto. Todos os assets existem em `.svg` e `.png`, versão dark e light.
- **Holding (SVG + PNG):** stacked, horizontal, header, icon, triple_v, loading, watermark_hero — dark/light.
- **Vértices com logo (SVG + PNG):** Marketing, Consultoria, Fotografia (capability), Automações (capability da Tech).
- **Vértices SEM logo ainda:** Tech e Wealth — assets pendentes de criação.
- **Propostas de cor (SVG + PNG):** 5 explorações arquivadas (neon_cyan, gold, royal_blue, crimson, emerald).
- **Workaround `.txt` na `logos_txt/`:** obsoleto. SVGs usáveis diretamente com `<img src="../logos/...svg">`.

---

## 9. Estado de desenvolvimento das páginas
- **Manual de marca** (`index.html`): construído. É referência de estilo, não o site.
- **Proposta Strivo** (Vertic Tech): construída. Template de proposta de alto nível e implementação de referência.
- **Landing Vertic Marketing:** só especificada (3 fases + Dark Choice). Sem código.
- **Site institucional da holding:** apenas conceito. Sem código.

### Spec da landing Marketing (3 fases)
1. **Hero/Boot:** fundo claro, partículas roxas atraídas pelo cursor + Triple V-Node montando via scroll.
2. **Demonstração:** MacBook 3D abrindo a tampa conforme o scroll, com navegador simulado de alto padrão na tela.
3. **Escala:** partículas viram grade cartesiana roxa ascendente com contadores de ROI/leads.
4. **The Dark Choice:** quebra para bloco escuro Finance Noir → dores + fechamento dos pacotes.

---

## 10. Vertic Marketing — Estratégia de Mercado (GTM)

> Migrado do backup `transicao_outro_agente_prompt.md`, que pode ser aposentado após esta consolidação.

### Público-alvo
Pequenos negócios locais, prospectados de forma presencial: clínicas médicas e odontológicas, consultórios, escritórios de advocacia e de arquitetura. Perfil de quem tem operação real mas carece de presença/estética corporativa de nível.

### Proposta de valor
Entregar a um pequeno negócio a **infraestrutura visual, a estética corporativa e a engenharia de dados de uma grande multinacional** — algo que normalmente está fora do seu alcance. É o "salto de categoria" percebido.

### Esteira de produtos (Módulos OS)
1. **Alpha Genesis** *(porta de entrada / "cavalo de Troia")* — Identidade Visual Premium + Landing Page de Elite em fundo claro. Entrega única, baixo custo operacional (alavancada por IA), alto impacto visual imediato. Serve para conquistar o cliente e provar valor rápido.
2. **Growth Vector** — Setup e gestão de anúncios (tráfego pago) + roteiros de vídeo de elite. Filosofia: menos posts, mais autoridade. Sobe o cliente da entrega pontual para a recorrência.
3. **Vertic OS** *(full stack)* — Gestão completa de redes, tráfego, copy e SEO + um **Cockpit de Dados** exclusivo (Growth Data Analyst / BI) rodando em tempo real. É o topo da esteira: o cliente passa a operar dentro do "sistema operacional" Vertic.

### Lógica da esteira
Alpha Genesis converte (impacto visual barato e rápido) → Growth Vector cria recorrência (tráfego + autoridade) → Vertic OS retém e aprofunda (operação + dados). A landing de Marketing (seção 9) é o funil que materializa essa narrativa, com *The Dark Choice* marcando a transição do encantamento visual para o fechamento comercial.

---

## 11. Itens em aberto / próximos passos
- [x] SVGs disponíveis em `logos/` — integrados ao manual via `<img>`. Workaround `.txt` obsoleto.
- [x] Confirmar paleta da Vertic Wealth além do dourado (tokens de texto/borda do tema claro). → Definidos na seção 3.
- [x] Atualizar o manual `index.html` para a arquitetura B → manual em `manual/index.html`, completo.
- [x] Construir landing Marketing — Fase 1 (Hero/Boot) em andamento. Ver seção 12.
- [x] Definir tokens completos do tema claro (borda, texto secundário, muted) para Marketing e Wealth. → Definidos na seção 3.
- [x] Consolidar estratégia GTM da Marketing no v2 (libera o `transicao_outro_agente` para deleção).
- [ ] Logos Vertic Tech e Vertic Wealth — ainda não criados.
- [ ] Landing Marketing: seções #how, #results, The Dark Choice, mobile, footer.

---

## 12. Estado de desenvolvimento — Landing Vertic Marketing (atualizado 2026-06-16)

**Arquivo:** `index.html` na raiz de `VERTIC_TESTES`. Repo: `filiperosa911/vertic` (GitHub Pages).

### Seções implementadas

| Seção | Status | Observações |
|---|---|---|
| Header | ✅ Completo | Logo SVG, nav, CTA, sticky |
| Hero — texto esquerdo | ✅ Completo | Badge, título, subtítulo, CTAs, tags público |
| Hero — animação scroll | ✅ Completo | V-Node glitch (low/high/exit) + MacBook entry |
| Hero — MacBook PNG | ✅ Completo | PNG 702px, clip-path SVG evenodd, vídeo na tela |
| Pricing cards | ✅ Completo | Liquid glass, 3 planos, badge destaque |
| #how (Como Funciona) | ⬜ Placeholder | Precisa de design e conteúdo |
| #results (Resultados) | ⬜ Placeholder | Precisa de cases e métricas |
| The Dark Choice | ⬜ Não iniciado | Transição claro→escuro no fechamento |
| Mobile | ⬜ Não iniciado | Decisão: showcase simples abaixo do hero |
| Footer | ⬜ Não existe | — |

### Detalhes técnicos do Hero (scroll-driven)

- `#hero`: `min-height: 260vh`, `position: relative`
- `.hero-sticky`: `position: sticky; top: 0; height: 100vh`
- Progresso do scroll: `(scrollY − hero.offsetTop) / (hero.offsetHeight − innerHeight)` → 0..1
- Glitch V-Node: 0.22→0.52 (low), 0.52→0.70 (high), 0.70+ (exit)
- MacBook entry: `macP = (p − 0.48) / 0.52`, easeOut cúbico
- MacBook size: `.mac-frame-wrap: 702px`, `.hero-vis: 702×676px`
- Clip-path (SVG global `id="mac-cut"`): inner rect `0.088,0.036 → 0.916,0.878`
- `.mac-screen-area`: `left:8.8% top:3.6% width:82.8% height:84.2% border-radius:10px 10px 0 0`
- Tela: `<video src="assets/sites-video.mp4" autoplay muted loop playsinline>`
