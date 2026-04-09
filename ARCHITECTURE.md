# 🧠 Arquitetura da Skill: sbc-article

Este documento detalha o design sistêmico da skill `sbc-article`. Entender esta arquitetura é fundamental para desenvolvedores que desejam estender a skill ou replicar seu modelo de sucesso em outros domínios.

---

## 🏗️ Design System

A skill foi projetada sob o princípio de **Engenharia de Prompt Modular**. Em vez de um único prompt monolítico, ela utiliza uma estrutura de arquivos interconectados que gerenciam o contexto do agente de forma eficiente.

### 1. Camada de Orquestração (`SKILL.md`)
O arquivo raiz atua como o **Kernel** do sistema.
- **Trigger Detection:** Identifica quando a intenção do usuário é acadêmica.
- **Context Gatekeeping:** Define os "Princípios Essenciais" que o agente nunca deve violar (ex: proibição de inventar referências).
- **Intake & Routing:** Um mecanismo de menu que impede o agente de "adivinhar" o que fazer, forçando uma coleta de dados estruturada.

### 2. Camada de Base de Conhecimento (`references/`)
Atua como a **Memória de Longo Prazo** (Domain Knowledge).
- Estes arquivos são injetados no contexto apenas quando necessário.
- **Rigor Normativo:** Contêm as regras "frias" (margens, estilos, normas ABNT/SBC adaptadas).
- **Heurísticas de IA:** O arquivo `ai-writing-guidelines.md` ensina o agente a ser um revisor crítico, não um gerador passivo.

### 3. Camada Operacional (`workflows/`)
Define as **Máquinas de Estado** para cada tarefa.
- **Processos Multi-Etapa:** Cada workflow (como o `kickoff-article.md`) guia o agente por fases (Pergunta -> Classifica -> Avalia -> Gera).
- **Consumo de Tokens:** Ao separar workflows, garantimos que o agente foque apenas na lógica da tarefa atual, evitando a degradação de performance em conversas longas.

---

## 🔄 Ciclo de Vida do Trabalho (State Flow)

A skill gerencia o progresso do artigo através de um fluxo lógico:

1.  **Discovery (Kickoff):** Transforma uma ideia vaga em um `PROJECT BRIEF` estruturado.
2.  **Structuring (Organize Data):** Mapeia os dados do usuário para a estrutura IMRaD (Introdução, Metodologia, Resultados e Discussão).
3.  **Production (Write Section):** Utiliza `templates/section-templates.md` para garantir que cada parágrafo tenha uma função retórica (ex: "Sentença de Tópico" -> "Evidência" -> "Conclusão").
4.  **Refinement (Find Evidence):** Um loop de busca e validação de referências reais.
5.  **Quality Gate (Validate):** A fase final onde o artigo é testado contra o **DoD (Definition of Done)** e a **Rubrica de Qualidade**.

---

## 🛡️ Mecanismos de Segurança e Ética

Para evitar os problemas comuns de IAs generativas na academia, a arquitetura implementa:

- **Anti-Alucinação:** Instruções explícitas para o agente admitir quando não encontra uma evidência em vez de sugerir uma falsa.
- **Voz Ativa Controlada:** Algoritmos de instrução que forçam a IA a reescrever textos em voz passiva excessiva para um estilo mais claro e direto.
- **Verificação de Baseline:** O workflow de validação impede que um artigo seja considerado "Pronto" se não houver uma comparação clara com o estado da arte.

---

## 📊 Medição de Sucesso

A eficácia da skill não é subjetiva. Ela é medida por:
- **Score da Rubrica:** Meta de >24/30 pontos.
- **Compliance Checklist:** 100% de aprovação nos critérios bloqueantes do DoD.

---

## 🛠️ Como Estender

Para adicionar suporte a um novo evento (ex: **STB - Simpósio de Teste de Software**):
1. Crie uma nova referência em `references/` com as regras específicas do evento.
2. Atualize o workflow `select-venue.md` para incluir os critérios de aceitação desse novo alvo.
