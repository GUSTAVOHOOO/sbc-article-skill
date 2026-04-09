<citation_methods>

<sbc_citation_style>
A SBC usa estilo próprio baseado em ABNT, mas com variações. Sempre confira o arquivo sbc.bst fornecido com o template do evento.

**No texto:**
- Citação narrativa: "Silva et al. [2023] propõem..."
- Citação parentética: "...conforme demonstrado na literatura [SILVA, 2023]"
- Múltiplas citações: "[SILVA, 2023; COSTA, 2022; LIMA, 2021]"

**Formato no texto com LaTeX:**
```latex
% Definindo no .bib e usando no texto:
\cite{silva2023}           % [Silva, 2023]
\cite{silva2023,costa2022} % [Silva, 2023; Costa, 2022]
```
</sbc_citation_style>

<bibtex_formats>
**Formatos BibTeX por tipo:**

**Artigo em periódico:**
```bibtex
@article{silva2023nlp,
  author  = {Silva, João Carlos and Costa, Maria Fernanda},
  title   = {Título Completo do Artigo},
  journal = {Journal of the Brazilian Computer Society},
  year    = {2023},
  volume  = {29},
  number  = {1},
  pages   = {1--20},
  doi     = {10.1007/xxx}
}
```

**Artigo em conferência SBC:**
```bibtex
@inproceedings{costa2022sbbd,
  author    = {Costa, Ana Paula},
  title     = {Título do Artigo de Conferência},
  booktitle = {Anais do XXXVII Simpósio Brasileiro de Banco de Dados},
  year      = {2022},
  pages     = {100--110},
  publisher = {SBC},
  address   = {Porto Alegre},
  doi       = {10.5753/sbbd.2022.xxx}
}
```

**Artigo IEEE/ACM:**
```bibtex
@inproceedings{lima2021ieee,
  author    = {Lima, Roberto and Santos, Paulo},
  title     = {Article Title},
  booktitle = {Proceedings of the IEEE International Conference on ...},
  year      = {2021},
  pages     = {1--8},
  publisher = {IEEE},
  doi       = {10.1109/xxx}
}
```

**Livro:**
```bibtex
@book{goodfellow2016,
  author    = {Goodfellow, Ian and Bengio, Yoshua and Courville, Aaron},
  title     = {Deep Learning},
  publisher = {MIT Press},
  year      = {2016},
  url       = {http://www.deeplearningbook.org}
}
```

**Capítulo de livro:**
```bibtex
@incollection{autor2020,
  author    = {Autor, Nome},
  title     = {Título do Capítulo},
  booktitle = {Título do Livro},
  editor    = {Editor, Nome},
  publisher = {Editora},
  year      = {2020},
  pages     = {10--30}
}
```

**Relatório técnico / Preprint:**
```bibtex
@techreport{devlin2018bert,
  author      = {Devlin, Jacob and Chang, Ming-Wei and Lee, Kenton and Toutanova, Kristina},
  title       = {{BERT}: Pre-training of Deep Bidirectional Transformers for Language Understanding},
  institution = {Google AI Language},
  year        = {2018},
  note        = {arXiv:1810.04805}
}
```
</bibtex_formats>

<citation_best_practices>
**Boas práticas:**

1. **Cite o artigo original do método**, não tutoriais ou posts de blog que explicam
2. **Chave BibTeX**: use padrão `sobrenome+ano+palavra` — ex: `silva2023bert`
3. **DOI sempre que disponível** — facilita verificação pelos revisores
4. **Acesso via CAPES**: se o artigo está atrás de paywall, acesse via Portal de Periódicos CAPES (VPN da universidade)
5. **Não cite sem ler**: ao menos leia abstract e contribuições antes de citar
6. **Evite autocitação excessiva**: máximo 20-30% das referências sendo do próprio grupo
7. **Equilibre nacional e internacional**: artigos SBC + IEEE/ACM mostra familiaridade com a área
</citation_best_practices>

<where_to_find>
**Onde encontrar referências:**

| Base | URL | Melhor para |
|------|-----|-------------|
| SBC OpenLib | sol.sbc.org.br | Artigos SBC (acesso livre) |
| Google Scholar | scholar.google.com | Busca ampla, ver citações |
| IEEE Xplore | ieeexplore.ieee.org | Computação, engenharia |
| ACM DL | dl.acm.org | Ciência da computação |
| Semantic Scholar | semanticscholar.org | AI, ML (acesso aberto) |
| arXiv | arxiv.org | Preprints recentes (cs.*) |
| CAPES Periódicos | periodicos.capes.gov.br | Acesso institucional completo |
| Connected Papers | connectedpapers.com | Descobrir trabalhos relacionados |

**Dica para trabalhos relacionados:** Use "Citado por" no Google Scholar para encontrar trabalhos que citam os mesmos artigos fundamentais da área — esses são seus trabalhos relacionados diretos.
</where_to_find>

</citation_methods>
