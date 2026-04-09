<full_article_template>

<!--
  TEMPLATE COMPLETO — Artigo SBC em LaTeX
  
  Copie e preencha os placeholders marcados com [PLACEHOLDER].
  Cada placeholder tem instrução sobre o que escrever.
  Remova os comentários de instrução após preencher.
-->

```latex
\documentclass[12pt]{article}

\usepackage{sbc-template}
\usepackage[brazil]{babel}
\usepackage[utf8]{inputenc}
\usepackage{graphicx,url}
\usepackage{amsmath}
\usepackage{booktabs}    % tabelas profissionais
\usepackage{algorithm2e} % algoritmos (se necessário)
\usepackage{hyperref}    % links clicáveis

% ============================================================
% METADADOS DO ARTIGO
% ============================================================

\title{
  [TÍTULO EM PORTUGUÊS]\\    % Ex: "Detecção de Anomalias em Séries Temporais com Transformers"
  \and
  [TITLE IN ENGLISH]         % Mesmo título em inglês
}

% Formato: Nome Completo\inst{N} — N corresponde à afiliação
\author{
  [Autor 1]\inst{1},
  [Autor 2]\inst{1},
  [Autor 3]\inst{2}
}

% Uma \address por afiliação
\address{
  [Departamento, Instituição, Cidade -- Estado, País]\\
  \email{\{[email1],[email2]\}@[dominio.br}}
  \nextinstitute
  [Segunda Instituição — se houver]\\
  \email{[email3]@[dominio2.br}}}
}

% ============================================================
% INÍCIO DO DOCUMENTO
% ============================================================
\begin{document}

\maketitle

% ============================================================
% ABSTRACT (inglês) — máx. 10 linhas / 200 palavras
% Estrutura: Contexto → Problema → Proposta → Método → Resultado → Impacto
% ============================================================
\begin{abstract}
  [CONTEXTO: 1-2 frases sobre a área e relevância geral.]
  [PROBLEMA: 1 frase identificando o gap ou desafio específico.]
  [PROPOSTA: 1 frase com verbo de ação — "This paper proposes / presents / introduces..."]
  [MÉTODO: 1 frase sobre a abordagem utilizada.]
  [RESULTADO: 1 frase com o resultado principal e métrica — "achieved X% improvement over baseline Y".]
  [IMPACTO: 1 frase sobre implicações ou contribuição para a área.]
\end{abstract}

% ============================================================
% RESUMO (português) — máx. 10 linhas / 200 palavras
% Tradução/adaptação do Abstract — NÃO é tradução literal automática
% ============================================================
\begin{resumo}
  [CONTEXTO em PT: 1-2 frases.]
  [PROBLEMA em PT: 1 frase.]
  [PROPOSTA em PT: "Este artigo propõe / apresenta / introduz..."]
  [MÉTODO em PT: 1 frase.]
  [RESULTADO em PT com métrica.]
  [IMPACTO em PT.]
\end{resumo}

% ============================================================
% SEÇÃO 1 — INTRODUÇÃO
% Estrutura: Contexto → Problema → Motivação → Contribuições → Organização
% Meta: 4-6 parágrafos, ~1 página
% ============================================================
\section{Introdução}

% P1: Contexto amplo — área, por que é importante, tendências
[CONTEXTO AMPLO: Situe o leitor na área geral. Ex: "Com o crescimento exponencial de dados gerados por dispositivos IoT, técnicas de..."]

% P2: Problema específico — com evidência quantitativa se possível
[PROBLEMA ESPECÍFICO: Estreite para o problema concreto. Idealmente com dado/estatística. Ex: "No entanto, X% dos sistemas atuais falham em Y [AUTOR, ANO]..."]

% P3: Gap na literatura — o que não existe ou não funciona
[GAP: O que falta. "Embora existam abordagens para Z [AUTOR, ANO], nenhuma considera W, que é crítico em..."]

% P4: Contribuições (use lista numerada)
Este artigo apresenta as seguintes contribuições:
\begin{itemize}
  \item [CONTRIBUIÇÃO 1: específica e verificável — o que exatamente foi feito/proposto]
  \item [CONTRIBUIÇÃO 2: se houver]
  \item [CONTRIBUIÇÃO 3: se houver — máx. 4 contribuições]
\end{itemize}

% P5: Resultados principais (opcional, reforça impacto)
[RESULTADOS ANTECIPADOS: "Os experimentos demonstram que a abordagem proposta supera o estado da arte em X% nas métricas Y e Z."]

% P6: Organização do artigo
O restante deste artigo está organizado da seguinte forma: a Seção~\ref{sec:related} apresenta os trabalhos relacionados; a Seção~\ref{sec:method} descreve [NOME DA METODOLOGIA]; a Seção~\ref{sec:results} apresenta e discute os resultados; e a Seção~\ref{sec:conclusion} conclui o artigo.

% ============================================================
% SEÇÃO 2 — TRABALHOS RELACIONADOS
% Estrutura: Agrupados por abordagem, não cronológicos
% Meta: 1-2 páginas, grupos temáticos, fecha com diferenciação
% ============================================================
\section{Trabalhos Relacionados}
\label{sec:related}

% Introdução da seção — anuncia os grupos
[PANORAMA: "A literatura sobre [TEMA] pode ser organizada em três grupos principais: (i) [GRUPO 1], (ii) [GRUPO 2] e (iii) [GRUPO 3]."]

% Grupo 1 — métodos/abordagem mais próxima
\subsection*{[Nome do Grupo 1]}  % ou apenas parágrafo sem subsection
[GRUPO 1: 2-4 referências. Descreva a abordagem, cite resultados, aponte limitações. "Silva et al.~\cite{silva2023} propõem... No entanto, esta abordagem apresenta limitação X..."]

% Grupo 2
[GRUPO 2: idem]

% Grupo 3 (se houver)
[GRUPO 3: idem]

% Fechamento — diferenciação explícita do trabalho atual (OBRIGATÓRIO)
[DIFERENCIAÇÃO: "Diferentemente dos trabalhos apresentados, o presente artigo [COMO É DIFERENTE]. Especificamente, [DETALHE DO DIFERENCIAL]."]

% ============================================================
% SEÇÃO 3 — METODOLOGIA (ou Proposta / Desenvolvimento)
% Estrutura: Visão geral → Componentes → Dataset → Protocolo experimental
% Meta: 2-3 páginas, suficiente para replicação
% ============================================================
\section{[Metodologia / Proposta / Nome do Sistema]}
\label{sec:method}

% Visão geral com figura de arquitetura (recomendado)
[VISÃO GERAL: "A Figura~\ref{fig:arch} apresenta uma visão geral da abordagem proposta. O método consiste em [N] etapas principais: [LISTA]."]

\begin{figure}[ht]
  \centering
  \includegraphics[width=0.9\columnwidth]{figuras/[nome-figura]}
  \caption{[LEGENDA AUTOEXPLICATIVA: O que a figura mostra, incluindo o que cada elemento/cor/símbolo representa.]}
  \label{fig:arch}
\end{figure}

% Componente 1 — descreva cada etapa/módulo
\subsection{[Etapa 1]}
[DESCRIÇÃO TÉCNICA: O que faz, como funciona, decisões de design e justificativas.]

% Componente 2
\subsection{[Etapa 2]}
[DESCRIÇÃO TÉCNICA]

% Dataset
\subsection{Configuração Experimental}

\textbf{Dataset:} [NOME DO DATASET]. [DESCRIÇÃO: número de instâncias, features, fonte/origem, características relevantes (balanceamento, período de coleta, licença).] O dataset está disponível em [URL/referência].

\textbf{Baselines:} Foram selecionados os seguintes métodos de comparação: (i)~[BASELINE 1]~\cite{ref}: [1 frase de justificativa por que este baseline é relevante]; (ii)~[BASELINE 2]~\cite{ref}: [justificativa].

\textbf{Métricas:} O desempenho foi avaliado por [MÉTRICA 1] e [MÉTRICA 2], [JUSTIFICATIVA: por que estas métricas são adequadas para o problema].

\textbf{Protocolo:} [VALIDAÇÃO CRUZADA / TRAIN-TEST SPLIT / etc. com proporções]. A semente aleatória utilizada foi [N] para reprodutibilidade. Todos os experimentos foram executados em [HARDWARE: CPU/GPU, RAM] com [SO e versão] e [bibliotecas + versões].

% ============================================================
% SEÇÃO 4 — RESULTADOS (ou Avaliação / Experimentos)
% Estrutura: Dados antes de interpretação, tabelas + figuras, análise
% Meta: 2-3 páginas
% ============================================================
\section{Resultados e Discussão}
\label{sec:results}

% Tabela de resultados principais (padrão: caption ACIMA da tabela)
A Tabela~\ref{tab:results} apresenta os resultados comparativos dos métodos avaliados.

\begin{table}[ht]
  \caption{[LEGENDA ACIMA: Comparação de [MÉTRICA] entre os métodos avaliados no dataset [NOME]. Melhor valor em \textbf{negrito}.]}
  \label{tab:results}
  \centering
  \begin{tabular}{lccc}
    \toprule
    \textbf{Método} & \textbf{[Métrica 1]} & \textbf{[Métrica 2]} & \textbf{[Métrica 3]} \\
    \midrule
    [Baseline 1]     & XX.X & XX.X & XX.X \\
    [Baseline 2]     & XX.X & XX.X & XX.X \\
    \midrule
    [Método Proposto] & \textbf{XX.X} & \textbf{XX.X} & \textbf{XX.X} \\
    \bottomrule
  \end{tabular}
\end{table}

% Análise dos resultados
[ANÁLISE 1: Descreva o resultado principal. "A abordagem proposta obteve [X]% em [Métrica], superando o melhor baseline em [Y]%."]

[ANÁLISE 2: Explique POR QUE os resultados são assim. "Este ganho pode ser atribuído a [RAZÃO TÉCNICA]."]

[ANÁLISE 3: Discuta casos onde o método não foi melhor (se houver). Honestidade aumenta credibilidade.]

% Análise estatística (quando aplicável)
[SIGNIFICÂNCIA: "Para verificar a significância estatística dos resultados, foi aplicado o teste [NOME] (p < 0,05). Os resultados confirmam/não confirmam [hipótese]."]

% ============================================================
% SEÇÃO 5 — CONCLUSÃO
% Estrutura: Síntese → Limitações → Trabalhos Futuros → Impacto
% Meta: 3-4 parágrafos, ~0.5 página
% ============================================================
\section{Conclusão}
\label{sec:conclusion}

% P1: Síntese (NÃO repita a Introdução — sintetize o que foi DESCOBERTO)
[SÍNTESE: "Este artigo apresentou [NOME/PROPOSTA], uma abordagem para [PROBLEMA]. Os experimentos demonstraram que [RESULTADO PRINCIPAL COM MÉTRICA], evidenciando [CONCLUSÃO TÉCNICA]."]

% P2: Resposta ao objetivo
[OBJETIVO RESPONDIDO: "O objetivo de [OBJETIVO DA INTRODUÇÃO] foi atingido ao [COMO FOI ATINGIDO]."]

% P3: Limitações (obrigatório — revisores respeitam honestidade)
[LIMITAÇÕES: "Este trabalho apresenta algumas limitações. [LIMITAÇÃO 1: específica]. [LIMITAÇÃO 2]."]

% P4: Trabalhos futuros (concretos, não genéricos)
[TRABALHOS FUTUROS: "Como trabalhos futuros, pretende-se [AÇÃO CONCRETA 1], bem como [AÇÃO CONCRETA 2]. Adicionalmente, [AÇÃO CONCRETA 3]."]

% ============================================================
% AGRADECIMENTOS (opcional)
% ============================================================
\section*{Agradecimentos}
[Se houver: agência de fomento, processo, bolsa. "Este trabalho foi parcialmente financiado pela [AGÊNCIA] (processo [N])."]

% ============================================================
% REFERÊNCIAS
% Use o estilo SBC: \bibliographystyle{sbc}
% ============================================================
\bibliographystyle{sbc}
\bibliography{referencias}  % arquivo referencias.bib

\end{document}
```

