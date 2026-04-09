<evidence_strategies>

<types_of_evidence>
**Tipos de evidência em artigos de computação:**

1. **Evidência experimental** — resultados de experimentos controlados (mais forte)
2. **Evidência comparativa** — seu método vs. baselines com métricas
3. **Evidência de caso real** — aplicação em dados/contexto real
4. **Evidência teórica** — provas matemáticas, análise de complexidade
5. **Evidência por consenso** — afirmações suportadas por múltiplas fontes independentes
6. **Evidência estatística** — testes de hipótese (t-test, Wilcoxon, etc.)
</types_of_evidence>

<strong_evidence_patterns>
**Padrões de evidência forte:**

**Para afirmações de desempenho:**
> "O método proposto alcançou F1-score de 0,92, superior aos baselines BERT (0,87) e RoBERTa (0,85) nos mesmos dados de teste [DATASET, ANO], com diferença estatisticamente significativa (p < 0,05, teste de Wilcoxon)."

**Para afirmações sobre o problema:**
> "Segundo [SILVA, 2023] e [COSTA, 2022], X representa um dos principais desafios em Y, afetando [dado quantitativo]% dos sistemas em produção."

**Para justificar escolha metodológica:**
> "Optou-se pelo algoritmo X por sua comprovada eficiência em cenários similares [AUTOR, ANO], e por apresentar complexidade O(n log n), adequada ao volume de dados do presente estudo."

**Para trabalhos futuros (com embasamento):**
> "Como trabalho futuro, planeja-se estender a abordagem para dados multilíngues, seguindo a direção sugerida por [LIMA, 2023], que identificou limitações similares em contextos bilíngues."
</strong_evidence_patterns>

<weak_evidence_to_avoid>
**Evidências fracas — evitar:**

- "É amplamente conhecido que..." → Prove com citação
- "Na prática, observa-se que..." → Cite estudo ou dado
- "Intuitivamente, podemos ver que..." → Mostre, não declare
- "É óbvio que..." → Nunca use isso
- Citar Wikipedia → Substitua pela fonte primária que a Wikipedia cita
- Citar apenas blogs ou sites comerciais → Busque artigo peer-reviewed equivalente
- "De acordo com dados recentes..." sem citar a fonte → Cite a fonte
</weak_evidence_to_avoid>

<experimental_design>
**Design experimental robusto para SBC:**

**Componentes obrigatórios:**
- **Dataset**: nome, tamanho, fonte, características relevantes
- **Baseline**: pelo menos 1-2 métodos de referência com implementação citada
- **Métricas**: definidas antes do experimento, justificadas teoricamente
- **Protocolo**: k-fold cross-validation, train/val/test split, seed fixada
- **Ambiente**: hardware (CPU/GPU/RAM), software (versões), tempo de execução

**Métricas por tipo de problema:**

| Tipo | Métricas comuns |
|------|----------------|
| Classificação | Acurácia, F1, Precisão, Recall, AUC-ROC |
| Regressão | MSE, RMSE, MAE, R² |
| Clustering | Silhouette, Davies-Bouldin, NMI |
| Recuperação de informação | MAP, NDCG, MRR, P@K |
| Geração de texto | BLEU, ROUGE, BERTScore |
| Tempo | Latência (ms), Throughput (req/s) |

**Testes estatísticos para SBC:**
- Comparação de dois métodos: teste de Wilcoxon (distribuição não-normal) ou t-test pareado
- Comparação múltipla: ANOVA + Tukey HSD ou Friedman + Nemenyi
- Reporte: média ± desvio padrão, p-value, tamanho do efeito
</experimental_design>

<finding_real_evidence>
**Estratégias práticas para encontrar evidências reais:**

**1. Snowballing backward** (a partir dos artigos que você já tem)
- Leia as referências do artigo mais relevante que você conhece
- Cada referência é um artigo potencialmente relevante
- Repita com os novos artigos encontrados

**2. Snowballing forward** (quem citou este artigo)
- No Google Scholar: clique em "Citado por X vezes"
- Filtre por ano recente (2020+)
- Artigos recentes que citam o clássico são os mais relacionados ao estado da arte

**3. Busca por survey** (visão geral rápida)
- Query: `"[tema]" survey 2022 OR 2023 OR 2024`
- Surveys reúnem referências principais — use como ponto de partida

**4. Connected Papers** (visualização de rede)
- connectedpapers.com — insira DOI de um artigo central
- Mostra graficamente artigos fortemente relacionados

**5. Semantic Scholar** (para ML/AI)
- semanticscholar.org — acesso aberto, filtro por influência
- Excelente para papers de IA/ML sem paywall

**6. SBC OpenLib** (específico SBC)
- sol.sbc.org.br — todos os artigos SBC em acesso aberto
- Busque por evento + ano + palavra-chave
</finding_real_evidence>

</evidence_strategies>
