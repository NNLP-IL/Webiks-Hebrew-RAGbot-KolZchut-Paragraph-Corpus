# Webiks-Hebrew-RAGbot-KolZchut-Paragraph-Corpus
* This repo contains a corpus of all paragraphs in the [Kol-Zchut](https://www.kolzchut.org.il/) website.
* The file: [`Webiks_Hebrew_RAGbot_KolZchut_Paragraphs_Corpus_v1.0.json`](https://drive.google.com/file/d/18hAihDl0NlBz4EFubSnN7YMwL4v58qP_/view?usp=drive_link) is the paragraph corpus used to train the [`Webiks_Hebrew_RAGbot_KolZchut_QA_Embedder`](https://drive.google.com/file/d/1eFAddJWBWDvoid-Gyn6ZT5jPwf-vNPI8/view?usp=drive_link) model. You can see how to use it in order to train this model in the following [`repository`](https://github.com/NNLP-IL/Webiks-Hebrew-RAGbot-Trainer). Each entry in this corpus is a paragraph. It contains all relevant paragraphs from the Kol-Zchut website, extracted by splitting the Kol-Zchut webpages according to their HTML titles, and then combining paragraphs up to the maximum context size of the me5-large model, which is 512 tokens.

## Fields
* `doc_id`: The unique identifier of the website page.
* `title`: The title of the website page.
* `link`: The website page link.
* `content`: This is the paragraph in the page.
* `license`: The license under which the file is published.

## Notes
* The corpus was extracated from the KolZchut website in May 2024 and is not necessarily up to date with today's website.

## License
This data is published under Creative Commons Attribution-NonCommercial-ShareAlike 2.5 license.
<br>
More info: https://creativecommons.org/licenses/by-nc-sa/2.5/
