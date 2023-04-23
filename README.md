Download Link: https://assignmentchef.com/product/solved-605-449-introduction-to-machine-learning-programming-project-4-extra-credit
<br>
The purpose of this assignment is to give you a chance to get some hands-on experience learning decision trees for classification and, for extra credit, regression. This time around, we are not going to use anything from the module on rule induction; however, you might want to examine the rules learned for your trees to see if they “make sense.” Specifically, you will be implementing a standard univariate (i.e., axis-parallel) decision tree and will compare the performance of the trees when grown to completion on trees that use either early stopping (for regression trees) or reduced error pruning (for classification trees).

For decision trees, it should not matter whether you have categorical or numeric attributes, but you need to remember to keep track of which is which. In addition, you need to implement that gain-ratio criterion for splitting in your classification trees. For the regression trees, all of the attributes will be numeric.

For this assignment, you will use three classification datasets (plus three regression data sets for the extra credit) that you will download from the UCI Machine Learning Repository, namely:

<ol>

 <li>Abalone — https://archive.ics.uci.edu/ml/datasets/Abalone</li>

</ol>

[Classification] Predicting the age of abalone from physical measurements.

<h1>2.    Car Evaluation — https://archive.ics.uci.edu/ml/datasets/Car+Evaluation</h1>

[Classification] The data is on evaluations of car acceptability based on price, comfort, and technical specifications.

<h1>3.    Image Segmentation — https://archive.ics.uci.edu/ml/datasets/Image+Segmentation</h1>

[Classification] The instances were drawn randomly from a database of 7 outdoor images. The images were hand segmented to create a classification for every pixel.

<h1>4.    Computer Hardware — https://archive.ics.uci.edu/ml/datasets/Computer+Hardware</h1>

[Regression] The estimated relative performance values were estimated by the authors using a linear regression method. The gives you a chance to see how well you can replicate the results with these two models.

<h1>5.    Forest Fires — https://archive.ics.uci.edu/ml/datasets/Forest+Fires</h1>

[Regression] This is a difficult regression task, where the aim is to predict the burned area of forest fires, in the northeast region of Portugal, by using meteorological and other data .

<h1>6.    Wine Quality — https://archive.ics.uci.edu/ml/datasets/Wine+Quality</h1>

[Regression] This contains two data sets, one for red wine and one for white. Either combine the data sets into a single set for the regression task or build separate regression trees. This is your choice; however, we expect the separate trees to be better. The objective is to learn a model to assess the quality of wine.

For this project, the following steps are required:

<ul>

 <li>Download the six (6) data sets from the UCI Machine Learning repository. You can find this repository at http://archive.ics.uci.edu/ml/. All of the specific URLs are also provided above.</li>

 <li>Implement the ID3 algorithm for classification decision trees using gain-ratio as the splitting criterion.</li>

 <li>Implement reduced-error pruning to be used as an option with your implementation of ID3.</li>

 <li>Run your ID3 implementation on each of the three classification data sets, comparing both pruned and unpruned versions of the trees. These runs should be done with 5-fold cross-validation so you can compare your results statistically. You should pull out 10% of the data to be used as a validation set and then use the remaining 90% for cross validation. You should use classification error for your loss function.</li>

</ul>

1

<ul>

 <li>Extra credit (for up to 20 additional points):</li>

 <li>Implement the CART algorithm for regression decision trees using mean squared error as the splitting criterion.</li>

 <li>Incorporate a cut-off threshold for early stopping. If the threshold is set to zero, this should indicate no early stopping.</li>

 <li>Run your CART implementation on each of the three regression data sets, comparing both full and stopped versions of the trees. You will need to tune the stopping threshold and should use the same procedure for extracting a validation set to serve as your tuning set. The runs should be done with 5-fold cross-validation so you can compare your results statistically. You should use mean squared error for your loss function.</li>

 <li>Write a very brief paper that incorporates the following elements, summarizing the results of your experiments.

  <ol>

   <li>Title and author name</li>

   <li>A brief, one paragraph abstract summarizing the results of the experiments</li>

   <li>Problem statement, including hypothesis, projecting how you expect each algorithm to perform</li>

   <li>Brief description of algorithms implemented</li>

   <li>Brief description of your experimental approach</li>

   <li>Presentation of the results of your experiments</li>

   <li>A discussion of the behavior of your algorithms, combined with any conclusions you can draw</li>

   <li>Summary</li>

   <li>References (you should have at least one reference related to each of the algorithms implemented,a reference to the data sources, and any other references you consider to be relevant)</li>

  </ol></li>

 <li>Submit your fully documented code, the outputs from running your programs, and your paper. Your grade will be broken down as follows:

  <ul>

   <li>Code structure – 10%</li>

   <li>Code documentation/commenting – 10%</li>

   <li>Proper functioning of your code, as illustrated by a 5 minute video – 30%</li>

   <li>Summary paper – 50%</li>

  </ul></li>

</ul>

2