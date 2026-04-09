<ai_writing_guidelines>

<!--
  DIRETRIZES DE ESCRITA COM IA — Uso Ético e Eficaz
  
  Framework para usar IA (Claude, ChatGPT, Gemini, etc.) como
  ferramenta de suporte na escrita de artigos acadêmicos SBC.
  
  Objetivo: maximizar qualidade, manter integridade acadêmica.
-->

## PRINCÍPIO FUNDAMENTAL

A IA é um **colaborador técnico**, não um autor.
O pesquisador é responsável por cada palavra, dado e conclusão do artigo.
A IA não tem acesso aos dados reais do seu experimento, não conhece o estado da arte da sua área específica, e não pode verificar a veracidade das informações — você sim.

---

## O QUE É ACEITÁVEL

### Uso permitido sem restrições:
- **Revisão de linguagem:** Verificar gramática, coesão, estilo formal
- **Reescrita de frases:** Melhorar clareza sem alterar conteúdo
- **Tradução:** Abstract/Resumo ou seções completas PT↔EN
- **Estruturação:** Organizar pontos em parágrafo coerente
- **Brainstorming:** Gerar ideias de trabalhos futuros, limitações a mencionar
- **Verificação de checklist:** Usar IA para revisar conformidade com DoD

### Uso permitido com supervisão humana cuidadosa:
- **Geração de rascunho de seção:** Desde que revisado, verificado e reescrito substantivamente
- **Sugestão de referências:** IA pode sugerir títulos/autores, mas você DEVE verificar que existem
- **Explicação de conceitos:** Para entender o que escrever — não copiar a explicação
- **Melhoria de abstract/resumo:** Revisar versão gerada por você

---

## O QUE É INACEITÁVEL

### Viola integridade acadêmica:
- **Fabricar referências:** Nunca cite referência que IA sugere sem verificar que existe e é real
- **Gerar dados:** Jamais use IA para simular, inventar ou extrapolar resultados experimentais
- **Copiar texto gerado por IA sem revisão substantiva:** Plágio de IA é plágio
- **Omitir contribuição da IA quando exigido:** Muitos eventos já pedem declaração de uso de IA

### Por que esses riscos são reais:
- Modelos de linguagem **alucinam referências** com frequência (autor real + título inventado)
- IA não conhece os dados do seu experimento — qualquer número gerado é invenção
- Detectores de IA estão se tornando mais comuns em revisão acadêmica

---

## WORKFLOW DE QUALIDADE COM IA

```
1. PESQUISA E DADOS (você, sem IA)
   └─ Coleta de dados, experimentos, análise de resultados
   └─ Leitura e síntese da literatura (IA pode ajudar a organizar, não a substituir)

2. RASCUNHO INICIAL (você, IA como auxiliar)
   └─ Escreva o rascunho das seções principais
   └─ Use IA para organizar bullet points em parágrafos
   └─ Use IA para verificar se a estrutura está clara
   └─ IA NUNCA gera os resultados ou interpretações — isso é seu

3. REVISÃO COM IA (IA como co-revisor)
   └─ "Revise a clareza e formalidade deste parágrafo"
   └─ "Este abstract segue a estrutura Contexto-Problema-Proposta-Resultado?"
   └─ "Quais limitações deste experimento não estão mencionadas?"
   └─ "Este parágrafo usa linguagem coloquial?"

4. VERIFICAÇÃO HUMANA (você, obrigatório)
   └─ Verifique CADA referência sugerida pela IA
   └─ Confirme que dados e métricas estão corretos
   └─ Releia toda seção revisada por IA antes de submeter

5. DECLARAÇÃO DE USO (quando exigido pelo evento)
   └─ Indique quais ferramentas foram usadas e para quê
```

---

## PROMPTS EFICAZES PARA ESCRITA COM IA

### Para revisar escrita acadêmica:
```
"Revise o trecho abaixo para garantir:
1. Terceira pessoa gramatical
2. Sem coloquialismos
3. Parágrafos com sentença tópico clara
4. Voz ativa predominante
[TRECHO]"
```

### Para melhorar o abstract:
```
"O abstract abaixo segue a estrutura: Contexto → Problema → Proposta → Método → Resultado → Impacto?
Identifique o que está faltando ou pode ser melhorado. Não reescreva — apenas aponte os problemas.
[ABSTRACT]"
```

### Para analisar coerência de seção:
```
"Leia esta seção e responda:
1. A contribuição anunciada na Introdução é respondida nos Resultados?
2. Algum parágrafo parece estar no lugar errado?
3. Há claims sem citação?
[SEÇÃO]"
```

### Para gerar sugestões de trabalhos futuros:
```
"Com base nos resultados e limitações descritos abaixo, sugira 3-5 direções concretas
de trabalhos futuros. Seja específico — evite 'investigar mais'.
Limitações: [...]
Resultados: [...]"
```

### Para verificar trabalhos relacionados:
```
"A seção de Trabalhos Relacionados abaixo:
1. Apenas lista trabalhos ou os analisa criticamente?
2. Fecha com diferenciação explícita do trabalho atual?
3. Os grupos temáticos estão claros?
[SEÇÃO]"
```

---

## VERIFICAÇÃO DE REFERÊNCIAS GERADAS POR IA

**REGRA ABSOLUTA:** Nunca cite uma referência que você não verificou existe.

### Como verificar:
1. Busque o título exato no Google Scholar, IEEE Xplore ou ACM DL
2. Confirme autores, ano e venue correspondem ao que a IA sugeriu
3. Leia pelo menos o abstract para confirmar que o paper trata do que você afirma
4. Baixe o PDF e confirme que você pode acessar o conteúdo citado

### Sinais de referência alucinada:
- Título muito genérico ("A Survey of Machine Learning Methods")
- Autores com nomes muito comuns sem outras publicações
- Venue inexistente ou sem histórico
- DOI inválido ou que não resolve

---

## TRANSPARÊNCIA E DECLARAÇÃO DE USO

### Quando declarar uso de IA:
- Quando o CFP do evento exigir explicitamente
- Quando a IA contribuiu substancialmente com texto (não apenas revisão de idioma)
- Quando há dúvida ética sobre o que declarar — declare

### Como declarar (modelo):
```
"Ferramentas de IA (especificamente [NOME]) foram utilizadas neste trabalho
exclusivamente para [PROPÓSITO ESPECÍFICO: revisão de linguagem / tradução / etc.].
Todo conteúdo científico, resultados e conclusões são de autoria dos pesquisadores."
```

### Eventos SBC com política conhecida (2024):
- A maioria ainda não tem política explícita — verifique o CFP de cada evento
- A tendência é exigir declaração, não proibir uso
- SBC OpenLib está atualizando diretrizes — confirme antes de submeter

---

## CHECKLIST DE USO ÉTICO

Antes de submeter, confirme:
- [ ] Toda referência foi verificada manualmente
- [ ] Nenhum dado ou resultado foi gerado ou alterado por IA
- [ ] Texto revisado por IA foi lido e aprovado linha por linha
- [ ] Declaração de uso incluída se exigida pelo evento
- [ ] Você consegue defender cada afirmação do artigo sem depender da IA

</ai_writing_guidelines>
