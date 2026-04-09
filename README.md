# 🎓 SBC Article AI Skill

**Um ecossistema inteligente de workflows para auxílio na criação, estruturação e revisão de artigos acadêmicos seguindo rigorosamente os padrões da Sociedade Brasileira de Computação (SBC).**

[![AI Powered](https://img.shields.io/badge/AI-Powered-blue.svg)](#architecture)
[![Standard](https://img.shields.io/badge/Standard-SBC%20Template-green.svg)](https://www.sbc.org.br/documentos-e-publicacoes/templates-para-artigos-e-capitulos-de-livros)
[![Ethics](https://img.shields.io/badge/Ethics-Researcher%20First-red.svg)](#-aviso-de-integridade-acadêmica)

---

### ⚠️ AVISO DE INTEGRIDADE ACADÊMICA

**Esta skill foi desenvolvida para atuar como um Copiloto Normativo e Consultor de Estrutura. Ela NÃO deve ser utilizada para gerar artigos inteiros de forma autônoma.**

A autoria científica exige responsabilidade, análise crítica e originalidade que apenas o pesquisador humano pode prover. O uso desta ferramenta deve focar em:
1.  **Suporte à Estruturação:** Organizar suas ideias e dados reais no fluxo IMRaD.
2.  **Conformidade Normativa:** Garantir que as normas da SBC e LaTeX sejam seguidas.
3.  **Melhoria de Fluidez:** Revisar gramática e estilo acadêmico de textos escritos por você.
4.  **Descoberta de Gaps:** Identificar onde sua argumentação precisa de mais provas ou referências.

**O pesquisador é o único responsável pelo conteúdo, veracidade dos dados e conclusões do trabalho.** Nunca submeta um texto gerado por IA sem revisão humana exaustiva.

---

## 🚀 Funcionalidades de Suporte

- **Orquestração de Workflows:** 7 pipelines que guiam o pesquisador por cada fase da escrita (Kickoff, Organização, Escrita, Evidência, LaTeX, Validação, Seleção de Venue).
- **Consultoria Normativa:** Aplicação automática das normas SBC (margens, fontes, citações, estrutura).
- **Garantia de Qualidade (DoD):** Sistema de *Definition of Done* que ajuda o autor a verificar se não esqueceu requisitos críticos de submissão.
- **Diretrizes de Integridade:** Guidelines integrados que ensinam o agente de IA a agir como revisor crítico, e não como gerador passivo.
- **Estratégias de Embasamento:** Métodos estruturados para auxiliar o pesquisador a encontrar evidências reais em bases científicas.

---

## 🏗️ Arquitetura da Skill

A skill segue o padrão de **Divulgação Progressiva**, mantendo o contexto do agente limpo e carregando conhecimento sob demanda.

### Estrutura de Diretórios

```
sbc-article/
├── SKILL.md                # Cérebro: Instruções mestres e roteamento
├── references/             # Base de Conhecimento (Domain Knowledge)
│   ├── sbc-standards.md    # Normas técnicas da SBC
│   ├── academic-writing.md # Estilo e gramática acadêmica
│   └── ...                 # Guias de citações, QUALIS e ética
├── workflows/              # Procedimentos Operacionais (Workflows)
│   ├── kickoff-article.md  # Início estruturado de projetos
│   ├── write-section.md    # Auxílio na escrita modular de seções
│   └── ...                 # Validação, LaTeX e busca de provas
└── templates/              # Artefatos e Ferramentas de Medição
    ├── dod-checklist.md    # Critérios de aceitação binários
    └── quality-rubric.md   # Avaliação multidimensional (Score 1-5)
```

---

## 🛠️ Instalação e Uso

### Pré-requisitos
- **Claude Code** ou **Gemini CLI** instalado.
- Ambiente configurado com suporte a **LaTeX** (opcional, para renderização final).

### Instalação (Manual)
1. Clone este repositório no diretório de skills do seu agente:
   ```bash
   cd ~/.claude/skills # ou caminho equivalente
   git clone https://github.com/seu-usuario/sbc-article.git
   ```

### Como usar
Ative a skill pedindo ajuda para estruturar ou revisar um artigo:
> *"Ajude-me a organizar meus resultados experimentais no padrão de seção da SBC."*

---

## 📊 Métricas de Qualidade

Diferente de ferramentas de "geração rápida", esta skill aplica critérios de rigor científico:

### Definition of Done (DoD)
Um trabalho é considerado "Apto para Revisão Final" apenas se:
1. Seguir 100% dos critérios do `templates/dod-checklist.md`.
2. **Todas** as referências forem verificadas pelo autor humano como existentes e pertinentes.
3. Os dados apresentados forem fruto de pesquisa real, não simulações de IA.

---

## 🤝 Contribuição

Interessado em adicionar templates para eventos específicos da SBC (ex: SBES, SIBGRAPI)? 
Consulte o arquivo `CONTRIBUTING.md`.

---

## 📄 Licença

Distribuído sob a licença MIT. Veja `LICENSE` para mais informações.
