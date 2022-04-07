# BERT-base-Turkish-QA

A custom Turkish question answering system made by fine-tuning BERTurk, which is a BERT base model transformer.

This project is made during our joint internship at SESTEK Speech Enabled Software Technologies with [@AybarsManav](https://github.com/AybarsManav).



## Model Comparison

| Base Models                  | Training Set        | Evalulation Set   | Results |       | Hyperparameters |                |            |               |
|------------------------------|---------------------|-------------------|---------|-------|-----------------|----------------|------------|---------------|
|                              |                     |                   |         |       |                 |                |            |               |
|                              |                     |                   | Exact   | F1    | epoch           | max_seq_length | doc_stride | learning_rate |
| best-base-turkish-128k-cased | whole_train_dataset | whole_dev_dataset | 62.48   | 81.60 | 2               | 512            | 128        | 3,00E-05      |
|                              | whole_train_dataset | okanvk_dev        | 62.48   | 81.66 | 2               | 512            | 128        | 3,00E-05      |
|                              | whole_train_dataset | tquad_dev         | 62.22   | 80.42 | 2               | 512            | 128        | 3,00E-05      |
|                              | whole_train_dataset | xquad.tr          | 45.89   | 66.37 | 2               | 512            | 128        | 3,00E-05      |
| best-base-turkish-128k-cased | Tquad_train         | whole_dev_dataset | 56.32   | 76.86 | 2               | 512            | 128        | 3,00E-05      |
|                              | Tquad_train         | okanvk_dev        | 56.31   | 76.87 | 2               | 512            | 128        | 3,00E-05      |
|                              | Tquad_train         | tquad_dev         | 57.40   | 78.68 | 2               | 512            | 128        | 3,00E-05      |
|                              | Tquad_train         | xquad.tr          | 41.76   | 60.83 | 2               | 512            | 128        | 3,00E-05      |
| best-base-turkish-128k-cased | Okanvk_train        | whole_dev_dataset | 60.37   | 80.53 | 2               | 512            | 128        | 3,00E-05      |
|                              | Okanvk_train        | okanvk_dev        | 60.37   | 80.63 | 2               | 512            | 128        | 3,00E-05      |
|                              | Okanvk_train        | tquad_dev         | 58.63   | 78.43 | 2               | 512            | 128        | 3,00E-05      |
|                              | Okanvk_train        | xquad.tr          | 46.38   | 70.74 | 2               | 512            | 128        | 3,00E-05      |
| XLM-R Base                   | whole_train_dataset | whole_dev_dataset | 54.60   | 76.83 | 2               | 512            | 128        | 3,00E-05      |
|                              | whole_train_dataset | okanvk_dev        | 54.68   | 76.94 | 2               | 512            | 128        | 3,00E-05      |
|                              | whole_train_dataset | tquad_dev         | 53.48   | 75.26 | 2               | 512            | 128        | 3,00E-05      |
|                              | whole_train_dataset | xquad.tr          | 42.27   | 61.72 | 2               | 512            | 128        | 3,00E-05      |
| Savasy QA (not base)         | Tquad_train         | tquad_dev         | 62.56   | 80.48 |                 |                |            |               |



## Authors

👤 **Aras Güngöre**

* LinkedIn: [@arasgungore](https://www.linkedin.com/in/arasgungore)
* GitHub: [@arasgungore](https://github.com/arasgungore)

👤 **Aybars Manav**

* LinkedIn: [@aybarsmanav](https://www.linkedin.com/in/aybarsmanav)
* GitHub: [@AybarsManav](https://github.com/AybarsManav)
