# Machine Learning Intro

## Definition

Machine learning is not about algorithms. Machine learning is a comprehensive approach to solving problems. Machine learning is the practice of teaching computers how to learn patterns from data, often for making decisions or predictions. For true machine learning, the computer must be able to learn patterns that it's not explicitly programmed to identify.

- **Model** - a set of patterns learned from data.
- **Algorithm** - a specific ML process used to train a model.
- **Training data** - the dataset from which the algorithm learns the model.
- **Test data** - a new dataset for reliably evaluating model performance.
- **Features** - Variables (columns) in the dataset used to train the model.
- **Target variable** - A specific variable you're trying to predict.
- **Observations** - Data points (rows) in the dataset.

### **Categories of Tasks**

**1. Supervised Learning**

- Supervised learning includes tasks for "labeled" data.
- In practice, it's often used as an advanced form of predictive modeling.
- Each observation must be labeled with a "correct answer."
- Only then can you build a predictive model because you must tell the algorithm what's "correct" while training it (hence, "supervising" it).
- Regression is the task for modeling continuous target variables.
- Classification is the task for modeling categorical (a.k.a. "class") target variables.

**2. Unsupervised Learning**

- Unsupervised learning includes tasks for "unlabeled" data.
- In practice, it's often used either as a form of automated data analysis or automated signal extraction.
- Unlabeled data has no predetermined "correct answer."
- You'll allow the algorithm to directly learn patterns from the data (without "supervision").
- Clustering is the most common unsupervised learning task, and it's for finding groups within your data.

### **The 3 Elements of Great Machine Learning**

1. A skilled chef (**human guidance**)

- You'll need to make dozens of decisions along the way.
- In fact, the very first major decision is how to roadmap your project for guaranteed success.

  2.Fresh ingredients (**clean, relevant data**)

- Garbage In = Garbage Out, no matter which algorithms you use.
- Professional data scientists spend most of their time understanding the data, cleaning it, and engineering new features.

  3.Don't overcook it (**avoid overfitting**)

- An overfit model within a hedge fund can cost millions of dollars in losses.
- An overfit model within a hospital can cost thousands of lives.
- For most applications, the stakes won't be quite that high, but overfitting is still the single largest mistake you must avoid.

&nbsp;

## Exploratory Analysis

Doing so upfront will make the rest of the project much smoother, in 3 main ways:

- You’ll gain valuable hints for Data Cleaning (which can make or break your models).
- You’ll think of ideas for Feature Engineering (which can take your models from good to great).
- You’ll get a "feel" for the dataset, which will help you communicate results and deliver greater impact.

**1. Start with Basics.** First, you'll want to answer a set of basic questions about the dataset:

- How many observations do I have?
- How many features?
- What are the data types of my features? Are they numeric? Categorical?
- Do I have a target variable?

**2. Plot Numerical Distributions.** Next, it can be very enlightening to plot the distributions of your numeric features. Often, a quick and dirty grid of histograms is enough to understand the distributions.

- Distributions that are unexpected
- Potential outliers that don't make sense
- Features that should be binary (i.e. "wannabe indicator variables")
- Boundaries that don't make sense
- Potential measurement errors

**3. Plot Categorical Distributions.** Categorical features cannot be visualized through histograms. Instead, you can use bar plots.

**4. Plot Segmentations.** Segmentations are powerful ways to observe the relationship between categorical features and numeric features.

**5. Study Correlations.** Correlations allow you to look at the relationships between numeric features and other numeric features. Correlation is a value between -1 and 1 that represents how closely two features move in unison. You don't need to remember the math to calculate them. Just know the following intuition:

- Positive correlation means that as one feature increases, the other increases.
- Negative correlation means that as one feature increases, the other decreases.
- Correlations near -1 or 1 indicate a strong relationship.
- Those closer to 0 indicate a weak relationship.
- 0 indicates no relationship.

&nbsp;

## Data Cleaning

### **Better Data > Fancier Algorithms**

**1. Remove Unwanted observations.**

- **Duplicate observations**

  - Combine datasets from multiple places
  - Scrape data
  - Receive data from clients/other departments

- **Irrelevant observations**

  - If you were building a model for Single-Family homes only, you wouldn't want observations for Apartments in there.
  - This is also a great time to review your charts from Exploratory Analysis.
  - Checking for irrelevant observations before engineering features can save you many headaches down the road.

**2. Fix Structural Errors.** Structural errors are those that arise during measurement, data transfer, or other types of "poor housekeeping."

**3. Filter Unwanted Outliers.** Outliers can cause problems with certain types of models. In general, if you have a legitimate reason to remove an outlier, it will help your model’s performance

**4. Handle Missing Data.**

- **You cannot simply ignore missing values in your dataset.** You must handle them in some way for the very practical reason that most algorithms do not accept missing values.

- **Ways of dealing with missing data actually suck:**

  - Dropping observations that have missing values
  - Imputing the missing values based on other observations

- **Dropping missing values is sub-optimal because when you drop observations, you drop information.**

  - The fact that the value was missing may be informative in itself.
  - You often need to make predictions on new data even if some of the features are missing!

