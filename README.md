# eX-TDA-chbmit
Interpret a CNN trained on chbmit through TDA

### Inspired by [previous work by Simone Morettini](https://github.com/SMorettini/CNNs-on-CHB-MIT)

## How does this thing work?
1. Generate spectrogram images from chbmit
2. Train a CNN on those spectrogram images
3. Use TDA to explore the behaviour of the CNN

## Wait, what does it mean to explore the behaviour of a CNN, and with TDA?
Exploring the behaviour of a CNN means to produce explanations describing how a CNN classifies images.
To whoever comes to this repository, I refer you to [Molnar, Christoph. "Interpretable machine learning. A Guide for Making Black Box Models Explainable", 2019.](https://christophm.github.io/interpretable-ml-book/)

Well, with TDA means producing explanations through Topological Data Analysis, in particular to apply a well defined pipeline based on Mapper.

## Wow, that sounds great! But, is TDA able to perform better than other methods?
There is growing interest in using TDA to interpret a machine learning model, see
* [R.B. Gabrielsson, G. Carlsson, "Exposition and Interpretation of the Topology of Neural Networks"](https://arxiv.org/abs/1810.03234)
* [N. Saul, D. Arendt, "Machine Learning Explanations with Topological Data Analysis"](https://sauln.github.io/blog/tda_explanations/)
* [M. Gabella, "Topology of Learning in Feedforward Neural Networks," in IEEE Transactions on Neural Networks and Learning Systems, doi: 10.1109/TNNLS.2020.3015790.](https://ieeexplore.ieee.org/abstract/document/9174770)
* ###### To the reader, if you know other works feel free to make a pull request!

The reason behind this is that TDA is able to infer global qualitative properties from data. Global properties are then able to produce a summary of the shape underlying data. The Mapper algorithm is one of the best tools to produce such summaries, since it is able to group similar patches of filtered data in a lower dimensional representation.

If TDA is better than other methods is an open question. The first step is to find the link between the behaviour of a machine learning model and its topological features. Once we have a clear understanding of this we will able to answer the question.

## Ok, but I still don't get it. Can I consider the obtained results trustworthy?
TODO...
