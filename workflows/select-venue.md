<select_venue_workflow>

## Objetivo
Ajudar o usuário a identificar o evento ou periódico SBC mais adequado para submeter seu artigo, com base na área, tipo de contribuição, nível desejado e deadline.

---

## Quando usar este workflow
- Usuário tem um artigo (ou ideia) e não sabe onde submeter
- Usuário quer maximizar QUALIS do venue
- Usuário tem deadline e precisa de opções com prazo compatível
- Usuário está em dúvida entre dois eventos

---

## ETAPA 1 — TRIAGEM INICIAL

Faça as seguintes perguntas (pode combinar em uma só mensagem):

1. **Área principal:**
   "Qual é a área principal do seu trabalho?"
   - Inteligência Artificial / Machine Learning
   - Banco de Dados / BI / Big Data
   - Engenharia de Software / Qualidade
   - Redes / Sistemas Distribuídos / Segurança
   - IHC / Realidade Virtual / Jogos
   - Educação / Informática na Educação
   - HPC / Sistemas Embarcados / IoT
   - Geral / Multidisciplinar

2. **Tipo de contribuição:**
   "Como você classificaria a contribuição do trabalho?"
   - Novo método/algoritmo
   - Aplicação em novo domínio
   - Estudo experimental/comparativo
   - Survey/mapeamento sistemático
   - Ferramenta/sistema
   - Estudo de caso
   - Trabalho em andamento (WIP)

3. **Nível desejado:**
   "Qual é seu objetivo com esta publicação?"
   - Máximo impacto (QUALIS A2/A3, aceito que é mais difícil)
   - Publicação segura (B1/B2, mais acessível)
   - Primeira publicação / TCC / Iniciação Científica

4. **Idioma:**
   "O artigo está em português, inglês ou qualquer um?"

5. **Deadline:**
   "Você tem algum deadline específico? Se sim, quando precisa submeter?"

---

## ETAPA 2 — MAPEAMENTO DE VENUES

Com base na área, consulte `references/qualis-guide` e mapeie os eventos compatíveis.

### Critérios de filtragem:
- **Escopo:** O tema do artigo está nos tópicos do evento?
- **Tipo:** O evento aceita o tipo de contribuição?
- **Nível:** O QUALIS esperado atende ao objetivo do usuário?
- **Idioma:** O evento aceita o idioma do artigo?
- **Deadline:** O deadline do evento é compatível com o prazo do usuário?

---

## ETAPA 3 — ANÁLISE DE FIT

Para cada venue candidato, avalie o fit:

```
ANÁLISE DE FIT — [NOME DO EVENTO]
─────────────────────────────────
Escopo: [Alinhado / Parcialmente alinhado / Pouco alinhado]
Razão: [por que o tema se encaixa ou não]

Tipo de contribuição: [Aceito / Pode ser aceito / Improvável]

QUALIS aproximado: [A2/A3/B1/B2]

Deadline típico: [MÊS/ANO] — [compatível / incompatível com sua data]

Idioma aceito: [PT / EN / Ambos]

Formato: [Artigo completo X-Y pág / Curto Z pág / WIP]

Nível de dificuldade: [Alta (>30% rejeição) / Média / Baixa]

Recomendação: [FORTEMENTE RECOMENDADO / RECOMENDADO / ALTERNATIVA]
```

---

## ETAPA 4 — APRESENTAÇÃO DE RECOMENDAÇÕES

Apresente TOP 3 venues na ordem:

### 1. [VENUE PRINCIPAL] — Recomendação primária
- **Por que:** [justificativa de fit]
- **QUALIS:** [classificação]
- **Deadline:** [data típica — sempre verificar no site do evento]
- **Formato:** [tipo de submissão + limite de páginas]
- **Como encontrar o CFP:** [sigla.sbc.org.br ou buscar "[sigla] [ano] call for papers"]
- **Atenção:** [se tem anonimização, sistemas especiais, etc.]

### 2. [VENUE ALTERNATIVO A] — Segunda opção
(mesma estrutura)

### 3. [VENUE ALTERNATIVO B] — Terceira opção / Backup
(mesma estrutura)

---

## ETAPA 5 — ORIENTAÇÕES PRÁTICAS

### Após escolher o venue, oriente o usuário:

**Passos imediatos:**
1. Acesse o site do evento e confirme o CFP do ano corrente
2. Verifique:
   - Deadline exato (submissão completa, não só abstract)
   - Template exigido (SBC ou ACM 2-col ou outro)
   - Limite de páginas exato
   - Política de anonimização (cego simples ou duplo-cego)
   - Sistema de submissão (SBC Open, EasyChair, JEMS)
3. Baixe o template oficial do CFP
4. Crie conta no sistema de submissão com antecedência

**Alerta de duplicação:**
"Lembre-se: nunca submeta o mesmo trabalho para dois eventos simultaneamente.
Submissão paralela é antiética e pode resultar em banimento."

**Se o trabalho for aceito:**
"Uma versão expandida de artigo de conferência pode ser submetida a periódicos
SBC após a conferência (ex: JBCS, RBIE). Verifique a política de extensão do evento."

---

## REFERÊNCIA CRUZADA

Para informações detalhadas de cada venue, consulte:
- `references/qualis-guide` → tabela completa de eventos + QUALIS
- `references/sbc-standards` → requisitos de formatação por tipo de submissão

</select_venue_workflow>
