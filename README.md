# Abstractive-Text-Summarization-for-Covid-19-Papers
Quintillions of data is generated on a daily basis and thousands of research papers and articles are published yearly. The Research Community today has to go through several such papers which will help them in their own research. Reading each and every document related to the subject is not humanly possible. This leads to the need of generating summaries of all the documents which will give the overview of the paper. Since manually generating summaries of all the documents is quite a tedious task, we resort to automated summarization using Deep Learning.

In this project, we aim to generate human-like summaries of Covid Research papers with the help of Abstractive Text Summarization using different transformer-based models. These are state-of-the-art models freely available on Huggingface. The models are :
1) T5 (' Text-to-Text Transfer Transformer ')
2) BART (' Bidirectional and Auto-Regressive Transformer ')
3) PEGASUS ('Pre-training with Extracted Gap-sentences for Abstractive SUmmarization Sequence-to-sequence models')

The validation of the generated summaries was done with the help of Rouge-Score metric.

To get better rouge-scores, we developed our own model  by finetuning the PEGASUS-large model on the CORD-19 (Covid-19 Open Research Data) dataset. This was done using an NVIDIA DGX STATION. The finetuned was then uploaded on Huggingface. The comparitive analysis of the four models is available in the code.

CORD-19 Dataset : https://huggingface.co/datasets/cord19

PEGASUS_COVID19 (Finetuned PEGASUS model): https://huggingface.co/suha1234/pegasus_covid19
