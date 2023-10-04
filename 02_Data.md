# Chapter 2: Data

Become one with the data
	- inspect data (understand distribution, look for patterns)
	- corrupted data/labels?
	- data imbalances/biases?
	- visualizations distribution (e.g. type of label, size of annotations, number of annotations, image size, average sentence length) and outliers
	- Split data into train/test/eval
		- is the training data representative 
		- is there information leakage between the train/test/val data
		- is the distribution of the validation data similar to the data in the production environment
	- implement dataloader
	- visualize data just before passing it into the model (raw tensor data/labels)
	- What are important metrics?
	- Which loss function should be used? (Do we need a custom loss?)
