# Workflow: Validar Qualidade do Artigo SBC

<required_reading>
**Leia agora:**
1. references/sbc-standards.md
2. references/academic-writing-pt.md
3. references/review-criteria.md
4. templates/dod-checklist.md
5. templates/quality-rubric.md
</required_reading>

<process>
## Passo 1: Definir escopo da validação

Pergunte (se não informado):
- O artigo está completo ou é uma seção específica?
- Qual é o evento/revista alvo? (afeta limites de páginas e formatação)
- O que mais preocupa: estilo, completude, formatação ou referências?

## Passo 2: Aplicar o DoD Checklist completo

Execute o checklist em `templates/dod-checklist.md` categoria por categoria.

**Categorias BLOQUEANTES (1-6):** qualquer item ❌ impede submissão imediata.
**Categorias RECOMENDADO (7-9):** meta ≥80% de itens ✅.

Ao concluir o DoD, registre:
- Categorias 1-6: quantos itens ❌ (se zero → passa)
- Categorias 7-9: X/Y itens ✅

## Passo 3: Aplicar a Rubrica de Qualidade

Score cada dimensão de 1-5 usando `templates/quality-rubric.md`:

| Dimensão | Score |
|---|---|
| D1 — Clareza do problema | ___/5 |
| D2 — Novidade/Contribuição | ___/5 |
| D3 — Rigor metodológico | ___/5 |
| D4 — Qualidade das evidências | ___/5 |
| D5 — Estrutura e fluxo | ___/5 |
| D6 — Escrita acadêmica | ___/5 |
| **TOTAL** | **___/30** |

**Thresholds:**
- ≥27/30 → venues A1/A2 (BRACIS, SBBD, top tracks)
- 24-26/30 → venues B1/B2 (workshops, tracks gerais)
- 20-23/30 → melhorar antes de submeter
- <20/30 → reescrita significativa necessária

## Passo 3: Análise de métricas de escrita

Para cada seção fornecida, avalie:

**Densidade de informação:**
- Parágrafos de 4-8 linhas são ideais
- Parágrafos muito curtos (1-2 linhas): fundidos ou expandidos
- Parágrafos muito longos (>12 linhas): divididos

**Proporção de seções (artigo completo de 8 págs):**
| Seção | Proporção esperada |
|-------|-------------------|
| Abstract/Resumo | ~0.3 pág cada |
| Introdução | 0.5-1 pág |
| Trabalhos Relacionados | 1-1.5 págs |
| Metodologia | 1.5-2 págs |
| Resultados | 1.5-2 págs |
| Conclusão | 0.5-1 pág |
| Referências | restante |

**Indicadores de escrita fraca:**
- Frases com mais de 40 palavras: reescrever
- "É importante ressaltar que..." / "Vale a pena mencionar..." → remover, afirme diretamente
- "Muito", "bastante", "inúmeros" sem dados → substituir por números
- Voz passiva excessiva (>40% das frases): balancear

## Passo 4: Relatório de validação

Produza um relatório estruturado:

```
RELATÓRIO DE VALIDAÇÃO — [Título do Artigo]
Evento alvo: [evento]

═══════════════════════════════════════
DOD CHECKLIST
═══════════════════════════════════════
Categorias 1-6 (Bloqueante): [X] itens ❌
  ❌ [item]: [o que corrigir]
Categorias 7-9 (Recomendado): [X/Y] itens ✅ ([%])

═══════════════════════════════════════
RUBRICA DE QUALIDADE
═══════════════════════════════════════
D1 Problema:      [X]/5
D2 Novidade:      [X]/5
D3 Metodologia:   [X]/5
D4 Evidências:    [X]/5
D5 Estrutura:     [X]/5
D6 Escrita:       [X]/5
TOTAL:            [X]/30

═══════════════════════════════════════
VEREDICTO
═══════════════════════════════════════
[✅ PRONTO PARA SUBMISSÃO / ⚠️ REQUER MELHORIAS / ❌ BLOQUEADO]
Venue recomendado: [A2/B1/B2 conforme score]

═══════════════════════════════════════
AÇÕES PRIORITÁRIAS
═══════════════════════════════════════
🔴 BLOQUEANTE:
  1. [ação obrigatória]
  2. [ação obrigatória]

🟡 MELHORIA (aumenta score):
  1. [ação para melhorar dimensão X]
  2. [ação para melhorar dimensão Y]
```

## Passo 5: Oferecer correções

Para cada problema identificado, ofereça:
- Texto original com o problema
- Texto sugerido corrigido
- Explicação da mudança

Priorize por impacto: conformidade SBC > coerência científica > estilo > formatação.
</process>

<success_criteria>
- [ ] Checklist completo executado
- [ ] Problemas priorizados por gravidade
- [ ] Relatório de validação gerado
- [ ] Correções concretas oferecidas para cada problema
- [ ] Artigo pronto para submissão ou lista clara do que falta
</success_criteria>
