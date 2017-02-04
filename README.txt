Environment details
-------------------

Language	Java(1.6)

Instructions
------------

compiling:
javac decisionTree.java

Generic Run format:
java decisionTree <L> <K> <training_set.csv> <validation_set> <test_set.csv> <to-print>

Sample test cases:
java decisionTree 100 5 ds1_training_set.csv ds1_validation_set.csv ds1_test_set.csv no
java decisionTree 200 10 ds1_training_set.csv ds1_validation_set.csv ds1_test_set.csv yes
java decisionTree 100 5 ds2_training_set.csv ds2_validation_set.csv ds2_test_set.csv yes
java decisionTree 200 10 ds2_training_set.csv ds2_validation_set.csv ds2_test_set.csv no

if <to-print> option is set, decision tree will be written to the standard output

Approach
--------

1.Tree is created with <training_set.csv> using Information Gain Heuristic 
2.Pruning is done using <validation_set.csv>
3.Accuracy is measured on <test_set.csv> 

note: accuracy is measure of (correctly predicted instances)/(total instances)


