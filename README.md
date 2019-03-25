# Image Classification using Support Vector Machine(SVM)

Support Vector Machine can be used for multiclass classification by using One vs One or One vs Rest technique.

## One vs One
Here, you pick 2 classes at a time, and train a two-class-classifier using samples from the selected 
two classes only (other samples are ignored in this step). You repeat this for all the two class combinations. 
So you end up with N(N-1)/2 classifiers. And while testing, you do voting among these classifiers.

## One vs Rest
Here, you pick one class and train a two-class-classifier with the samples of the selected class on one side and 
all the other samples on the other side. Thus, you end up with N classifiers. 
While testing, you simply classify the sample as belonging to the class with maximum score among the N classifiers.

### Future work
In the above project One vs One technique has been implemented. The One vs Rest technique can be implemented and the accuracies of 
both the techniques can be compared.
