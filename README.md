# nlp-paper-summary

This repo contains the summary of following NLP papers.

<table border="0" align="center">
<tr>
    <td style="padding:15px;"><a href="#bert-vs-lstm">BERT-vs-LSTM</a></td>
    <td style="padding:15px;"><a href="#tinybert-distilling-bert-for-natural-language-understanding">TinyBERT</a></td>
    <td style="padding:15px;"><a href="#albert-a-lite-bert-for-self-supervised-learning-of-language-representations">ALBERT</a></td>
</tr>
</table>

## BERT-vs-LSTM

This paper talks about:

#### Give a small dataset, can we use a large pre-trained model like BERT and get better results than simple models?

<a href="bert-vs-lstm#bert-vs-lstm">Checkout the summary here</a>

## TinyBERT: Distilling BERT for Natural Language Understanding

This paper talks about:

#### BERT based models are usually computationally expensive and memory intensive, so it is difficult to effectively execute them on resource-restricted devices. How to reduce the size while keeping the performance drop to minimum?

TinyBERT is empirically effective and achieves more than **96%** the performance of teacher BERT(base) on GLUE benchmark, while being **7.5x smaller** and **9.4x faster** on inference.

<a href="tiny-bert#tinybert-distilling-bert-for-natural-language-understanding">Checkout the summary here</a>

## ALBERT: A Lite BERT for Self-Supervised Learning of Language Representations

This paper talks about:

#### Increasing model size while pretraining natural language representations often results in improved performance on downstream tasks. However, at some point further model increases become harder due to GPU/TPU memory limitations and longer training times. How to handle these issues?

ALBERT proposes two parameter reduction techniques to lower memory consumption and increase the training speed of BERT. It also proposes a self-supervised loss that focuses on modeling inter-sentence coherence, and show it consistently helps downstream tasks with multi-sentence inputs.

<a href="albert#albert">Checkout the summary here</a>

## Poor Man's BERT: Smaller and Faster Transformer Models

This paper talks about: 

#### NLP has recently been dominated by large-scale pre-trained Transformer models, where size does matter. Models such as BERT, XLNet, RoBERTa, etc. are now out of reach for researchers and practitioners without large GPUs/TPUs. How to reduce the model size that do not require model pretraining from scratch?

There are many ways to reduce the size of pre-trained models. Some notable approaches are: 

- Prune parts of the network after training
- Reduction through weight factorization and sharing (Albert)
- Compression through knowledge distillation (Distilbert, Tinybert)
- Quantization (Q-bert)

This work falls under the class of pruning methods.This paper question's whether it is necessary to use all layers of a pre-trained model in downstream tasks and propose straight-forward strategies to drop some layers from the neural network.

<a href="poor-man-bert##poor-mans-bert-smaller-and-faster-transformer-models">Checkout the summary here</a>