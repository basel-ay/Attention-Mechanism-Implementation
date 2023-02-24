# Attention-Mechanism-Implementation

The attention mechanism was introduced to improve the performance of the encoder-decoder model for machine translation. The idea behind the attention mechanism was to permit the decoder to utilize the most relevant parts of the input sequence in a flexible manner, by a weighted combination of all the encoded input vectors, with the most relevant vectors being attributed the highest weights.

<p align="center">
  <img src="https://user-images.githubusercontent.com/64821137/220428391-fb72cd39-ce07-4dd1-b565-5821ecbddb17.png" />
</p>

The attention mechanism was introduced by Bahdanau et al. (2014) to address the bottleneck problem that arises with the use of a fixed-length encoding vector, where the decoder would have limited access to the information provided by the input. This is thought to become especially problematic for long and/or complex sequences, where the dimensionality of their representation would be forced to be the same as for shorter or simpler sequences.

## What is self-attention?

If you think that self-attention is similar, the answer is yes! They fundamentally share the same concept and many common mathematical operations.

A self-attention module takes in n inputs and returns n outputs. What happens in this module? In layman’s terms, the self-attention mechanism allows the inputs to interact with each other (“self”) and find out who they should pay more attention to (“attention”). The outputs are aggregates of these interactions and attention scores.

![image](https://user-images.githubusercontent.com/64821137/220429271-2186e2e4-899a-4aec-b3d2-26fbff81dcbf.png)


## Queries, Keys, and Values

The key/value/query concept is analogous to retrieval systems. For example, when you search for videos on Youtube, the search engine will map your query (text in the search bar) against a set of keys (video title, description, etc.) associated with candidate videos in their database, then present you the best matched videos (values).

The attention operation can be thought of as a retrieval process as well.

<p align="center">
  <img src="https://user-images.githubusercontent.com/64821137/220430122-ea844bfa-a26f-45fd-8851-f1eeb7a2b3f8.png" />
</p>

![image](https://user-images.githubusercontent.com/64821137/220433640-9638efe8-7010-4293-adf5-60d9b81e12ec.png)

