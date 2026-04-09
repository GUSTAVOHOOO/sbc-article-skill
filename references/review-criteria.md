<review_criteria>

<!--
  CRITÉRIOS DE REVISÃO SBC
  
  O que revisores avaliam e como antecipar feedback antes de submeter.
  Baseado em critérios de aceitação de eventos SBC, CSBC, BRACIS, SBBD, SBES.
-->

## O QUE REVISORES AVALIAM

Revisores SBC respondem implícita ou explicitamente a estas perguntas:

### 1. Relevância
- **Pergunta:** "Este trabalho pertence a este evento/área?"
- **Sinal positivo:** Tema alinhado ao escopo do CFP, cita trabalhos do próprio evento
- **Sinal negativo:** Muito geral, fora da área, sem conexão com literatura da comunidade

### 2. Originalidade / Novidade
- **Pergunta:** "Isso já foi feito? O que é realmente novo aqui?"
- **Sinal positivo:** Contribuição claramente diferenciada dos trabalhos relacionados
- **Sinal negativo:** "Incremental demais", "é apenas aplicação de X em Y sem análise crítica"

### 3. Qualidade Técnica e Rigor
- **Pergunta:** "Os experimentos são válidos? Posso confiar nos resultados?"
- **Sinal positivo:** Metodologia replicável, baseline adequado, métricas justificadas
- **Sinal negativo:** "Sem baseline", "dataset não descrito", "sem análise estatística"

### 4. Suporte das Afirmações
- **Pergunta:** "Os claims são suportados por evidências?"
- **Sinal positivo:** Toda afirmação referenciada ou demonstrada experimentalmente
- **Sinal negativo:** "Os autores afirmam X mas não provam", "sem referências para Y"

### 5. Clareza e Apresentação
- **Pergunta:** "Consigo entender o que foi feito e por quê?"
- **Sinal positivo:** Estrutura clara, escrita precisa, figuras e tabelas informativas
- **Sinal negativo:** "Mal escrito", "confuso", "não fica claro qual é a contribuição"

### 6. Trabalhos Relacionados
- **Pergunta:** "Os autores conhecem o estado da arte?"
- **Sinal positivo:** Cobre abordagens principais, critica limitações, posiciona o trabalho
- **Sinal negativo:** "Referências desatualizadas", "ignora trabalho relevante [X]", "apenas lista, não analisa"

---

## MOTIVOS MAIS COMUNS DE REJEIÇÃO

Com base em padrões observados em eventos SBC (BRACIS, SBBD, SBES, CSBC):

### Técnicos (causes mais críticas):
1. **Sem baseline adequado** — "Os autores comparam apenas com versões anteriores do próprio método"
2. **Metodologia não-reproduzível** — "Faltam parâmetros, não posso replicar"
3. **Resultados sem análise estatística** — "Diferenças pequenas sem teste de significância não são conclusivas"
4. **Dataset muito pequeno ou não justificado** — "N=30 não é suficiente para as afirmações feitas"
5. **Métricas inadequadas para o problema** — "Accuracy em dataset desbalanceado não é métrica adequada"

### Científicos:
6. **Contribuição muito incremental** — "É apenas aplicação de método existente sem análise nova"
7. **Trabalhos relacionados incompletos** — "Ignora [X] que resolve o mesmo problema"
8. **Claims não suportados** — "Afirmam ser 'estado da arte' sem comparar com estado da arte"
9. **Problema mal motivado** — "Não fica claro por que isso é um problema relevante"

### De Apresentação:
10. **Introdução sem contribuições claras** — "Não consigo identificar qual é a contribuição do trabalho"
11. **Conclusão repete a Introdução** — "Sem síntese dos resultados reais"
12. **Figuras/tabelas sem discussão** — "Os resultados são apresentados mas não explicados"

---

## ANTECIPAR FEEDBACK: POR SEÇÃO

### Introdução — o revisor pergunta:
- "Qual é exatamente o problema?" → Tenha uma frase de problema no P2
- "Por que isso importa?" → Tenha evidência quantitativa de impacto
- "O que foi feito?" → Liste contribuições numeradas no P4
- "Por que não usar [método existente]?" → Antecipe no gap da literatura

### Trabalhos Relacionados — o revisor pergunta:
- "Por que este trabalho é diferente dos anteriores?" → Seção deve fechar com diferenciação explícita
- "Conhecem [paper X]?" → Cobertura abrangente, especialmente trabalhos recentes (2022+)
- "Estão apenas listando ou analisando?" → Critique limitações de cada grupo

### Metodologia — o revisor pergunta:
- "Posso replicar isto?" → Forneça dataset, parâmetros, protocolo, ambiente
- "Por que estas escolhas?" → Justifique dataset, baseline, métricas
- "O experimento é justo?" → Mesmas condições para todos os métodos comparados

### Resultados — o revisor pergunta:
- "A diferença é significativa?" → Inclua intervalos de confiança ou teste estatístico
- "Melhor em quê?" → Discuta trade-offs, não apenas vitórias
- "E quando falha?" → Análise de casos negativos aumenta credibilidade

### Conclusão — o revisor pergunta:
- "O objetivo foi atingido?" → Conecte explicitamente resultados ao objetivo da Introdução
- "Quais são as limitações reais?" → Seja honesto — revisores respeitam honestidade
- "O que vem a seguir?" → Trabalhos futuros concretos, não "investigar melhor"

---

## TIPOS DE REVISÃO SBC

### Duplo-cego (mais comum em conferências):
- Nomes e afiliações REMOVIDOS do PDF
- Autocitações anonimizadas: "[OMITIDO]"
- Revisores não sabem quem são os autores

### Simples-cego:
- Autores visíveis para revisores
- Revisores anônimos para autores

### Aberta (raro em SBC):
- Ambos identificados

**Sempre verificar o CFP do evento específico.**

---

## COMO USAR ESTE ARQUIVO

Antes de submeter, para cada seção do artigo, pergunte-se:
> "Se eu fosse revisar este artigo, o que criticaria nesta seção?"

Se você consegue identificar críticas óbvias, o revisor também conseguirá.
Corrija antes de submeter — não depois.

</review_criteria>
