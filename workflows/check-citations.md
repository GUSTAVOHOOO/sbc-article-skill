<check_citations_workflow>

## Objetivo
Verificar se uma referência acadêmica realmente existe, validar seus dados (autores, título, ano, venue) e identificar sua classificação Qualis (SBC/CAPES).

---

## Quando usar este workflow
- Usuário quer validar se uma citação sugerida pela IA ou encontrada online é real.
- Usuário precisa do Qualis de um artigo para relatórios ou avaliação de currículo.
- Usuário quer gerar um BibTeX correto e completo de uma obra.
- Usuário quer checar a integridade de uma lista de referências.

---

## ETAPA 1 — TRIAGEM DA CITAÇÃO (INTAKE)

Peça ao usuário a informação da citação. Ele pode fornecer em qualquer formato:
- **Texto bruto** (ex: "Artigo do Vaswani sobre Transformers de 2017")
- **Entrada BibTeX**
- **Título e Autores**
- **DOI ou Link**

---

## ETAPA 2 — PROCESSO DE VERIFICAÇÃO (AI INTERNAL)

Para validar a citação, siga estas sub-etapas:

### 1. Pesquisa e Identificação (Search)
- Use ferramentas de busca (Google Scholar, DBLP, Semantic Scholar) para localizar o artigo.
- **Validação Crítica:** Verifique se o título e autores batem exatamente com o resultado da busca para evitar "alucinações" de citações inexistentes.

### 2. Identificação do Venue (Venue ID)
- Identifique onde o trabalho foi publicado:
  - **Conferência/Simpósio:** Procure pelo nome em `booktitle`.
  - **Periódico/Journal:** Procure pelo nome em `journal`.
- Extraia o nome completo do evento ou jornal, evitando siglas ambíguas.

### 3. Consulta de Qualis (Qualis Lookup)
- Consulte `references/qualis-guide` para verificar se o venue está listado.
- Se não estiver nas referências locais, utilize busca web (Sucupira, PPGCC/PUCRS ou buscas por "[Nome do Venue] Qualis Computação").
- **Atenção:** Considere o novo modelo Qualis 2025-2028 (baseado em h5-index para conferências e CiteScore para periódicos).

### 4. Sincronização e Correção (BibTeX Sync)
- Gere ou corrija a entrada BibTeX com base nos dados oficiais encontrados.
- Certifique-se de incluir campos essenciais: `author`, `title`, `booktitle/journal`, `year`, `pages`, `doi` (se disponível).
- Aplique chaves duplas `{{...}}` em acrônimos no título para preservar a capitalização no LaTeX.

---

## ETAPA 3 — APRESENTAÇÃO DOS RESULTADOS

Apresente o resultado de forma estruturada:

```
RELATÓRIO DE VERIFICAÇÃO DE CITAÇÃO
───────────────────────────────────
STATUS: [✅ VERIFICADA / ⚠️ DADOS DIVERGENTES / ❌ NÃO ENCONTRADA]

Título: [Título oficial]
Autores: [Lista de autores]
Ano: [Ano de publicação]
Venue: [Nome completo da Conferência ou Journal]

CLASSIFICAÇÃO QUALIS:
Área: Ciência da Computação
Nível: [A1, A2, A3, A4, B1, B2, B3, B4, C ou N/A]
Fonte: [Sucupira / PPGCC-PUCRS / Estimativa por métrica]

ENTRADA BIBTEX CORRIGIDA:
[Bloco de código BibTeX]
```

---

## CRITÉRIOS DE SUCESSO
- **Existência comprovada:** O artigo foi localizado em base de dados confiável.
- **Venue identificado:** O local de publicação foi extraído sem ambiguidade.
- **Qualis verificado:** A classificação atual do venue foi identificada ou estimada.
- **BibTeX validado:** A entrada BibTeX gerada está pronta para uso no LaTeX da SBC.

---

## REFERÊNCIAS ÚTEIS
- `references/qualis-guide` → Regras e lista de venues.
- `references/citation-methods` → Padrões BibTeX e estilos SBC.

</check_citations_workflow>
