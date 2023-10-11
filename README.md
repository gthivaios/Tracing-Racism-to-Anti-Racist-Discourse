# Tracing-Racism-to-Anti-Racist-Discourse
TRACE: “Tracing Racism to Anti-Racist Discourse: A critical approach to European public speech on the migrant and refugee crisis” (TRACE/HFRI-FM17-42, HFRI 2019-2022) [TRACE](https://traceprojectwiki.miraheze.org/wiki/%CE%91%CF%81%CF%87%CE%B9%CE%BA%CE%AE_%CF%83%CE%B5%CE%BB%CE%AF%CE%B4%CE%B1)

## Project Description

This project focuses on institutionalized/ official anti-racist discourse of the European public sphere, which refers to the migration and refugee issue. The mass migration and refugee movements in Europe from 2015 onwards and the ensuing intense discussions at a global level led to the rise of different stances and practices on behalf of European states, ranging from solidarity to xenophobia. In this context, this research program intends to reveal that racist views are not cultivated only through hate speech, which stigmatizes and overtly demonizes migrant and refugee populations, but also through seemingly anti-racist discourse, which aims at denouncing racist practices, but ends up disguising, reproducing and sedimenting inequalities.

To this end, the first aim is the creation of a corpus of anti-racist (multimodal) texts including, on the one hand, media texts such as advertising campaigns, news articles, TV shows, cartoons, and, on the other, institutional texts such as educational material, parliamentary proceedings, and other political and legal texts, which circulate in European countries. This corpus will be annotated and analyzed in order to detect texts indirectly perpetuating social and/or sociolinguistic inequalities: what we tentatively call ‘racist’ anti-racist texts. More specifically, drawing on Critical Discourse Analysis, the analysis concerns the various linguistic and other semiotic strategies through which racist views infiltrate discourse intended as anti-racist. Through the creation of a critical toolkit (TRACE) based on the findings of the analysis, the main intention is to enhance individuals’ critical awareness so as to be able to detect racism in anti-racist discourse. The ultimate goal of the program is to inform and sensitize the public, particularly educational and institutional bodies, on this kind of latent racism via the use of printed and audio-visual material.

## Implementation

Continuously to the above theoretical background, my thought was to make a text research analysis using nlp techniques for the already gathered texts that used for this project. We would like to make a preliminary visualization of the dataset we have created. Then we are doing the appropriate text preprocessind and finally we try to export some conclusions.

### Dataset

The dataset consists of a corpus of 78 greek anti-racist texts or text extracts, originating of 14 different sources of origin covering a wide range of the Greek public sphere, which are divided into basic categories:

- 64 texts of liquid racism
- 14 texts of pure antiracist texts(texts in which no categories of racism are found)

### Text Preprocessing

- Load the dataset
- Remove special characters
- Remove stopwords
- Lemmatization
- Word Frequency and Wordcloud
- TF-IDF Scoring

### Similarity heatmap

We created a similarity heatmap for the liquid racism text and the purely antiracist texts accordingly, using the spacy's library similarity metric. 

## Conclusions

Based on word frequency as this is captured in the wordcloud and on the tf-idf measure which indicates the word importance we can mention the following points:

- Regarding the texts of liquid racism, we notice that words referring to the nation-state ('χώρα(country)', 'Ελλάδα(Greece)') and words referring to a place of detention ('δομή(structure)') predominate.
- Regarding the purely anti-racist texts, we notice that words denoting care, collectivity and solidarity dominate ('παιδί(child)', 'κοινωνία(society)', 'φαγητό(food)', 'νερό(water)')

## Future Research Challenges

- Guidance with linguistic analysis in order to find specific phrase patterns that indicates the liquid racism or the pure antiracism speech.
- Due to the fact, we have an imbalanced dataset, it would be a good idea to run an unsupervised analysis and detect the smaller category as outliers.(https://medium.datadriveninvestor.com/unsupervised-outlier-detection-in-text-corpus-using-deep-learning-41d4284a04c8)
- Graph Based Represenation: Investigate the importance of a term into a whole corpus of documents by utilizing contemporary graph theory methods, such as community detection algorithms and node centrality measures.(https://link.springer.com/chapter/10.1007/978-3-030-49161-1_9)

## Used Tools/Technologies

- Python 3.5
- Spacy
- SKlearn
- Jupyter Notebook
