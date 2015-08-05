[![Keras question answering for bAbi](http://i.imgur.com/RuINg4m.jpg)](https://www.flickr.com/photos/isherwoodchris/6917253693/in/photolist)

# Keras question answering for bAbi

**Note: This code has been merged as an example into Keras -- see [babi_rnn.py](https://github.com/fchollet/keras/blob/master/examples/babi_rnn.py)**

This repository contains Keras code to train two recurrent neural networks based upon a story and a question.
The resulting merged vector is then queried to answer a range of bAbI tasks.

An example from the first task, QA1, is below:

    1 Mary moved to the bathroom.
    2 John went to the hallway.
    3 Where is Mary? bathroom 1
    4 Daniel went back to the hallway.
    5 Sandra moved to the garden.
    6 Where is Daniel? hallway 4

The results are comparable (or superior) to those for the LSTM baseline provided in Weston et al.'s [Towards AI-Complete Question Answering: A Set of Prerequisite Toy Tasks](http://arxiv.org/abs/1502.05698) given only 1000 samples and without any hyperparamater tuning.

Task Number                  | FB LSTM Baseline | Keras QA
---                          | ---              | ---
QA1 - Single Supporting Fact | 50               | 52.1
QA2 - Two Supporting Facts   | 20               | 37.0
QA3 - Three Supporting Facts | 20               | 20.5
QA4 - Two Arg. Relations     | 61               | 62.9
QA5 - Three Arg. Relations   | 70               | 61.9
QA6 - Yes/No Questions       | 48               | 50.7
QA7 - Counting               | 49               | 78.9
QA8 - Lists/Sets             | 45               | 77.2
QA9 - Simple Negation        | 64               | 64.0
QA10 - Indefinite Knowledge  | 44               | 47.7
QA11 - Basic Coreference     | 72               | 74.9
QA12 - Conjunction           | 74               | 76.4
QA13 - Compound Coreference  | 94               | 94.4
QA14 - Time Reasoning        | 27               | 34.8
QA15 - Basic Deduction       | 21               | 32.4
QA16 - Basic Induction       | 23               | 50.6
QA17 - Positional Reasoning  | 51               | 49.1
QA18 - Size Reasoning        | 52               | 90.8
QA19 - Path Finding          | 8                | 9.0
QA20 - Agent's Motivations   | 91               | 90.7

For the resources related to the bAbI project, refer to the [Facebook AI Research bAbI project page](https://research.facebook.com/researchers/1543934539189348).

# License

MIT License, as per `LICENSE`
