 Set up the end-to-end training/evaluation skeleton + get dumb baselines
	- train a dumb/simple model 
	- verify initial loss (uni\ttest?)
	- initialize final layer weights correctly (init bias on logits such that loss is uniformly distributed) (unittest?)
	- input-independent baseline (all 0 input) (unittest?)
	- zero-rule baseline (accuracy when always predicting majority class for all examples) (unittest?)
	- confusion matrix plotting
	- overfit one batch (unittest?)
	- visualize predictions for a fixed batch 
	- use R^2 to track accuracy for regression
	- use backprop to chart dependencies (unittest?)
		 Hey, I performed a similar kind of test. With Pytorch:  
		1. Create a multi-batch input (x = torch.rand([4, 3, 224, 224])  
		2. Set your input to be differentiable (x.requires_grad = True)  
		3. Run a forward pass (out = model(x))  
		4. Define the loss as depending from only one of the inputs (for instance: loss = out[2].sum())  
		5. Run a backprop (loss.backward)  
		6. Verify that only x[2] has non-null gradients: assert (x.grad[i] == 0.).all() for i != 2 and (x.grad[2] != 0).any())
		 Note: you will want to set your model into evaluation mode (model.eval()), otherwise batch norm ops will make this test fail.
