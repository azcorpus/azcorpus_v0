

![](https://user-images.githubusercontent.com/31247506/229346998-1e08344b-26fc-4978-89f7-0ecba076fe25.png)

# azcorpus - The largest open-source NLP corpus for Azerbaijani (1.9M documents, ~ 18M sentences)

In recent years, deep learning models have been widely used in NLP, yielding excellent results. However, most research works in NLP have focused on high-resource languages such as English. There is a significant gap in NLP research for low- resource languages, Azerbaijani being no exception. So, the availability of adequate corpora for most of the languages is still limited, especially for less-resourced languages such as Azerbaijani. 

Therefore, this study aimed to contribute to the NLP research community by building the largest NLP corpus for Azerbaijani language.


## Corpus Summary

“azcorpus” built for text generation purposes contains a total of 1.9 million documents, drawn from a variety of sources. The corpus is designed to provide a broad range of linguistic data for natural language processing and organized by genre and topic, with texts covering a range of subjects including politics, economics, science, culture, sport, history, society and etc. 

Texts were selected from a variety of sources including newspapers, magazines, academic journals, wikipedia articles and books. The corpus includes both contemporary and historical texts, providing a rich linguistic and cultural context for natural language processing applications.

___

## Corpus structure


### Data fields

- id: Document id
- text - Newline-separated content
- source - Document source
- reliability - Subjective cleaning evaluation rate
- license - Document license

### Data Splits

This corpus has 3 sources(az_books, az_wiki, and az_news) and 1.876.492 cleaned documents. 


| Source name   | Number of Instances |     Size (GB)         |
| ------------- | --------------------|:----------------------|
| az_books      | 1,540,732           |      19.5             |
| az_wiki       | 98,882              |      0.9              |
| az_news       | 236,878             |      3.8              |

___

## Methodology

The first step in building "azcorpus" was to collect text data from various sources. 
The news websites were selected based on their popularity and the diversity of topics covered. 
Additionally, a collection of ebooks in Azerbaijani was obtained from various online sources. We have expanded our collection to encompass not only fictional literature, but also scholarly works, such as physics, chemistry, and etc.
Source-specific cleaning techniques were applied separately to ensure consistency and accuracy in the corpus. Further information regarding the methodolgy at hand will be expounded upon in our forthcoming academic paper.





To ensure the ethical use of the corpus, we only collected publicly available data, and we did not collect any personal or sensitive information. We also ensured that the corpus was used for research purposes only and not for commercial gain. In accordance with legal considerations, it is not within our current plans to divulge sources at this time.

___
## Corpus Usage 

To obtain comprehensive guidance on how to use "azcorpus", please refer to the detailed usage instructions provided in this notebook.

```python
corpus = AzCorpus(access_token = "your_token")

# To obtain a corpus in the raw JSON format
corpus.generate_samples()

```
The download of the entire corpus is a process that entails a time span of approximately 25 minutes to 2 hours, contingent upon the velocity of your internet connection. Presently, our team is engrossed in the refinement of the download script with the objective of enhancing efficiency.
___
## Considerations for Using the Corpus


#### Social Impact

Our work has the potential to contribute to the community by providing a valuable resource for development of new text generation tools in Azerbaijani.

"azcorpus" demonstrates the importance of building large NLP corpora for under-resourced languages, and highlights the social impact of such resources. By making this corpus available to the wider community, we hope to stimulate further research and development in the field of Azerbaijani text generation, and contribute to the broader goal of promoting linguistic diversity and cultural heritage. Future studies could explore the potential community impact of our work.

#### Biases and Limitations

Addressing potential bias in machine learning corpuses is a common concern in research.
In this study, we acknowledge that our dataset may be subject to bias and to mitigate this issue, we employed several techniques. 
However, we recognize that our approach may still have limitations.
So, It is important to exercise caution with models trained on a "azcorpus" that has not been adequately filtered,
as this may have an impact on the resulting models. In particular, it is crucial to be mindful of any biases 
that may be present in the "azcorpus_v0".

Future work could further investigate these issues and explore additional 
methods to address bias in the corpus.
___

## Additional Information

#### Corpus authors

The corpus was put together by [Huseyn Kishiyev](https://www.linkedin.com/in/huseynkishiyev/), [Jafar Isbarov](https://www.linkedin.com/in/jafar-isbarov/), [Kanan Suleymanli](https://www.linkedin.com/in/kanan-suleyman/), [Khazar Heydarli](https://www.linkedin.com/in/xezer-heyderli/), [Leyla Eminova](https://www.linkedin.com/in/leyla-eminova/) and [Nijat Zeynalov](https://www.linkedin.com/in/nijat-zeynalov-064163142/).

The authors' names have been arranged in alphabetical order. All authors have equal rights and contributed equally to this work.


The authors declare no conflict of interest. There are no founding sponsors and no other role in the design of the work other than the authors; in the collection, analysis, or interpretation of data; in the writing of the manuscript, and in the decision to publish the corpus.

___
