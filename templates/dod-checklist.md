<dod_checklist>

<!-- 
  DEFINITION OF DONE — Artigo SBC
  
  Use este checklist antes de submeter qualquer artigo.
  Todos os itens marcados como BLOQUEANTE devem estar ✅ para submissão.
  Itens RECOMENDADO aumentam a probabilidade de aceitação.
  
  Threshold mínimo: 100% dos itens BLOQUEANTE + ≥80% dos RECOMENDADO
-->

## CATEGORIA 1 — FORMATAÇÃO E TEMPLATE (Bloqueante)

- [ ] Template `sbc-template.sty` aplicado (baixado do CFP ou sol.sbc.org.br)
- [ ] Fonte Times New Roman 12pt no corpo, 10pt no resumo/abstract
- [ ] Margens: 3cm superior, 2.5cm inferior, 3cm laterais (A4)
- [ ] Layout de coluna única (NÃO duas colunas)
- [ ] Espaçamento simples
- [ ] Título em português E em inglês (quando exigido pelo evento)
- [ ] Número de páginas dentro do limite do CFP específico
- [ ] PDF compilado sem erros de LaTeX
- [ ] Arquivo PDF ≤ 10MB
- [ ] Submetido no sistema correto (SBC Open, EasyChair, JEMS, etc.)

---

## CATEGORIA 2 — SEÇÕES OBRIGATÓRIAS (Bloqueante)

- [ ] **Abstract** em inglês presente (≤10 linhas / ≤200 palavras)
- [ ] **Resumo** em português presente (≤10 linhas / ≤200 palavras)
- [ ] **Keywords** em inglês (3-6 termos)
- [ ] **Palavras-chave** em português (3-6 termos)
- [ ] **Introdução** com objetivo de pesquisa explícito
- [ ] **Trabalhos Relacionados** (seção própria ou dentro da Introdução)
- [ ] **Metodologia** (ou Proposta / Desenvolvimento / Experimentos)
- [ ] **Resultados** (ou Avaliação / Discussão)
- [ ] **Conclusão** com síntese + limitações + trabalhos futuros
- [ ] **Referências** formatadas no estilo SBC (sbc.bst)

---

## CATEGORIA 3 — FIGURAS, TABELAS E EQUAÇÕES (Bloqueante)

- [ ] Toda figura tem: número sequencial, legenda ABAIXO, referência no texto (`Figura X`)
- [ ] Toda tabela tem: número sequencial, legenda ACIMA, referência no texto (`Tabela X`)
- [ ] Toda equação tem: número entre parênteses à direita, referência no texto
- [ ] Figuras com resolução adequada (≥300 dpi para impressão)
- [ ] Legendas são autoexplicativas (leitor entende sem ler o texto)

---

## CATEGORIA 4 — REFERÊNCIAS E CITAÇÕES (Bloqueante)

- [ ] Toda referência na lista BibTeX foi citada no texto
- [ ] Toda citação no texto tem entrada correspondente na lista de referências
- [ ] Mínimo de referências adequado (tipicamente ≥10 para artigo completo)
- [ ] ≥1 artigo publicado em evento ou periódico SBC

---

## CATEGORIA 5 — ESCRITA ACADÊMICA (Bloqueante)

- [ ] Terceira pessoa em todo o texto (sem "eu fiz", "minha proposta")
- [ ] Sem linguagem coloquial ("muito bom", "ótimo resultado", "interessante observar")
- [ ] Siglas definidas na primeira ocorrência: "Aprendizado de Máquina (AM)"
- [ ] Termos técnicos usados consistentemente (mesmo nome em todo o artigo)

---

## CATEGORIA 6 — RIGOR CIENTÍFICO (Bloqueante)

- [ ] Objetivo de pesquisa declarado explicitamente na Introdução
- [ ] Metodologia descrita com detalhes suficientes para replicação
- [ ] Resultados respondem diretamente ao objetivo declarado
- [ ] Conclusão sintetiza os resultados (não apenas repete a Introdução)

---

## CATEGORIA 7 — QUALIDADE DE EVIDÊNCIAS (Recomendado)

- [ ] Todo claim factual tem citação (sem "é sabido que", "é evidente que")
- [ ] Citações primárias utilizadas (artigos originais, não tutoriais/blogs/Wikipedia)
- [ ] ≥60% das referências são dos últimos 5 anos
- [ ] Autocitação ≤20% das referências totais
- [ ] Fontes de Tier A/B predominam (IEEE Transactions, ACM, SBBD, BRACIS, etc.)

---

## CATEGORIA 8 — RIGOR EXPERIMENTAL (Recomendado — obrigatório se experimental)

- [ ] Dataset identificado: nome, tamanho, fonte, características
- [ ] Baseline(s) definido(s) e justificados
- [ ] Métricas de avaliação definidas antes dos experimentos
- [ ] Protocolo de validação descrito (k-fold, train/val/test, seed fixo)
- [ ] Ambiente de execução documentado (hardware, SO, versões de software)
- [ ] Teste estatístico aplicado quando relevante (Wilcoxon, t-test, etc.)

---

## CATEGORIA 9 — COERÊNCIA NARRATIVA (Recomendado)

- [ ] Parágrafos entre 4-8 linhas (máx. 12)
- [ ] Voz ativa predominante (>60% das frases)
- [ ] Transições presentes entre seções ("A seção seguinte apresenta...")
- [ ] Trabalhos Relacionados fecha com diferenciação explícita da proposta
- [ ] Limitações do trabalho discutidas honestamente
- [ ] Trabalhos futuros são concretos (não genéricos como "investigar mais")

---

## CATEGORIA 10 — ANONIMIZAÇÃO (Condicional — verificar CFP)

- [ ] Nomes dos autores removidos do PDF (se submissão duplo-cego)
- [ ] Afiliações removidas (se duplo-cego)
- [ ] Autocitações anonimizadas: "[OMITIDO PARA REVISÃO]"
- [ ] Metadados do PDF sem identificação dos autores

---

## RESULTADO FINAL

### Como calcular:
- **Categorias 1-6**: Todos os itens devem ser ✅ — qualquer ❌ BLOQUEIA submissão
- **Categorias 7-9**: Contar itens ✅ / total. Meta: ≥80%
- **Categoria 10**: Aplicar apenas se CFP exigir anonimização

### Veredicto:
| Situação | Ação |
|---|---|
| Categorias 1-6: 100% + Cat. 7-9: ≥80% | ✅ **Pronto para submissão** |
| Categorias 1-6: 100% + Cat. 7-9: 60-79% | ⚠️ **Melhorar qualidade antes de submeter** |
| Qualquer item Categoria 1-6 ausente | ❌ **Bloqueado — corrigir antes de qualquer coisa** |

</dod_checklist>
