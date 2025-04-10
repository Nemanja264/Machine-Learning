Has infinite number of outputs

**1) Linear Regression**  
**Use:**  
    Predicts continuous outcomes (e.g., house prices, salary, stock prices).
   
  **Cost function: J(w,b) = 1/2m * sum((Y(i)-y(i))^2)** // sum(m), i=1  
  *Goal of Linear Regression:* minimize J(w), J(w)=wx, to find the cost function that fits the training data the best (by finding values for w that does it)  
  *General case:* find minimizeJ(w,b)=wx+b - **single input variable**
  
  The height of line in x,y graph is actually the value of b and the angle of it is w  
  In **squared error cost function** there is no mulitple local minimums, only one thats **global minimum**

***Gradient Decent*** 

*multiple local minimums*  
**&alpha; - learning rate**, the size of the steps that are taken to reach the minimum
<img src="Pictures/Screenshot%202025-02-11%20005832.png" height="300">

<img src="Pictures/Screenshot%202025-02-11%20013128.png" height="300">  

**Multiple inputs variables**:   
Some ML libraries use ***normal equation*** in back-end to solve (w,b) vectorization - ***interview question***  
<img src="Pictures/Screenshot%202025-02-11%20160930.png" height="300">  

**Rescaling:**
**Feature scaling** - when features have very different range its better to rescale them in 0-1 for better search for local minimum  
*Mean normalization*  
*Z-score normalization*  
  

**3) Decision Trees**  
  **Use:**  
    Provides interpretable models for decision-making.  
    Used in both classification (e.g., credit scoring, customer segmentation) and regression (predicting continuous values).  

  Supervised Learning Algorithm that splits data into branches based on feature values.
  Variations:
    Classification Trees for categorical outcomes.
    Regression Trees for continuous outcomes.

**4) Support Vector Machines (SVM)**  
**Use:**  
    Finds the optimal boundary (hyperplane) to separate classes; also used for regression (SVR - Support Vector Regression).

  Supervised Learning Algorithm mainly for classification.  
  Variations:  
    Linear SVM: For linearly separable data.  
    Non-Linear SVM: Uses kernel functions (e.g., RBF, polynomial) for data that isn’t linearly separable.  
    SVR: The regression variant of SVM.

  SVC (Support Vector Classifier)
    Purpose: A type of Support Vector Machine (SVM) used for classification tasks.  
    Core Idea: Finds the optimal hyperplane that maximizes the margin between classes.  
    Ideal For: Small to medium-sized and high-dimensional datasets.  

    Key Hyperparameters:
      C: Regularization parameter balancing margin size and classification errors.  
        C determines how many data samples are allowed to be placed in different classes  

      Kernel Function: a method used to take data as input and transform it into the required form of processing data.(Linear, Polynomial, Radial Basis Function(RBF), Gaussian...)
          RBF: /*It maps the data into an infinite-dimensional*/. We use RBF kernel When the decision boundary is highly non-linear and we have no prior knowledge about the data’s structure is available.

      Gamma: Kernel coefficient controlling the influence of individual data points.
