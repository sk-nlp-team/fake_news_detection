# Neural NLP Final Project: Fake News Detection

## Description:

This work is inspired by the article [The Surprising Performance of Simple Baselines for Misinformation Detection](https://arxiv.org/pdf/2104.06952.pdf).
In the project all the suggested approaches for automatic fake news detection were reproduced and tested on 3 main datasets: FakeNews, Celebrity, ReCOVery.
In addition, different preprocessing approaches were examined, cross-dataset experiments were conducted and also experiments on larger datasets (FakeNewsNet, NELA_GT_2018) were made to verify the quality of results.
Moreover, since the texts of the articles in our datasets are pretty long, we provide the experiments on Longformer model, which was designed to have long sequences of tokens (More than 1000. All other models have the restriction of 512 tokens) as an input.
And last but not least, we obtained the visualization of attention layers, which are the part of the majority of considered transformers, in order to get some understanding, what words are important for model to make a decision.


## Video description:
[Here](https://youtu.be/J0tVwP-ssb0) you can see our video presentation of the project.

## Report and presentation PDFs:

[Report](https://github.com/sk-nlp-team/misinformation_detection/blob/main/report.pdf)

[Presentation](https://github.com/sk-nlp-team/misinformation_detection/blob/main/report.pdf)

## Results for different models with Recovery dataset using Many Splits method:

| Model          | F1    | Recall | Precision |
| -------------- | ----- | ------ | --------- |
| Bert           | 0.756 | 0.784  | 0.784     |
| Bert-tiny      | 0.768 | 0.842  | 0.707     |
| RoBERTa        | 0.831 | 0.967  | 0.728     |
| ALBERT         | 0.712 | 0.703  | 0.737     |
| BERTWeet       | 0.811 | 0.891  | 0.745     |
| Covid twitter  | 0.829 | 0.989  | 0.713     |
| DeCLUTR        | 0.820 | 0.929  | 0.735     |
| Funnel Transf. | 0.779 | 0.808  | 0.751     |


## Many Splits loss on BERT on Recovery dataset:

<img src="https://github.com/sk-nlp-team/misinformation_detection/blob/main/images/loss_bert_many_splits.png" width=50% height=50%>



Authors: [Mikhail Kuimov](https://github.com/kmisterios), [Assel Yermekova](https://github.com/Allessyer), [Mikhail Filitov](https://github.com/lll-phill-lll), [Varvara Shushkova](https://github.com/shushkova)
----------
