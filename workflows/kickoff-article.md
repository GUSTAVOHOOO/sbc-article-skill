<kickoff_workflow>

## Objetivo
Coletar todas as informações necessárias para iniciar um artigo SBC do zero, avaliar viabilidade, mapear gaps e definir a estratégia de trabalho.

---

## Quando usar este workflow
- Usuário quer iniciar um novo artigo e não sabe por onde começar
- Usuário tem dados/resultados mas não sabe como estruturá-los em artigo
- Usuário precisa de orientação sobre o que é necessário antes de escrever

---

## ETAPA 1 — QUESTIONÁRIO DE KICKOFF

Faça as seguintes perguntas ao usuário (pode ser em blocos):

### Bloco A — O trabalho

1. **Tema geral:** "Qual é a área/tema principal do seu trabalho?" 
   *(Ex: detecção de anomalias, classificação de texto, sistemas distribuídos)*

2. **Problema específico:** "Qual problema concreto você está resolvendo?"
   *(Peça uma frase: "O problema é que [X] não consegue [Y] quando [Z]")*

3. **Contribuição principal:** "O que você fez que é novo ou diferente?"
   *(Peça uma frase: "Propusemos/desenvolvemos/avaliamos [NOME] que [FAZ O QUÊ]")*

4. **Tipo de contribuição:** "Como você classificaria seu trabalho?"
   - Proposta de novo método/algoritmo
   - Aplicação de método existente em novo domínio
   - Estudo experimental/comparativo
   - Survey/mapeamento sistemático
   - Ferramenta/sistema implementado
   - Estudo de caso
   - Outro

### Bloco B — Os dados e experimentos

5. **Dados disponíveis:** "Você já tem resultados experimentais?" 
   - Sim, experimentos completos
   - Sim, experimentos parciais
   - Não, ainda preciso executar os experimentos
   - Meu trabalho é teórico (sem experimentos)

6. **Baseline:** "Você comparou sua proposta com algum método existente?"
   - Sim, com [QUAIS]
   - Não ainda
   - Não se aplica

7. **Métricas:** "Quais métricas de avaliação foram usadas?"

### Bloco C — O contexto

8. **Venue alvo:** "Você já tem algum evento/periódico em mente para submeter?"
   - Sim: [QUAL] / Deadline: [DATA]
   - Não, preciso de ajuda para escolher
   - Qualquer evento SBC

9. **Idioma:** "O artigo será em português ou inglês?"

10. **Deadline:** "Quando precisa estar pronto para submissão?"

---

## ETAPA 2 — IDENTIFICAÇÃO DO TIPO DE CONTRIBUIÇÃO

Com base nas respostas, classifique o trabalho:

| Tipo | Estrutura principal recomendada | Foco dos Resultados |
|---|---|---|
| **Novo método** | Intro → Relacionados → Proposta → Avaliação → Conclusão | Comparação com baselines + análise de ablação |
| **Aplicação em novo domínio** | Intro → Domínio + Relacionados → Adaptação → Avaliação → Conclusão | Desafios do domínio + resultados adaptativos |
| **Estudo experimental** | Intro → Relacionados → Setup Experimental → Resultados → Discussão → Conclusão | Análise comparativa ampla + análise estatística |
| **Survey** | Intro → Metodologia de busca → Taxonomia → Análise → Lacunas → Conclusão | Tabela comparativa de trabalhos + lacunas identificadas |
| **Ferramenta/Sistema** | Intro → Arquitetura → Implementação → Avaliação de usabilidade/performance → Conclusão | Demonstração + benchmark |
| **Estudo de caso** | Intro → Contexto → Método aplicado → Resultados → Lições aprendidas → Conclusão | Resultados qualitativos + quantitativos + transferibilidade |

---

## ETAPA 3 — AVALIAÇÃO DE VIABILIDADE

Avalie honestamente com o usuário:

### Checklist de viabilidade:

**Mínimo para artigo completo (8-12 páginas):**
- [ ] Tem problema claramente definido
- [ ] Tem contribuição diferenciada (sabe por que é diferente do existente)
- [ ] Tem dados ou resultados (ou caminho para obtê-los)
- [ ] Tem pelo menos 1 baseline para comparação (se experimental)
- [ ] Conhece ao menos 5 trabalhos relacionados na área

**Sinais de alerta — discuta com o usuário:**
- Sem baseline definido → "Precisamos definir com o que comparar antes de escrever"
- Sem dados → "Sem experimentos, o artigo seria teórico/survey — é isso?"
- Contribuição vaga → "Precisamos formular uma contribuição específica e verificável"
- Deadline muito curto → "Com X semanas, vamos priorizar Y seções"

**Recomendação por situação:**
| Situação | Recomendação |
|---|---|
| Dados completos + baseline + deadline ok | Artigo completo (8-12 pág) |
| Dados parciais + deadline curto | Artigo curto/WIP (4-6 pág) |
| Sem dados ainda + tempo | Planejar experimentos primeiro |
| Sem baseline | Definir baselines antes de continuar |
| Trabalho teórico bem fundamentado | Survey ou artigo teórico |

---

## ETAPA 4 — GERAÇÃO DO BRIEF DO PROJETO

Após coletar as informações, gere um brief estruturado:

```
═══════════════════════════════════════════
BRIEF DO ARTIGO — [TÍTULO PROVISÓRIO]
═══════════════════════════════════════════

PROBLEMA:
[1 frase clara do problema]

CONTRIBUIÇÃO:
[1-3 frases descrevendo o que foi feito de novo]

TIPO: [Novo método / Aplicação / Experimental / Survey / Sistema / Estudo de caso]

VENUE ALVO: [evento + deadline]
IDIOMA: [PT / EN]
TIPO DE SUBMISSÃO: [Artigo completo / Curto / WIP]
TAMANHO: [X-Y páginas]

───────────────────────────────────────────
MAPEAMENTO DE SEÇÕES:
───────────────────────────────────────────
✅ Introdução → [esboço disponível / a escrever]
✅ Trabalhos Relacionados → [referências disponíveis / gap: precisam ser buscadas]
✅ [Metodologia/Proposta] → [dados disponíveis / parcial / a executar]
✅ Resultados → [completos / parciais / pendente]
✅ Conclusão → [a escrever após resultados]
✅ Referências → [X referências identificadas / gap: precisam mais Y]

───────────────────────────────────────────
GAPS IDENTIFICADOS:
───────────────────────────────────────────
❌ [GAP 1]: [o que falta + o que fazer]
❌ [GAP 2]: [o que falta + o que fazer]

───────────────────────────────────────────
PRÓXIMOS PASSOS RECOMENDADOS:
───────────────────────────────────────────
1. [AÇÃO 1 — mais urgente dado o deadline]
2. [AÇÃO 2]
3. [AÇÃO 3]
═══════════════════════════════════════════
```

---

## ETAPA 5 — ENCAMINHAMENTO

Após gerar o brief, ofereça ao usuário:

**O que quer fazer agora?**

1. **Escrever uma seção específica** → usar workflow `write-section`
2. **Buscar referências para os Trabalhos Relacionados** → usar workflow `find-evidence`
3. **Selecionar o venue certo** → usar workflow `select-venue`
4. **Ver o template completo do artigo** → ver `templates/full-article-template`
5. **Usar os templates de seção como base** → ver `templates/section-templates`
6. **Outra necessidade** → perguntar

</kickoff_workflow>
