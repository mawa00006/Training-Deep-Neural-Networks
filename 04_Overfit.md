# Chapter 4: Overfit

First get a model large enough to overfit the data (low training loss), then focus on regularizing the model (Improve evaluation metrics by giving up some training loss)
Full training+ evaluation pipeline is working

    - pick a model (don't be a hero and start with a simple architecture from a related paper)
    - use adam optimizer
    - complexify one at a time
    - do not trust learning rate decay defaults (use a constant learning and only tune it at the end)
