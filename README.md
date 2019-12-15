# Chemical Compound Classifier -> Neural Network (L-Layer)

#### TASK: 
The given dataset contains details about organic chemical compounds including their chemical features, isomeric conformation, names and the classes in which they are classified. The compounds are classified as either ‘Musk’ or ‘Non-Musk’ compounds. 

Build a classification model.

## DATA PRE-PROCESSING:
#### Dataset - Musk_csv:
1. No. of columns 170
2. No. of rows 6598

#### Drop unnecessary columns :- ID, Molecular name, conformation isomer.

#### DATA = 166 required features
#### LABELS = 1(MUSK), 0(NON-MUSK)

## TRAINING:

### Using Neural Network (L - LAYER NETWORK)
An ANN is based on a collection of connected units or nodes called artificial neurons (analogous to biological neurons in an animal brain). Each connection (synapse) between neurons can transmit a signal from one to another. The receiving (postsynaptic) neuron can process the signal(s) and then signal downstream neurons connected to it. In common ANN implementations, the synapse signal is a real number, and the output of each neuron is calculated by a non-linear function of the sum of its input. Neurons and synapses may also have a weight that varies as learning proceeds, which can increase or decrease the strength of the signal that it sends downstream. Further, they may have a threshold such that only if the aggregate signal is below (or above) that level is the downstream signal sent.

<img src = "https://upload.wikimedia.org/wikipedia/commons/thumb/4/46/Colored_neural_network.svg/300px-Colored_neural_network.svg.png">

##### L-LAYER NETWORK - The number of hidden layers can be increased or decreased by simply adding or deleting the entries in "layers_dims" array. 
##### Gives flexibility in training and generalises the model for future use.

<img src = "https://github.com/vivek7415/chemical_compound_classifier/blob/master/MODEL.png">

#### Hidden Layers - [166, 20, 1]
#### Learning Rate - 0.1
#### Number of iterations - 3000

Trained the model using these settings. 
<img src="https://github.com/vivek7415/chemical_compound_classifier/blob/master/TRAINING.png">


## RESULT:
<img src = "https://github.com/vivek7415/chemical_compound_classifier/blob/master/GRAPH.png">

#### ACCURACY : 97.8%

#### Precision, Recall, F-1 Score
<img src = "https://github.com/vivek7415/chemical_compound_classifier/blob/master/F-1.png">
