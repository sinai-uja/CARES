# CARES - A Corpus of Anonymised Radiological Evidences in Spanish 📑🏥
## Description
CARES is a high-quality text resource manually labeled with ICD-10 codes and reviewed by radiologists. These types of resources are essential for developing automatic text classification tools as they are necessary for training and fine-tuning our computational systems.

The CARES corpus has been manually annotated using the ICD-10 ontology, which stands for for the 10th version of the International Classification of Diseases. For each radiological report, a minimum of one code and a maximum of 9 codes were assigned, while the average number of codes per text is 2.15 with the standard deviation of 1.12.

The corpus was additionally preprocessed in order to make its format coherent with the automatic text classification task. Considering the hierarchical structure of the ICD-10 ontology, each sub-code was mapped to its respective code and chapter, obtaining two new sets of labels for each report. The entire CARES collection contains 6,907 sub-code annotations among the 3,219 radiologic reports. There are 223 unique ICD-10 sub-codes within the annotations, which were mapped to 156 unique ICD-10 codes and 16 unique chapters of the cited ontology.

As for the dataset train and test subsets, a stratified split was performed in order to guarantee that the number of labels in the test data is representative.

## Availability
The CARES corpus is available through HuggingFace: https://huggingface.co/datasets/chizhikchi/CARES

## Citation
Mariia Chizhikova, Pilar López-Úbeda, Jaime Collado-Montañez, Teodoro Martín-Noguerol, Manuel C. Díaz-Galiano, Antonio Luna, L. Alfonso Ureña-López, M. Teresa Martín-Valdivia,
*CARES: A Corpus for classification of Spanish Radiological reports*.
Computers in Biology and Medicine,
Volume 154,
2023,
106581,
ISSN 0010-4825.
https://doi.org/10.1016/j.compbiomed.2023.106581


```
@article{CHIZHIKOVA2023106581,
  title = {CARES: A Corpus for classification of Spanish Radiological reports},
  author = {Mariia Chizhikova
    and Pilar López-Úbeda
    and Jaime Collado-Montañez
    and Teodoro Martín-Noguerol
    and Manuel C. Díaz-Galiano
    and Antonio Luna
    and L. Alfonso Ureña-López
    and M. Teresa Martín-Valdivia},
  journal = {Computers in Biology and Medicine},
  volume = {154},
  pages = {106581},
  year = {2023},
  issn = {0010-4825},
  doi = {https://doi.org/10.1016/j.compbiomed.2023.106581},
  url = {https://www.sciencedirect.com/science/article/pii/S001048252300046X},
  keywords = {Biomedical natural language processing, Radiology report, Text classification, Medical corpus, ICD-10, Transformer language model, Spanish medical resource},
}
```