---

## ARQUIVO referencias.bib — MODELOS DE ENTRADA

```bibtex
% Artigo em periódico
@article{silva2023,
  author    = {Silva, João and Costa, Maria},
  title     = {[Título do artigo]},
  journal   = {[Nome do periódico]},
  year      = {2023},
  volume    = {15},
  number    = {3},
  pages     = {100--115},
  doi       = {10.XXXX/XXXXX}
}

% Artigo em conferência (proceedings)
@inproceedings{santos2022,
  author    = {Santos, Pedro and Oliveira, Ana},
  title     = {[Título do artigo]},
  booktitle = {Proceedings of the [Nome do Evento] ([SIGLA])},
  year      = {2022},
  pages     = {45--56},
  publisher = {SBC},
  address   = {Porto Alegre, RS, Brasil}
}

% Livro
@book{goodfellow2016,
  author    = {Goodfellow, Ian and Bengio, Yoshua and Courville, Aaron},
  title     = {Deep Learning},
  publisher = {MIT Press},
  year      = {2016},
  url       = {http://www.deeplearningbook.org}
}

% Capítulo de livro
@incollection{lecun1998,
  author    = {LeCun, Yann and Bottou, Léon},
  title     = {[Título do capítulo]},
  booktitle = {[Título do livro]},
  editor    = {[Editor]},
  publisher = {[Editora]},
  year      = {1998},
  pages     = {5--50}
}

% Preprint (usar apenas quando necessário — preferir versão publicada)
@misc{vaswani2017,
  author    = {Vaswani, Ashish and others},
  title     = {Attention Is All You Need},
  year      = {2017},
  eprint    = {1706.03762},
  archivePrefix = {arXiv}
}
```

---

## DICAS DE COMPILAÇÃO

```bash
# Ordem obrigatória para referências funcionarem:
pdflatex artigo.tex
bibtex artigo
pdflatex artigo.tex
pdflatex artigo.tex

# Ou com latexmk (automatiza):
latexmk -pdf artigo.tex
```

**Erros comuns e soluções:**

| Erro | Causa | Solução |
|---|---|---|
| `! LaTeX Error: File 'sbc-template.sty' not found` | Template não está na pasta | Copiar `sbc-template.sty` para a pasta do projeto |
| `Citation 'X' on page Y undefined` | BibTeX não rodou | Rodar na ordem correta acima |
| `! Package inputenc Error: Unicode char` | Encoding errado | Usar `\usepackage[utf8]{inputenc}` |
| Figura não aparece | Caminho errado | Verificar pasta `figuras/` e nome do arquivo |
| Tabela com legenda abaixo | Não seguiu padrão SBC | `\caption{}` deve vir ANTES de `\begin{tabular}` |

</full_article_template>
