# Estudo de Mercado & Posicionamento

Skill de Claude Code que conduz um estudo de mercado completo do zero — do "o que você vende" até um deck de posicionamento com GAP, ICP, persona e mapa sintoma × causa — e não deixa você (nem o Claude) inventar nada: toda afirmação carrega a fonte.

## Por que essa é diferente de pedir "faz um estudo de mercado" pro Claude

- **Rastreabilidade obrigatória.** Toda linha do deck carrega `[ARQ]` (arquivo do projeto), `[WEB]` (página buscada agora) ou `[USR]` (você respondeu). Sem uma dessas três, marca `[SEM FONTE]` e vira hipótese, nunca fato.
- **Fluxo guiado com portões.** A skill para em pontos-chave e pergunta antes de avançar — não robotiza um relatório genérico em 30 segundos.
- **Funciona mesmo sem produto ainda.** Se você ainda não vende nada, o Caminho B mapeia primeiro o que as pessoas já te pedem de graça — o sinal de demanda mais forte que existe.
- **Sai um deck de verdade.** HTML autossuficiente, 37 slides, aplicando a identidade visual da sua marca (ou propondo uma, avisando que foi proposta).

## Como usar

1. Copie a pasta `.claude/skills/estudo-mercado/` pra dentro do `.claude/skills/` do seu projeto no Claude Code (ou instale como skill global).
2. Abra o Claude Code no seu projeto (ideal: com o branding book da marca em algum lugar do projeto).
3. Peça: *"Conduz um estudo de mercado e posicionamento pra [sua marca/produto]"*.
4. Siga o fluxo — a skill vai pedir prints de concorrentes, orientar uma pesquisa, e parar em cada fase pra você confirmar antes de avançar.

**Tempo real:** depende de quanto material você já tem, mas espere passar por 6 fases (negócio → concorrentes → pesquisa → dores → reclamações → sugestões) antes do deck sair.

## O que você recebe no final

- `apresentacoes/{data}-estudo-mercado-posicionamento.html` — o deck completo
- `apresentacoes/{data}-fontes.md` — registro de toda fonte usada (auditável)
- Os materiais brutos de cada fase, salvos como `.md` no projeto

## Suporte

Dúvida ou bug: abra uma Issue neste repositório, ou me chama no Instagram [@cyntiaesberard](https://instagram.com/cyntiaesberard).
