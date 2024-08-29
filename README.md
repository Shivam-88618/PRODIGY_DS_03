Decision Tree Classifier with Randomly Generated Data
This Python program demonstrates how to build and visualize a decision tree classifier using a randomly generated dataset. The code generates a dataset with two features and a binary target variable, splits the data into training and testing sets, trains a decision tree classifier, evaluates its performance, and visualizes the resulting decision tree.

Features
Random Data Generation:

The dataset contains 1000 samples, with each sample having two features (feature1 and feature2) and a binary target variable (target).
The target variable is defined as 1 if the sum of the two features is greater than 1, otherwise 0.
Data Splitting:

The dataset is split into training (80%) and testing (20%) sets using train_test_split from scikit-learn.
Decision Tree Classifier:

A decision tree classifier is trained using the training data.
The tree's depth is limited to a maximum of 3 levels to avoid overfitting.
Model Evaluation:

The trained model is evaluated on the test data using accuracy score and classification report metrics.
Decision Tree Visualization:

The decision tree is visualized using plot_tree from scikit-learn, showing the structure of the tree, including decision nodes and leaf nodes.
Dependencies
To run this program, you'll need the following Python libraries:

numpy
pandas
scikit-learn
matplotlib
You can install these dependencies using pip:

pip install numpy pandas scikit-learn matplotlib

Usage
Set Up the Environment: Ensure you have Python installed along with the required libraries.

Run the Script: Execute the script to generate the random dataset, train the decision tree classifier, evaluate the model, and visualize the decision tree.

python script_name.py

View the Output: The program will display:
The accuracy of the classifier on the test set.
A classification report showing precision, recall, and F1-score for each class.
A visualization of the decision tree.
How It Works
Data Generation:

The script generates a dataset with 1000 samples, each containing two features (feature1 and feature2).
The target variable (target) is calculated based on the sum of the two features.
Data Splitting:

The dataset is split into training and testing sets using an 80/20 ratio.
Decision Tree Training:

The decision tree classifier is trained on the training set with a maximum depth of 3 to prevent overfitting.
Model Evaluation:

The accuracy of the classifier on the test set is computed and printed.
A detailed classification report is provided, showing performance metrics for each class.
Tree Visualization:

The decision tree is visualized, with each node color-coded based on the class distribution and the depth of the tree.
Example Output
Accuracy and Classification Report
The script will print the accuracy of the classifier on the test set.
The classification report will show metrics such as precision, recall, and F1-score for each class.
Decision Tree Visualization
The decision tree structure will be displayed as a plot, showing how the features are split to make predictions.
Customization
Number of Samples: You can modify the n_samples variable to generate more or fewer samples.
Tree Depth: You can change the max_depth parameter in the DecisionTreeClassifier to control the complexity of the tree.
Feature Relationships: Modify the logic in generating the target variable to explore different relationships between features.

Author
This script was created as an educational tool to demonstrate the basics of decision tree classification using Python.
