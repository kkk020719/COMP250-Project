# COMP250-Project
Using binary decision trees to classify and analyze spatial data based on entropy calculations

# Despcription of the project
Training Phase:
We first create a decision tree based on a labelled data set where aach data item (datum) in the given labelled data set has well defined attributes x and label y.
We refer to the data set that is used to create a decision tree as the training set. 

Testing Phase:
For the testing phase, one can use data items from the original data used for training (above) or one can use new data. Typically when a decision tree is used in 
practice, the test objects are unlabelled and we will to use the decision tree to choose a label for the object.

The problem of this project is to to classify points coming from a dataset(i.e. split the set of data items into two subsets)during the training phase and attribute
the two subsets to the two nodes. Each datapoint has an array of attributes x(x[0], is represented as x1 and x[1] as x2), and a binary label y (0 or 1).

In this project, we are splitting the data based on entropy. Specific formula can be found in the DTNode.fillDTNode() function. We can use entropy to compare the 
‘goodness’ of different splits. To prevent overfitting, the method that we will use is called early stopping, namely stop splitting nodes in the decision tree when 
the number of data  points in a subset is smaller than some predetermined number.





