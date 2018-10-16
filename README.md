The *Cited Loci* project aims at extracting all bibliographic references pointing to classical (Greek and Latin) authors and their texts from the classics articles contained in [JSTOR](http://jstor.org).

## Technology

This project developed a citation mining solution consisting of four software components, working together to perform the extraction of references:
- the [Citation Extractor](https://github.com/mromanello/CitationExtractor), responsible for identifying the citation components within the stream of text
- the Citation Matcher, which assigns to each extracted reference a unique identifier, in the form of a CTS URN
- the [HuCit Knowledge Base](https://github.com/mromanello/hucit_kb), a database containing unique identifiers, abbreviations, and variant forms for classical authors and their works (used by Matcher and Extractor)
- the [Citation Parser](https://github.com/mromanello/CitationParser), which takes care of transforming reference scopes into a normalized form, suitable to be embedded into a CTS URN.



![tech architecture diagram](assets/img/tech.png)

## Applications

### Aeneid in JSTOR

[*Cited Loci of the Aeneid*](http://aeneid.citedloci.org/) is a proof of concept of how next-generation tools for retrieving bibliographic information could look like. More than five thousands articles that quote or refer to specific passages of Virgil's *Aeneid* are made searchable trough an intuitive interface. To build this, more than 12,000 canonical references to the *Aeneid* were extracted from over 5,700 journal articles in JSTOR using Cited Loci's technology.

Read more about this collaboration in [this blog post](https://labs.jstor.org/blog/#!cited_loci_of_the_aeneid-searching_through_jstors_content_the_classicists_way).

### EpiBau

Cited Loci's citation mining technology is currently being employed, in a collaboration with the [*Epische Bauformen*](https://www.epische-bauformen.uni-rostock.de/en/) project at the University of Rostock, to support the creation of an index of cited passages (*index locorum*) for the compendium [*Structures of Epic Poetry*](https://www.degruyter.com/view/product/475925). This publication in three volumes is edited by Prof. Christiane Reitz and Dr. Simone Finkmann, and will be published by De Gruyter.

### CHS OA Books

Thanks to a collaboration with Leonard Muellner, summer interns at [Harvard's Center for Hellenic Studies (CHS)](https://chs.harvard.edu) have been training Cited Loci's citation mining tools to index canonical references contained in the [Open Access books and monographs](https://chs.harvard.edu/CHS/article/display/1166.browse-online-publications) published by the centre.  

## Publications

- Romanello, M. 2019 (forthcoming). “Large-Scale Extraction of Canonical References: Challenges and Prospects.” In Pierazzo, E. and Cogitore, I. eds., *Digital Humanities and Antiquity. Humanités Numériques et Antiquité. Actes Du Colloque International, Grenoble 2-4 Septembre 2015*, 74–89 ([preprint](http://dx.doi.org/10.13140/RG.2.2.32634.59842)).

- Romanello, M. 2015. “From Index Locorum to Citation Network: An Approach to the Automatic Extraction of Canonical References and Its Applications to the Study of Classical Texts.” King’s College London. [doi:11858/00-1780-0000-002A-4537-A](http://dx.doi.org/11858/00-1780-0000-002A-4537-A).
