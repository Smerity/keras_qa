[![Keras question answering for bAbi](http://i.imgur.com/RuINg4m.jpg)](https://www.flickr.com/photos/isherwoodchris/6917253693/in/photolist)

# Keras question answering for bAbi

This repository contains Keras code to train two recurrent neural networks based upon a story and a question.
The resulting merged vector is then queried to answer a range of bAbI tasks.

An example from the first task, QA1, is below:

    1 Mary moved to the bathroom.
    2 John went to the hallway.
    3 Where is Mary? bathroom 1
    4 Daniel went back to the hallway.
    5 Sandra moved to the garden.
    6 Where is Daniel? hallway 4

The results are comparable to those for an LSTM model provided in Weston et al.'s [Towards AI-Complete Question Answering: A Set of Prerequisite Toy Tasks](http://arxiv.org/abs/1502.05698).

For the resources related to the bAbI project, refer to the [Facebook AI Research bAbI project page](https://research.facebook.com/researchers/1543934539189348).

# License

MIT License, as per `LICENSE`
