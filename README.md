# Radar de Posicionamento

Skill de Claude Code que conduz um estudo de mercado completo do zero — do "o que você vende" até um deck de posicionamento com GAP, Jobs-to-be-Done, Mapa de Valor (Value Proposition Canvas), ICP, persona e mapa sintoma × causa — e não deixa você (nem o Claude) inventar nada: toda afirmação carrega a fonte.

Serve para empresa, agência, profissional liberal ou infoproduto.

## Por que essa é diferente de pedir "faz um estudo de mercado" pro Claude

- **Rastreabilidade obrigatória.** Toda linha do deck carrega `[ARQ]` (arquivo do projeto), `[WEB]` (página buscada agora) ou `[USR]` (você respondeu). Sem uma dessas três, marca `[SEM FONTE]` e vira hipótese, nunca fato.
- **Fluxo guiado com portões.** A skill para em pontos-chave e pergunta antes de avançar — não robotiza um relatório genérico em 30 segundos.
- **Funciona mesmo sem produto ainda.** Se você ainda não vende nada, o Caminho B mapeia primeiro o que as pessoas já te pedem de graça — o sinal de demanda mais forte que existe.
- **Não para na pesquisa de mercado — chega até o encaixe da oferta.** Aplica o Value Proposition Canvas: fixa o Job (o que a pessoa tá tentando realizar), ranqueia Pains e Gains, e força um Mapa de Valor mostrando exatamente o que na SUA oferta resolve cada um — com uma nota de Fit (alto, médio, baixo) que expõe lacuna real de produto, não só de comunicação.
- **Sai um deck de verdade.** HTML autossuficiente, 40 slides, aplicando a identidade visual da sua marca (ou propondo uma, avisando que foi proposta).

## O que você precisa

| O quê | Para quê | Custo |
|---|---|---|
| [Claude Code](https://claude.com/claude-code) | roda a skill | plano pago do Claude |
| Busca na web ligada no Claude Code | as fases de dores e reclamações buscam na internet | incluída |
| Prints e links de 5 concorrentes | a Fase 1 lê esse material | grátis |

Não precisa saber programar.

## Passo a passo

**1. Baixe a skill**

Clique em **Code → Download ZIP** nesta página e descompacte. Ou, se usa Git:

```bash
git clone https://github.com/Cyntiaesb/radar-de-posicionamento.git
```

**2. Instale (escolha um)**

- **Só num projeto:** crie a pasta do seu estudo (ex.: `estudo-minha-marca`) e copie para dentro dela a pasta `.claude` que veio no download. Fica assim: `estudo-minha-marca/.claude/skills/radar-posicionamento/SKILL.md`.
- **Em todos os projetos:** copie a pasta `radar-posicionamento` (que está em `.claude/skills/`) para a pasta de skills do seu usuário:
  - Windows: `C:\Users\SEU-USUARIO\.claude\skills\radar-posicionamento\`
  - Mac: `~/.claude/skills/radar-posicionamento/`

> A pasta `.claude` começa com ponto e pode estar escondida. No Windows, ative "Itens ocultos" na aba Exibir do Explorador de Arquivos. No Mac, aperte `Cmd + Shift + .` no Finder.

**3. Abra o Claude Code na pasta do estudo**

Se o Claude Code já estava aberto, feche e abra de novo para ele enxergar a skill nova. Se tiver o manual da marca (cores, fontes, logo), coloque na pasta do estudo.

**4. Chame a skill**

Digite `/radar-posicionamento` ou peça:

> Conduz um estudo de mercado e posicionamento pra [sua marca ou produto].

**5. Siga o fluxo**

A skill para em cada fase e pergunta antes de avançar. Na Fase 1 ela pede prints dos concorrentes: salve numa pasta por concorrente dentro do projeto, por exemplo `concorrentes/clinica-sorriso/bio.png`.

**Tempo real:** depende de quanto material você já tem. São 6 fases (negócio → concorrentes → pesquisa → dores → reclamações → sugestões) antes do deck sair.

## O que você recebe no final

- `apresentacoes/{data}-radar-de-posicionamento.html` — o deck completo (abra com dois cliques no navegador)
- `apresentacoes/{data}-fontes.md` — registro de toda fonte usada (auditável)
- Os materiais brutos de cada fase, salvos como `.md` no projeto

## Problemas comuns

- **A skill não aparece:** confira se o arquivo ficou em `.claude/skills/radar-posicionamento/SKILL.md` (sem pasta a mais no meio) e reabra o Claude Code.
- **"Não consegui buscar na web":** a busca precisa estar liberada no Claude Code. Sem ela, as fases 3 e 4 ficam sem fonte e a skill avisa.
- **Muita coisa como `[SEM FONTE]`:** é esperado quando falta material. Junte mais prints e respostas de clientes e rode a fase de novo.

## Suporte

Dúvida ou bug: abra uma Issue neste repositório, ou me chama no Instagram [@cyntia.esberard](https://instagram.com/cyntia.esberard).
