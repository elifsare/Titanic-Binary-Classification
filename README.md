# :ship:	Data Preprocess
- NaN values have been replaced by the median. 
- Sex, cabin names, names of embarkation ports have been replaced with integers.

# :chart_with_upwards_trend: Desciription Of Model
### Why We Use Sequel Model?
This model is appropriate for a plain stack of layers where each layer has exactly one input tensor and one output tensor. That's why the Sequel Model is used.

### Adam Algorithm
According to Kingma et al., 2014, the method is "computationally efficient, has little memory requirement, invariant to diagonal rescaling of gradients, and is well suited for problems that are large in terms of data/parameters".  That's why the Adam algorithm is used.

### Model Compilation And Saving to a File
Binary classification is done in the model, so binary entropy is used in the loss function. ModelCheckpoint callback is used in conjunction with training using model.fit() to save a model or weights (in a checkpoint file) at some interval, so the model or weights can be loaded later to continue the training from the state saved. That's why the ModelCheckpoint() is used.

### Pylot Results
<img src="https://github.com/elifsare/Titanic-Binary-Classification/blob/main/Accuracy_loss.png" />