- **Imputing missing values is sub-optimal because the value was originally missing but you filled it in**, which always leads to a loss in information, no matter how sophisticated your imputation method is.

  - "Missingness" is almost always informative in itself, and you should tell your algorithm if a value was missing.
  - Even if you build a model to impute your values, you’re not adding any real information. You’re just reinforcing the patterns already provided by other features.

- **Missing categorical data.** The best way to handle missing data for categorical features is to simply label them as ’Missing’!

  - You’re essentially adding a new class for the feature.
  - This tells the algorithm that the value was missing.
  - This also gets around the technical requirement for no missing values.

- **Missing numeric data.** For missing numeric data, you should flag and fill in the values.

  - Flag the observation with an indicator variable of missingness.
  - Then, fill the original missing value with 0 just to meet the technical requirement of no missing values.

&nbsp;

## Feature Engineering

Feature engineering is about **creating new input features from your existing ones**. This is often one of the most valuable tasks a data scientist can do to improve model performance, for 3 big reasons:

- You can isolate and highlight key information, which helps your algorithms "focus" on what’s important.
- You can bring in your own domain expertise.
- Most importantly, once you understand the "vocabulary" of feature engineering, you can bring in other people’s domain expertise!

**1. Infuse Domain Knowledge.** You can often engineer informative features by tapping into your (or others’) expertise about the domain.

**2. Create Interaction Features.** By the way, in some contexts, "interaction terms" must be products between two variables. In our context, interaction features can be products, sums, or differences between two features. A general tip is to look at each pair of features and ask yourself, "could I combine this information in any way that might be even more useful?"

**3. Combine Sparse Classes.** Sparse classes (in categorical features) are those that have very few total observations. They can be problematic for certain machine learning algorithms, causing models to overfit.

- There's no formal rule of how many each class needs.
- It also depends on the size of your dataset and the number of other features you have.
- As a rule of thumb, we recommend combining classes until each one has at least ~50 observations. As with any "rule" of thumb, use this as a guideline.

**4. Add Dummy Variables.** Dummy variables are a set of binary (0 or 1) variables that each represent a single class from a categorical feature. The information you represent is exactly the same, but this numeric representation allows you to pass the technical requirements for algorithms.

**5. Remove Unused Features.** Unused features are those that don’t make sense to pass into our machine learning algorithms. Examples include:

- ID columns
- Features that wouldn't be available at the time of prediction
- Other text descriptions

&nbsp;

## Algorithm Selection

**1. Why Linear Regression is Flawed?**

Simple linear regression suffers from two major flaws:

- It's prone to overfit with many input features.
- It cannot easily express non-linear relationships.

**2. Regularization in Machine Learning.** The first flaw of linear models is that they are prone to overfit with many input features. Regularization is a technique used to prevent overfitting by artificially penalizing model coefficients.

- It can discourage large coefficients (by dampening them).
- It can also remove features entirely (by setting their coefficients to 0).
- The "strength" of the penalty is tunable. (More on this tomorrow...)

**3. Regularized Regression Algos.** There are 3 common types of regularized linear regression algorithms:

- **Lasso Regression.** Stands for Least Absolute Shrinkage and Selection Operator.

  - Lasso regression penalizes the absolute size of coefficients.
  - Practically, this leads to coefficients that can be exactly 0.
  - Thus, Lasso offers automatic feature selection because it can completely remove some features.
  - Remember, the "strength" of the penalty should be tuned.
  - A stronger penalty leads to more coefficients pushed to zero.

- **Ridge Regression.** Stands Really Intense Dangerous Grapefruit Eating (just kidding... it's just ridge).

  - Ridge regression penalizes the squared size of coefficients.
  - Practically, this leads to smaller coefficients, but it doesn't force them to 0.
  - In other words, Ridge offers feature shrinkage.
  - Again, the "strength" of the penalty should be tuned.
  - A stronger penalty leads to coefficients pushed closer to zero.

- **Elastic-Net.** A compromise between Lasso and Ridge.

  - Elastic-Net penalizes a mix of both absolute and squared size.
  - The ratio of the two penalty types should be tuned.
  - The overall strength should also be tuned.
  - There’s no "best" type of penalty. It really depends on the dataset and the problem.

**4. Decision Tree Algos.** Due to their branching structure, decision trees can easily model nonlinear relationships.

- For example, let's say for Single Family homes, larger lots command higher prices.
- However, let's say for Apartments, smaller lots command higher prices (i.e. it's a proxy for urban/rural).
- This reversal of correlation is difficult for linear models to capture unless you explicitly add an interaction term
- On the other hand, decision trees can capture this relationship naturally.

**5. Tree Ensembles.** Ensembles are machine learning methods for combining predictions from multiple separate models. There are a few different methods for ensembling, but the two most common are:

- **Bagging.** Attempts to reduce the chance of overfitting complex models.

  - It trains a large number of "strong" learners in parallel.
  - A strong learner is a model that's relatively unconstrained.
  - Bagging then combines all the strong learners together in order to "smooth out" their predictions.

- **Boosting.** Attempts to improve the predictive flexibility of simple models.

  - It trains a large number of "weak" learners in sequence.
  - A weak learner is a constrained model (i.e. you could limit the max depth of each decision tree).
  - Each one in the sequence focuses on learning from the mistakes of the one before it.
  - Boosting then combines all the weak learners into a single strong learner.
