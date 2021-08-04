# Dunder Methods & Probability & Mathematical statistics functions

## Dunder Methods

In Python, special methods are a set of predefined methods you can use to enrich your classes. They are easy to recognize because they start and end with double underscores, for example, **init** or **str**.

These **dunders** or **special methods** in Python are also sometimes called **magic methods**

Dunder methods let you emulate the behavior of built-in types.

- **Initialization of new objects: init**

- **Object representation: str , repr**

- **Enable iteration: len , getitem , reversed**

- **Operator overloading (comparison): eq , lt**

- **Operator overloading (addition): add**

- **Method invocation: call**

- **Context manager support (with statement): enter , exit**

&nbsp;

## Probability in Python

At the most basic level, probability seeks to answer the question, **What is the chance of an event happening?** An event is some outcome of interest. To calculate the chance of an event happening, we also need to consider all the other events that can occur.

probability gives us a framework for making predictions about how often events will happen.

In a probability context, the high point in a normal distribution represents the event with the highest probability of occurring.

### **Revisiting the normal**

The normal distribution is significant to probability and statistics thanks to two factors: the Central Limit Theorem and the Three Sigma Rule.

### **Z-score**

The Z-score is a simple calculation that answers the question, **Given a data point, how many standard deviations is it away from the mean?** The equation below is the Z-score equation.

&nbsp;

## Mathematical statistics functions

| **Function**         | **Discription**                                             |
| -------------------- | ----------------------------------------------------------- |
| **mean()**           | Arithmetic mean (“average”) of data                         |
| **fmean()**          | Fast, floating-point arithmetic mean                        |
| **geometric_mean()** | Geometric mean of data                                      |
| **harmonic_mean()**  | Harmonic mean of data                                       |
| **median()**         | Median (middle value) of data                               |
| **median_low()**     | Low median of data                                          |
| **median_high()**    | High median of data                                         |
| **median_grouped()** | Median, or 50th percentile, of grouped data                 |
| **mode()**           | Single mode (most common value) of discrete or nominal data |
| **multimode()**      | List of modes (most common values) of discrete or nomimal   |
| **quantiles()**      | Divide data into intervals with equal probability           |
