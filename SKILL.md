---
name: sbc-article
description: Auxilia na criação de artigos acadêmicos no padrão SBC (Sociedade Brasileira de Computação). Cobre kickoff de projeto, organização de dados, escrita acadêmica em português, formatação LaTeX, busca de embasamento científico, seleção de venue e validação de qualidade com DoD e rubrica de score. Use quando o usuário precisa escrever, estruturar ou revisar um artigo para submissão em eventos ou revistas da SBC.
---

<essential_principles>
## Princípios para Artigos SBC

**1. Padrão SBC é obrigatório**
Todo artigo deve seguir o template oficial SBC (sbc-template.sty). Margens (3cm superior, 2.5cm inferior, 3cm laterais), fontes (Times 12pt) e estrutura são definidos pelo template — não customize sem necessidade.

**2. Escrita acadêmica em português formal**
- Terceira pessoa do singular ou plural ("Este trabalho propõe...", "Os resultados indicam...")
- Sem coloquialismos, sem primeira pessoa ("eu fiz", "a gente")
- Voz ativa predominante (>60%); passiva aceitável em metodologia
- Precisão terminológica: use termos técnicos corretos da área

**3. Toda afirmação precisa de embasamento**
Afirmações factuais requerem citação. Prefira artigos peer-reviewed: IEEE, ACM, Springer, SBC, CAPES. Nunca cite referência sugerida por IA sem verificar que existe.

**4. Estrutura IMRaD adaptada para SBC**
Introdução → Trabalhos Relacionados → Metodologia → Resultados → Conclusão (+ Referências)
Sempre consulte o CFP (Call for Papers) do evento alvo — limites e variações são frequentes.

**5. LaTeX é o formato padrão**
A SBC fornece template LaTeX. Word só é aceito em alguns eventos específicos. Priorize LaTeX com sbc-template.

**6. Definition of Done (DoD) é o critério de conclusão**
Um artigo está "pronto" somente quando o DoD Checklist (`templates/dod-checklist.md`) for 100% nas categorias bloqueantes e a Rubrica de Qualidade (`templates/quality-rubric.md`) atingir ≥24/30.

**7. IA como ferramenta, não como autor**
Use IA para revisão de linguagem, estruturação e identificação de gaps. Nunca para gerar dados, inventar referências ou substituir análise crítica. Veja `references/ai-writing-guidelines.md`.
</essential_principles>

<intake>
O que você quer fazer?

1. **Iniciar um novo artigo** — Tenho uma ideia/pesquisa e quero começar do zero (kickoff)
2. **Organizar meus dados** — Tenho informações/resultados e preciso estruturar em artigo
3. **Escrever uma seção** — Preciso escrever ou melhorar uma seção específica
4. **Buscar embasamento** — Preciso encontrar referências e evidências científicas
5. **Formatar em LaTeX** — Preciso formatar no template SBC
6. **Validar o artigo** — Quero revisar qualidade, DoD e score de rubrica
7. **Escolher onde publicar** — Preciso selecionar o evento/revista SBC certo
8. **Verificar citações** — Quero validar se uma referência existe e checar seu Qualis

**Aguarde sua resposta antes de prosseguir.**
</intake>

<routing>
| Resposta | Workflow |
|----------|----------|
| 1, "iniciar", "começar", "novo artigo", "kickoff" | `workflows/kickoff-article.md` |
| 2, "organizar", "dados", "estruturar" | `workflows/organize-data.md` |
| 3, "escrever", "seção", "intro", "metodologia", "conclusão", "abstract" | `workflows/write-section.md` |
| 4, "buscar", "referência", "embasamento", "prova", "evidência", "fonte" | `workflows/find-evidence.md` |
| 5, "latex", "formatar", "template", "formato" | `workflows/latex-formatting.md` |
| 6, "validar", "revisar", "qualidade", "checar", "DoD", "rubrica" | `workflows/validate-article.md` |
| 7, "venue", "evento", "publicar", "onde", "QUALIS", "submeter" | `workflows/select-venue.md` |
| 8, "verificar", "citação", "bibtex", "validar citação" | `workflows/check-citations.md` |
| outro | Peça esclarecimento e roteie |

**Após ler o workflow, siga-o exatamente.**
</routing>

<reference_index>
Todo conhecimento de domínio em `references/`:

**Padrões SBC:** sbc-standards.md
**Escrita acadêmica:** academic-writing-pt.md
**Estrutura do artigo:** article-structure.md
**Citações e referências:** citation-methods.md
**Busca de evidências:** evidence-strategies.md
**Critérios de revisão SBC:** review-criteria.md
**Venues e QUALIS:** qualis-guide.md
**Uso ético de IA:** ai-writing-guidelines.md
</reference_index>

<templates_index>
Templates prontos em `templates/`:

**Template LaTeX completo:** full-article-template.md — estrutura completa com placeholders documentados
**Templates por seção:** section-templates.md — estrutura de parágrafos + frases-modelo para cada seção
**DoD Checklist:** dod-checklist.md — checklist binário de conclusão (bloqueante + recomendado)
**Rubrica de qualidade:** quality-rubric.md — score 1-5 por dimensão, threshold 24/30 para submissão
</templates_index>

<workflows_index>
| Workflow | Propósito |
|----------|-----------|
| kickoff-article.md | Coleta estruturada para iniciar artigo do zero — brief + gaps + próximos passos |
| organize-data.md | Transforma dados brutos do usuário em estrutura de artigo |
| write-section.md | Escreve ou melhora seções com templates e estilo acadêmico SBC |
| find-evidence.md | Estratégias para encontrar referências e embasamento científico |
| latex-formatting.md | Formatação LaTeX completa no template SBC |
| validate-article.md | Validação com DoD Checklist + Rubrica de Qualidade + veredicto |
| select-venue.md | Seleciona evento/periódico SBC adequado com base em área, nível e deadline |
| check-citations.md | Verifica a existência de uma citação e identifica seu Qualis |
</workflows_index>
