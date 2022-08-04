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


## Encoder Decoder with Attention Model

> Encoder Decoder with Attention model is a general end-to-end approach to sequence learning that makes minimal assumptions on the sequence structure. It uses a multilayered Gated Recurrent Unit (GRU) to map the input sequence to a vector of a fixed dimensionality, and then another deep GRU to decode the target sequence from the vector.
<img src="https://www.researchgate.net/profile/Vlad_Zhukov2/publication/321210603/figure/fig1/AS:642862530191361@1530281779831/An-example-of-sequence-to-sequence-model-with-attention-Calculation-of-cross-entropy.png" width="800" alt="attention mechanism">

> A sequence to sequence model has two parts – an encoder and a decoder. Both the parts are practically two different neural network models combined into one giant network. the task of an encoder network is to understand the input sequence, and create a smaller dimensional representation of it. This representation is then forwarded to a decoder network which generates a sequence of its own that represents the output. The input is put through an encoder model which gives us the encoder output. Here, each input words is assigned a weight by the attention mechanism which is then used by the decoder to predict the next word in the sentence. We use Bahdanau attention for the encoder.

