# HuRTE
This is the home repository for the Hungarian version of the Recognizing Textual Entailment datasets. This dataset is also part of the Hungarian Language Understanding Evaluation Benchmark Kit [HuLU](hulu.nlp.nytud.hu). The corpus was created by translating and re-annotating the instances of the RTE datasets that are part of the GLUE benchmark. 

## Data

The files are in the 'data' folder. The dataset contains 4 504 instances. These contain a (sometimes multi-sentence) premise and a one-sentence hypothesis, and the task is to decide whether the former entails the latter or not. The task is binary classification.

The train, validation and test sets contain 2 131, 242 and 2 131 instances, respectively. The test set is distributed without the labels; to evaluate your model please contact us (ligeti-nagy.noemi@nytud.hu) or visit [HuLU's website](hulu.nytud.hu) for an automatic evaluation. The metric of the evaluation is accuracy.

## Data format

The data files are in json format. The keys are the following:

`id`: unique id of the instances;

`premise`: the premise;

'hypothesis': the hypothesis;

`label`: "1", if the premise entails the hypothesis, "0" otherwise.


## License and usage

This work is licensed under a [Creative Commons Attribution-ShareAlike 4.0 International License](https://creativecommons.org/licenses/by-sa/4.0/).

## Citation

If you use this resource or any part of its documentation, please refer to:

Ligeti-Nagy, N., Ferenczi, G., Héja, E., Jelencsik-Mátyus, K., Laki, L. J., Vadász, N., Yang, Z. Gy. and Váradi, T. (2022) HuLU: magyar nyelvű benchmark adatbázis kiépítése a neurális nyelvmodellek kiértékelése céljából [HuLU: Hungarian benchmark dataset to evaluate neural language models]. In: Berend, G., Gosztolya, G. and Vincze, V. (eds), XVIII. Magyar Számítógépes Nyelvészeti Konferencia. Szeged, Szegedi Tudományegyetem, Informatikai Intézet. 431–446.

```
@inproceedings{ligetinagy2022hulu,
  title={HuLU: magyar nyelvű benchmark adatbázis kiépítése a neurális nyelvmodellek kiértékelése céljából},
  author={Ligeti-Nagy, N. and Ferenczi, G. and Héja, E. and Jelencsik-Mátyus, K. and Laki, L. J. and Vadász, N. and Yang, Z. Gy. and Váradi, T.},
  booktitle={XVIII. Magyar Számítógépes Nyelvészeti Konferencia},
  year={2022},
  pages = {431--446},
  editors = {Berend, G. and Gosztolya, G. and Vincze, V.},
  address = {Szeged},
  publisher = {Szegedi Tudományegyetem, Informatikai Intézet}
}
```
and 

Richard Socher, Alex Perelygin, Jean Wu, Jason Chuang, Christopher Manning, Andrew Ng and Christopher Potts (2013), Recursive Deep Models for Semantic Compositionality Over a Sentiment Treebank. In: Proceedings of the 2013 Conference on Empirical Methods in Natural Language Processing. 1631--1642.
```
@inproceedings{socher-etal-2013-recursive,
    title = "Recursive Deep Models for Semantic Compositionality Over a Sentiment Treebank",
    author = "Socher, Richard  and
      Perelygin, Alex  and
      Wu, Jean  and
      Chuang, Jason  and
      Manning, Christopher D.  and
      Ng, Andrew  and
      Potts, Christopher",
    booktitle = "Proceedings of the 2013 Conference on Empirical Methods in Natural Language Processing",
    month = oct,
    year = "2013",
    address = "Seattle, Washington, USA",
    publisher = "Association for Computational Linguistics",
    url = "https://www.aclweb.org/anthology/D13-1170",
    pages = "1631--1642",
}
