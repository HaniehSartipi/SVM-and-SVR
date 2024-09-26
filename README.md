# SVM-and-SVR
Used the make_moons dataset and achieved the best results with an RBF kernel, reaching an accuracy of 0.93.
I start by splitting the dataset (with 0.2 noise) into training and testing sets, using train_test_split with test_size=0.3. For each kernel (e.g., linear, RBF, polynomial), I fine-tune hyperparameters using RandomizedSearchCV and evaluate the models with accuracy and recall.

Linear Kernel: Achieved 85% accuracy but poorly separates the data.
RBF Kernel: Performed best with 93% accuracy, effectively separating the data due to its fit to the dataset's structure.
Polynomial Kernel: Reached 92% accuracy but showed risk of overfitting due to narrower margins.
Sigmoid Kernel: Similar to the linear kernel, achieved 85% accuracy, but was too simplistic for the data.
