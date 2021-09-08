# Refactored MIDD dataset for Named Entity Recognition (NER) on Invoice documents 

Attempt to merge all `.csv` files of the MIDD dataset into a single file stored in the JSON format.

The refactored dataset is available in 2 versions depending on wether we want to convert the string `ner_tag` into integers.

Each row of the final dataset corresponds to a CSV-document in the MIDD dataset and is stored as a JSON object with the following schema :

```python
{
    "name": <file_name>,
    "layout":<layout_id>,
    'ner_tag':[
        <tag 1>,
        <tag 2>,
        ...
        <tag n>,
    ],
    'token':[
        <token 1>,
        <token 2>,
        ...
        <token n>,
    ]
}
```

# Citation

```BibTeX
@Article{data6070078,
AUTHOR = {Baviskar, Dipali and Ahirrao, Swati and Kotecha, Ketan},
TITLE = {Multi-Layout Invoice Document Dataset (MIDD): A Dataset for Named Entity Recognition},
JOURNAL = {Data},
VOLUME = {6},
YEAR = {2021},
NUMBER = {7},
ARTICLE-NUMBER = {78},
URL = {https://www.mdpi.com/2306-5729/6/7/78},
ISSN = {2306-5729},
ABSTRACT = {The day-to-day working of an organization produces a massive volume of unstructured data in the form of invoices, legal contracts, mortgage processing forms, and many more. Organizations can utilize the insights concealed in such unstructured documents for their operational benefit. However, analyzing and extracting insights from such numerous and complex unstructured documents is a tedious task. Hence, the research in this area is encouraging the development of novel frameworks and tools that can automate the key information extraction from unstructured documents. However, the availability of standard, best-quality, and annotated unstructured document datasets is a serious challenge for accomplishing the goal of extracting key information from unstructured documents. This work expedites the researcher’s task by providing a high-quality, highly diverse, multi-layout, and annotated invoice documents dataset for extracting key information from unstructured documents. Researchers can use the proposed dataset for layout-independent unstructured invoice document processing and to develop an artificial intelligence (AI)-based tool to identify and extract named entities in the invoice documents. Our dataset includes 630 invoice document PDFs with four different layouts collected from diverse suppliers. As far as we know, our invoice dataset is the only openly available dataset comprising high-quality, highly diverse, multi-layout, and annotated invoice documents.},
DOI = {10.3390/data6070078}
}
```

