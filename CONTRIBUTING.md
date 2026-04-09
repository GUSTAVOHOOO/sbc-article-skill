# 🤝 Contribuindo com a SBC Article AI Skill

Primeiramente, obrigado por dedicar seu tempo para contribuir! 🎉

Este repositório visa criar o copiloto definitivo para pesquisadores brasileiros. Para manter o rigor científico e a integridade da ferramenta, seguimos um conjunto de regras rigorosas para contribuições.

---

## ⚖️ Código de Conduta

Ao participar deste projeto, você concorda em manter um ambiente acolhedor, inclusivo e livre de assédio. Valorizamos o debate técnico fundamentado e o respeito mútuo.

---

## 🛠️ Como Posso Contribuir?

### 1. Adicionando Templates de Eventos
A SBC possui dezenas de simpósios (SBES, SIBGRAPI, IHC, etc.). Você pode contribuir criando sub-templates em `templates/` ou referências específicas em `references/` para um evento que você conhece bem.

### 2. Melhorando a Base de Conhecimento
Encontrou uma norma desatualizada ou uma técnica de escrita acadêmica melhor? Edite os arquivos na pasta `references/`.

### 3. Otimizando Workflows
Se você percebeu que a IA se "perde" em algum passo do kickoff ou da validação, sinta-se à vontade para propor melhorias na lógica dos arquivos em `workflows/`.

---

## 📜 Regras de Design da Skill

Para que sua contribuição seja aceita, ela deve seguir estes princípios:

1.  **Divulgação Progressiva:** Não coloque instruções gigantescas no `SKILL.md`. Use-o como roteador e coloque o detalhamento em arquivos específicos nas pastas `references/` ou `workflows/`.
2.  **Anti-Alucinação:** Todo novo workflow que envolva referências deve incluir passos de verificação obrigatórios.
3.  **Rigor Linguístico:** Templates de texto devem seguir o português formal acadêmico (voz ativa, terceira pessoa).
4.  **Determinismo:** Prefira tabelas de decisão e checklists binários em vez de descrições vagas.

---

## 🚀 Processo de Pull Request

1.  **Fork** o repositório.
2.  Crie uma **Branch** para sua modificação:
    ```bash
    git checkout -b feat/novo-template-sbes
    # ou
    git checkout -b fix/norma-citacao-abnt
    ```
3.  **Commits Convencionais:** Use o padrão [Conventional Commits](https://www.conventionalcommits.org/):
    - `feat:` para novas funcionalidades ou templates.
    - `fix:` para correções de normas ou bugs de roteamento.
    - `docs:` para melhorias na documentação.
4.  **Validação:** Se você alterou um workflow, teste-o com seu agente de IA local e anexe um log curto (ou screenshot) do comportamento no PR.
5.  Abra o **Pull Request** detalhando o "porquê" da mudança e como ela ajuda o pesquisador.

---

## 🏗️ Padrão de Arquivos

- **Workflows (`.md`):** Devem começar com as tags `<workflow_name>` e ter objetivos claros.
- **Referências (`.md`):** Devem ser baseadas em fontes oficiais (cite o link da SBC quando possível).
- **Templates (`.md`):** Devem usar placeholders claros (ex: `[INSIRA AQUI SEU PROBLEMA]`).

---

## 💎 Check de Qualidade (DoD do Contribuidor)

Antes de enviar seu PR, verifique:
- [ ] O arquivo `SKILL.md` continua com menos de 500 linhas?
- [ ] As novas instruções evitam que a IA invente dados?
- [ ] O novo template segue o arquivo `.sty` oficial da SBC?
- [ ] O Markdown está bem formatado e sem erros gramaticais?

---

Dúvidas? Abra uma **Issue** ou entre em contato com os mantenedores. Vamos construir o futuro da pesquisa brasileira juntos! 🚀
