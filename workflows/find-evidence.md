# Workflow: Buscar Embasamento Científico

<required_reading>
**Leia agora:**
1. references/evidence-strategies.md
2. references/citation-methods.md
</required_reading>

<process>
## Passo 1: Entender a necessidade

Pergunte (se não informado):
- Qual afirmação/seção precisa de embasamento?
- Qual é o tema específico? (ex: "eficiência de algoritmos de clustering", "IoT em saúde")
- Qual tipo de evidência falta? (trabalhos relacionados, fundamentação teórica, dados/estatísticas, metodologia validada)

## Passo 2: Formular queries de busca

Para cada necessidade, crie queries para bases científicas:

**Google Scholar:**
```
"[termo exato]" site:dl.acm.org OR site:ieeexplore.ieee.org
[termo] [ano_inicial]:[ano_final] survey OR review
```

**IEEE Xplore / ACM DL (portais preferenciais da SBC):**
- Busque por termos em inglês (publicações internacionais)
- Use filtros: Conference Paper, Journal Article, 2018-2025

**Bases brasileiras:**
- SBBD, SBSI, SBES, SBRC (eventos SBC relevantes por área)
- SBC OpenLib: sol.sbc.org.br
- CAPES Periódicos: periodicos.capes.gov.br

## Passo 3: Critérios de qualidade

Priorize nesta ordem:
1. **Tier A** — IEEE Transactions, ACM TOIS, journals Qualis A1/A2 CAPES
2. **Tier B** — Conferências IEEE/ACM top (ICSE, VLDB, WWW, SIGIR), eventos SBC principais
3. **Tier C** — Conferências nacionais SBC, workshops com revisão
4. Evite: preprints sem revisão, blogs, sites sem peer-review

**Indicadores de qualidade:**
- h-index do veículo (Google Scholar Metrics)
- Qualis CAPES da área (quadriênio 2017-2020 ainda válido)
- Número de citações do artigo específico

## Passo 4: Estratégias por tipo de embasamento

### Para fundamentação teórica
- Busque surveys/reviews recentes (2020+) sobre o tema
- Query: `[tema] survey 2020 2021 2022 2023`
- Um bom survey já reúne as referências principais

### Para trabalhos relacionados
- Identifique 3-5 abordagens diferentes para o mesmo problema
- Para cada abordagem: cite 1-3 artigos representativos
- Busque: artigos que citam os mesmos artigos que você citaria (Google Scholar "Citado por")

### Para validação metodológica
- Cite o artigo original do método (ex: paper original do BERT, do k-means)
- Cite trabalhos que usaram o mesmo método em contexto similar

### Para dados e estatísticas
- Prefira: relatórios de organizações (IBGE, IDC, Gartner, IEEE, ACM)
- Cite a fonte primária, não o site que relata o dado
- Dados com mais de 5 anos: mencione o ano explicitamente no texto

## Passo 5: Formatar referências

Use o formato SBC (baseado em abntex2 ou formato próprio do evento):

**Artigo em conferência:**
```
SOBRENOME, N. Título do artigo. In: NOME DO EVENTO, XX., ANO, Cidade. Anais [...]. Porto Alegre: SBC, ANO. p. XX-XX.
```

**Artigo em periódico:**
```
SOBRENOME, N. Título do artigo. Nome do Periódico, v. XX, n. X, p. XX-XX, ANO.
```

**Em LaTeX com BibTeX:**
```bibtex
@inproceedings{chave2023,
  author    = {Sobrenome, Nome},
  title     = {Título do Artigo},
  booktitle = {Anais do XX Simpósio Brasileiro de...},
  year      = {2023},
  pages     = {1--10},
  publisher = {SBC}
}
```

## Passo 6: Apresentar resultados

Para cada lacuna identificada, forneça:
- 2-4 referências relevantes com título, autores, venue, ano
- Breve justificativa de por que é relevante
- Trecho sugerido de como citar no texto
</process>

<success_criteria>
- [ ] Queries de busca fornecidas para cada lacuna
- [ ] Fontes priorizadas por qualidade (Tier A/B/C)
- [ ] Pelo menos 2-3 referências sugeridas por necessidade
- [ ] Formato de citação correto para SBC
- [ ] Texto sugerido de como integrar a citação
</success_criteria>
