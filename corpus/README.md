## **Short description**
We present a unique corpus of Russian legal documents. Corpus is based on documents available on rg.ru. Documents date from 2008 to 2022.

There are 3 versions of this dataset:
**Full corpus** - Filtered legal corpus (almost 2000 pairs). Specially edited for simplification. Contains 5 columns: Название документа,  Ссылка, Текст (оригинал документа), Комментарий РГ, Дата.
**Legal dataset 2023** - only text-comment pairs (without other columns). Available on Hugging Face: https://huggingface.co/datasets/marcus2000/legal_dataset2023    
**Unfiltered corpus** - Unfiltered legal corpus. Contains almost 3000 pairs of original doc and its comment that were available on rg.ru (Российская Газета). Also available in Kaggle - https://www.kaggle.com/datasets/athugodage/russian-legal-text-parallel-corpus


##**Context**
This dataset was proposed to train a model for Russian legal text simplification. This dataset has already helped to train GPT and [T5](https://github.com/Athugodage/RuLawSimplification/blob/main/trained_models/ru_t5_test(rouge_metrics).ipynb) models for this task, as well as in [Dynamic Topic Modelling](https://github.com/Athugodage/legal_dtm/blob/main/BERTopic_DTM_legal_docs.ipynb) task to analyze the history of Russian law from 2008 to 2022 .

We have collected our data from [Rossiyskaya Gazeta website](https://rg.ru/doc).  It's a Russian newspaper published by the Government of Russia. The daily newspaper serves as the official government gazette of the Government of the Russian Federation, publishing government-related affairs such as official decrees, statements and documents of state bodies, the promulgation of newly approved laws, Presidential decrees, and government announcements.
Rossiyskaya Gazeta provides legal text descriptions for common people called "comments". But these descriptions are made only for important documents, so while there are hundreds of thousands of legal documents in Russia, only a couple of thousands has a "comment". We used this "comment" as simplified version of the document.


##**Content**

Dataset has 5 columns: 
1. Название документа (Document Title)
2. Ссылка (Link to the original document)
3. Текст (Original document text)
4. Комментарий РГ (Rossiyskaya Gazeta comment)
5. Дата (Publication date) 

Overall there are 2963 pairs of original documents and simplified ones. Dataset contains documents from December 31, 2008 up to November 28, 2022 - thus it contains COVID-19-related laws as well as documents associated with the war in Ukraine. 

Example of original document text:
![2, 2](https://www.googleapis.com/download/storage/v1/b/kaggle-user-content/o/inbox%2F11047041%2Fb6eb66b83f6e880a6af3c0770b910028%2Foriginal.png?generation=1676085591921691&alt=media)
Example of Rossiyskaya Gazeta comment:
![2, 2](https://www.googleapis.com/download/storage/v1/b/kaggle-user-content/o/inbox%2F11047041%2Fac7b6df0b8f8903ed55a26b185c57d64%2Fsimplified.png?generation=1676085712692880&alt=media)
