---
layout: wp
number: 2
name: Attention mechanisms
description: Developing deep learning algorithms based on attention mechanisms to enable robust and efficient identification of multiple event types within PSG data.
---

Development of deep learning attention mechanisms algorithms to allow concurrent and individual identification of different types of events in the context of each PSG interval, thus overcoming limitations of current approaches and being more robust, generalizable and much more computationally efficient. 

Here we plan the integration of Transformers within the PSG analysis framework because they do not analyze inputs sequentially, having therefore the potential of modeling complex time series dynamics. This can be done in several ways that must be studied: just replacing “first-generation” layers such as LSTMs by self-attention layers. Another possibility is to use the raw PSG signals directly as input. 

A further step down this line can be taken by considering a prediction problem in which each token represents the value of a single variable per time step. Transformers are then free to attend to the values of any variable at any time in order to produce more accurate predictions. Since the complexity of Transformers might become a limiting factor in our PSG context it is planned to use the Perceiver architecture to reduce space complexity by adding a cross attention layer between the input sequence and multi-headed attention. A supercharged version, namely Perceiver(IO), has also been recently proposed which adds extra cross-attention in the last layer of the decoder, this, in the proposed processing pipeline can allow complex output configuration, including event positioning, which might be a convenient approach for integration of self-attention in the event identification framework.