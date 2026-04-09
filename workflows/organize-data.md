# Workflow: Organizar Dados em Artigo SBC

<required_reading>
**Leia agora:**
1. references/article-structure.md
2. references/sbc-standards.md
</required_reading>

<process>
## Passo 1: Coleta de insumos

Pergunte ao usuário (use AskUserQuestion se necessário):
- **Tema/problema:** Qual problema este trabalho resolve?
- **Contribuição:** O que é novo/diferente neste trabalho?
- **Dados disponíveis:** Resultados experimentais, análises, comparações, protótipos?
- **Público-alvo:** Qual evento ou revista SBC?
- **Idioma:** Português ou inglês? (muitos eventos SBC aceitam inglês)

Se o usuário já trouxe os dados, extraia essas informações diretamente sem perguntar novamente.

## Passo 2: Identificar a contribuição central

Defina em 1-2 frases:
> "Este trabalho propõe/apresenta/avalia [CONTRIBUIÇÃO] para [PROBLEMA], utilizando [MÉTODO], e demonstra [RESULTADO PRINCIPAL]."

Apresente isso ao usuário e confirme antes de continuar.

## Passo 3: Mapear dados para seções

Classifique cada dado/informação fornecida pelo usuário em:

| Seção | O que vai aqui |
|-------|---------------|
| **Abstract** | Problema, método, resultado principal (150-200 palavras) |
| **Introdução** | Contexto, problema, gap, contribuição, organização do artigo |
| **Trabalhos Relacionados** | O que já existe e como este trabalho se diferencia |
| **Metodologia** | Como foi feito (reprodutível) |
| **Resultados** | O que foi encontrado (dados, tabelas, figuras) |
| **Conclusão** | O que foi alcançado, limitações, trabalhos futuros |
| **Referências** | Citações usadas |

## Passo 4: Identificar lacunas

Após o mapeamento, liste o que está faltando:
- [ ] Embasamento para a introdução
- [ ] Trabalhos relacionados identificados
- [ ] Dados experimentais completos
- [ ] Comparação com baseline
- [ ] Métricas de avaliação definidas

## Passo 5: Gerar esboço estruturado

Produza um esboço com:
- Título provisório
- Uma frase descrevendo cada seção
- Lista de dados/conteúdo disponível por seção
- Lista de lacunas a preencher

## Passo 6: Recomendar próximos passos

Ofereça as opções:
1. Escrever seções com os dados disponíveis (→ workflow write-section)
2. Buscar embasamento para as lacunas (→ workflow find-evidence)
3. Formatar o que já existe em LaTeX (→ workflow latex-formatting)
</process>

<success_criteria>
- [ ] Contribuição central definida em 1-2 frases
- [ ] Todos os dados do usuário mapeados para seções
- [ ] Lacunas claramente identificadas
- [ ] Esboço estruturado gerado
- [ ] Próximos passos recomendados
</success_criteria>
