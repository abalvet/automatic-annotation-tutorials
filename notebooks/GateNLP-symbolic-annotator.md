# Annotating elements with GateNLP

## Symbolic approaches to data annotation

Before the generalization of corpus-derived statistical and neural models around the 1990's, NLP mainly relied on what were called **symbolic** approaches.  The term ```symbolic``` refers to a range of strategies relying on explicit knowledge for data processing. 
Explicit knowledge can be translated into either lexical resources (lists of elements, eg.: list of places) or pattern-matching rules. 

### Lexical resources 

**Lexical resources** are essentially lists of words associated to a set of features, for example:

  - lemma (eg.: "shouted" -> "shout")
  - morphological properties (eg.: "shouted" -> preterit, "shouts" -> present, 3rd person, singular)
  - part-of-speech (eg.: "shouted" -> VERB)
  - category (eg.: "John" -> PER, "Paris" -> LOC)

Such lists are easy to set up (especially now that we have tons of web content available), matching elements in a text based on those lists is essentially a lookup function, which can be optimized (compression, hashing, caching, etc.). Using a lexical resource is therefore a straightforward process, which requires no computationally-intensive Machine Learning steps. Lexical resources typically yield high precision in specialized domains (eg.: medical texts), but require a lot of manual work (editing, updating, and overall maintenance). They are still a valid approach in specialized domains or whenever Machine Learning is not applicable (eg.: under-resourced languages).

### Pattern-matching rules 

Rules can be used:
 - to identify sentence and token boundaries based on explicit typographic cues (separators)
 - to match certain words (words with a given suffix, like "-er", words starting with a capital letter).

In principle, rules can not only be used in a "search" mode, but also in a "search-and-replace" mode. Search-and-replace can be used to actually segment (split) a raw text file into basic linguistic units, using explicit marks (eg.: space, carriage return, special character) or even markup (YAML, XML, etc.). 

Pattern-matching rules can be used at multiple points in a text-processing pipeline. 

### Hands-on tutorial based on GateNLP

[![Open In Colab](https://colab.research.google.com/assets/colab-badge.svg)]([https://colab.research.google.com/github/googlecolab/colabtools/blob/master/notebooks/colab-github-demo.ipynb](https://colab.research.google.com/drive/1xYVPw4qhoq5ftQ4XxzGSw2xEI1GgCRwX?usp=sharing))
