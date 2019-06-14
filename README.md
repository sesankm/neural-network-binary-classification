# neural-network-binary-classification

## The objective is to predict whether or not individual has a cardiovascular disease.

**Dataset Information**

The data set consists of a total of 11 features. The target variable is a binary value indicating whether or not a cardiovascular disease is present in the subject. <br>

**Feature Information**

Age | Objective Feature | age | int (days) | <br>
Height | Objective Feature | height | int (cm) | <br>
Weight | Objective Feature | weight | float (kg) | <br>
Gender | Objective Feature | gender | categorical code | 1: Women, 2: Men |<br>
Systolic blood pressure | Examination Feature | ap_hi | int | <br>
Diastolic blood pressure | Examination Feature | ap_lo | int |<br>
Cholesterol | Examination Feature | cholesterol | 1: normal, 2: above normal, 3: well above normal |<br>
Glucose | Examination Feature | gluc | 1: normal, 2: above normal, 3: well above normal |<br>
Smoking | Subjective Feature | smoke | binary |<br>
Alcohol intake | Subjective Feature | alco | binary |<br>
Physical activity | Subjective Feature | active | binary |<br>
Presence or absence of cardiovascular disease | Target Variable | cardio | binary |<br>

---
## Model Info
The model is densely connected feedforward Neural Network. The .ipynb has a more extensive explanation of the following info.

### Activation Functions:
**relu**
<br> The vanishing gradient problem: the gradients of some activation functions becoming increasingly smaller as the number of hidden layers increases. This is problematic because the parameters in the neural network won't be tuned effectively.
<br>ReLU overcomes this problem.
 
**sigmoid**
<br>Activation function used in the output layer. Effective for classification problems.

### Loss Function:
**Binary Crossentropy**
<br>Cross entropy is calculated by finding the predicted probability (the probability of classification being correct based on given data). Larger predicted probabilities yeild lower losses. Binary Cross Entropy loss is a sigmoid activiation function along with the cross entropy loss function. 

### Optmization Function:
**Adam Optmizier**
<br> Calculates adaptive learning rates for each parameter.
