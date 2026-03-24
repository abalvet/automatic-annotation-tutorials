# Automatic Annotation Tutorials

This repository provides a collection of tutorials for the manual and automatic annotation of textual data. It is designed for students and researchers in linguistics and related fields (eg.: sociology, Digital Humanities) who wish to explore Natural Language Processing (NLP) and Artificial Intelligence methods without requiring an advanced programming background.

The tutorials focus on practical approaches to identifying and structuring linguistic information in texts, with particular attention to text pre-processing (normalization, sentence boundaries detction, tokenization),  Named Entity Recognition,  syntactic annotation, and more ``semantic'' annotations such as polarity annotation, and co-reference chains.

The overall perspective of this project is to support the development of accessible, reusable, and well-structured linguistic resources in the context of corpus linguistics and Digital Humanities, in line with initiatives such as the Clarin network and the Corli consortium.

---

## Objectives

This repository aims to:

- introduce the main approaches to text annotation, from rule-based methods to machine learning and large language models
- provide hands-on notebooks that can be executed directly in a browser
- help users understand how linguistic knowledge can be formalized and operationalized
- support the creation of annotated corpora for research, teaching, and applied purposes
- promote a "coding for inclusion" approach, where computational tools are used to improve accessibility and understanding of language data

---

## Intended Audience

This material is intended for:

- Master's students in linguistics, especially those with limited programming experience
- researchers in corpus linguistics, lexicography, and Digital Humanities
- members of research infrastructures and consortia working with textual data
- anyone interested in learning how NLP and AI can be used to annotate and structure texts

No prior experience with Python is required. The notebooks are designed to be self-contained and progressively introduce key concepts.

---

## How to Use the Notebooks

All tutorials are provided as Jupyter notebooks and can be executed directly using Google Colab, without installing anything on your computer.

To open a notebook:

1. Navigate to the `notebooks/` directory
2. Click on the notebook you want to explore
3. Click on "Open in Colab" if available, or copy the notebook URL into https://colab.research.google.com

Once opened in Colab:

- run each cell in order using the "Run" button
- read the explanations provided in the text cells
- modify the examples to experiment with your own data

Each notebook includes installation steps for required libraries.

---

## Current Content

The repository currently includes:

- annotation with GateNLP using rule-based approaches
- gazetteer-based annotation for Named Entities such as dates and other expressions

Additional tutorials will be added progressively, including:

- regular expression based annotation
- rule-based annotation with spaCy (EntityRuler) 
- statistical and neural Named Entity Recognition
- weak supervision approaches (for example with Snorkel)
- annotation using large language models

---

## Pedagogical Approach

The tutorials are organized to illustrate a progression from simple to more complex methods:

1. symbolic approaches based on lexicons and rules
2. hybrid approaches combining rules and statistical models
3. machine learning and neural models
4. large language models as annotators

This progression allows users to understand not only how to use tools, but also the underlying principles and trade-offs of each approach.

---

## Repository Structure

automatic-annotation-tutorials/
│
├── notebooks/
│   ├── 01_gazetteer_gatenlp.ipynb
│
├── data/
│   ├── sample_texts/
│   ├── gazetteers/
│
├── utils/
│   ├── preprocessing.py
│   ├── evaluation.py
│
├── README.md



- `notebooks/` contains the main tutorials
- `data/` will include example corpora and gazetteers
- `utils/` will provide helper scripts when needed

---

## Requirements

The notebooks are designed to run in Google Colab. No local installation is required.

If you prefer to run them locally, you will need:

- Python 3
- standard NLP libraries such as spaCy, GateNLP, or others depending on the notebook

Each notebook specifies its own dependencies.

---

## License

This project is distributed under the Creative Commons Attribution - NonCommercial - ShareAlike 4.0 International License (CC BY-NC-SA 4.0).

You are free to share and adapt the material, provided that you:

- give appropriate credit
- do not use the material for commercial purposes
- distribute any modifications under the same license


---

## Acknowledgements and Context

This repository is developed within the context of teaching and research in linguistics, with a focus on corpus analysis, annotation practices, and digital methods.

It contributes to a broader effort to make NLP and AI techniques accessible to non-specialists, and to support the creation of structured linguistic data for research and education.

---

## Related Programs and Infrastructures

- Master in Linguistics: [Linguistique Informatique pour l’Inclusion et l’Accessibilité Numérique (LIIAN)](https://formation.univ-lille.fr/fr/offre-de-formation/master-lmd-XB/master-sciences-du-langage-MG002189/linguistique-informatique-pour-l-inclusion-et-l-accessibilite-numerique-MX002192.html)

- [CORLI (Consortium pour les Corpus, les Langues et les Interactions)](https://corli.huma-num.fr/fr/accueil-principal/)

- [CLARIN (European Research Infrastructure for Language Resources and Technology)](https://www.clarin.eu/)

- [ORTOLANG (Infrastructure for language resources)](https://www.ortolang.fr/fr/accueil/)

- [Huma-Num (Digital infrastructure for humanities and social sciences)](https://www.huma-num.fr/)
