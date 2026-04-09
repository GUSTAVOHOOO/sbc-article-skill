# Workflow: Formatação LaTeX no Template SBC

<required_reading>
**Leia agora:**
1. references/sbc-standards.md
</required_reading>

<process>
## Passo 1: Verificar template

O template SBC usa `sbc-template.sty`. O documento começa com:

```latex
\documentclass[12pt]{article}
\usepackage{sbc-template}
\usepackage[brazil]{babel}
\usepackage[utf8]{inputenc}
\usepackage[T1]{fontenc}
\usepackage{graphicx,url}
```

Se o usuário não tem o template, indique para baixar em: sol.sbc.org.br (SBC OpenLib) — cada evento distribui junto com o CFP.

## Passo 2: Estrutura obrigatória do documento

```latex
\begin{document}

\title{Título do Artigo em Português\\
       Title of the Article in English}

\author{Autor Um\inst{1}, Autor Dois\inst{2}}

\address{Instituição Um\\
  Cidade -- Estado -- Brasil
  \nextinstitute
  Instituição Dois\\
  Cidade -- Estado -- Brasil
  \email{\{autor1\}@inst1.br, autor2@inst2.br}
}

\maketitle

\begin{abstract}
Abstract em inglês (150-200 palavras).
\end{abstract}

\begin{resumo}
Resumo em português (150-200 palavras).
\end{resumo}

\section{Introdução}
...

\section{Trabalhos Relacionados}
...

\section{Metodologia}
...

\section{Resultados}
...

\section{Conclusão}
...

\bibliographystyle{sbc}
\bibliography{referencias}

\end{document}
```

## Passo 3: Elementos comuns

### Figuras
```latex
\begin{figure}[ht]
\centering
\includegraphics[width=.5\textwidth]{figura.png}
\caption{Legenda da figura.}
\label{fig:nome}
\end{figure}

% Referenciar: como mostra a Figura~\ref{fig:nome}
```

### Tabelas
```latex
\begin{table}[ht]
\centering
\caption{Legenda da tabela (caption ANTES da tabela na SBC).}
\label{tab:nome}
\begin{tabular}{|l|c|r|}
\hline
\textbf{Coluna 1} & \textbf{Coluna 2} & \textbf{Coluna 3} \\
\hline
Dado A & 10 & 0.95 \\
Dado B & 20 & 0.87 \\
\hline
\end{tabular}
\end{table}
```

### Citações (com BibTeX)
```latex
% No texto:
\cite{silva2023}       % [Silva, 2023]
\cite{silva2023,costa2022}  % múltiplas

% No arquivo .bib:
@article{silva2023,
  author  = {Silva, João and Costa, Maria},
  title   = {Título do Artigo},
  journal = {Nome do Periódico},
  year    = {2023},
  volume  = {10},
  pages   = {1--15}
}
```

### Equações
```latex
\begin{equation}
  f(x) = \sum_{i=1}^{n} x_i^2
  \label{eq:nome}
\end{equation}
```

### Algoritmos
```latex
\usepackage{algorithm}
\usepackage{algorithmic}

\begin{algorithm}
\caption{Nome do Algoritmo}
\begin{algorithmic}[1]
\REQUIRE entrada
\ENSURE saída
\STATE inicializar variáveis
\FOR{cada item em lista}
  \IF{condição}
    \STATE ação
  \ENDIF
\ENDFOR
\RETURN resultado
\end{algorithmic}
\end{algorithm}
```

## Passo 4: Erros comuns e soluções

| Erro | Causa | Solução |
|------|-------|---------|
| Caracteres especiais quebrados | Encoding incorreto | Usar `\usepackage[utf8]{inputenc}` |
| Referências [?] | .bib não compilado | Rodar: `pdflatex → bibtex → pdflatex → pdflatex` |
| Figura deslocada | Float sem `[ht]` | Adicionar `[ht]` ou `[h!]` |
| Caption errado em tabela | Caption depois da tabela | Caption ANTES do `\begin{tabular}` |
| Texto cortado nas margens | Pacote babel ausente | Adicionar `\usepackage[brazil]{babel}` |

## Passo 5: Compilação

Ordem correta para referências funcionarem:
```bash
pdflatex artigo.tex
bibtex artigo
pdflatex artigo.tex
pdflatex artigo.tex
```

Com Overleaf: compilação automática — apenas certifique-se que o arquivo .bib está no projeto.

## Passo 6: Checklist final LaTeX

- [ ] Título em português E inglês
- [ ] Abstract em inglês + Resumo em português
- [ ] Afiliações corretas com `\inst{}`
- [ ] Figuras com legenda e `\label`
- [ ] Tabelas com caption ANTES e `\label`
- [ ] Todas as referências no .bib
- [ ] `\bibliographystyle{sbc}` declarado
- [ ] Compilou sem erros no pdflatex
</process>

<success_criteria>
- [ ] Estrutura do documento correto com sbc-template
- [ ] Elementos (figuras, tabelas, equações) formatados corretamente
- [ ] BibTeX configurado e referências funcionando
- [ ] Compilação sem erros
</success_criteria>
