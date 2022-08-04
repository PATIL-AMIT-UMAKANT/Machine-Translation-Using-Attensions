# Machine-Translation-Using-Attensions


## The goal of this notebook is to introduce sequence to sequence language translation (seq2seq) and Attention mechanism.
The notebook deals with a sequence to sequence model for English to Hindi translation. After training the model one will be able to input a English sentence and get back its Hindi translation.

>RNNs are also capable of doing natural language translation, aka. machine translation. It involves two RNNs, one for the source language and one for the target language. One of them is called an encoder, and the other one decoder. The reason is that, the first one encodes the sentence into a vector and the second one converts the encoded vector into a sentence in target language. The decoder is a separete RNN. Given the encoded sentence, it produces the translated sentence in target language. Attention lets the decoder to focus on specific parts of the input sentence for each output word. This helps the input and output sentences to align with one another.

We obtained the dataset used from Kaggle: https://www.kaggle.com/aiswaryaramachandran/hindienglish-corpora

<h2> References: </h2>
<li></a> Sequence to Sequence Learning with Neural Networks (Research Publication)</li>
<li></a> https://www.tensorflow.org/tutorials/text/nmt_with_attention </li>
<li></a> Using stochastic computation graphs formalism for optimization of sequence-to-sequence model (Research Publication) </li>
</ul>
