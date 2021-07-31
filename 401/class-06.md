# Game of Greed 1

## How to use the Random Module in Python

### **Random functions**

- **Randint**(lowest_value,highest_value): to get a random integer in a range
- **Random**(): to get a random large number
- **Choice**(value1, value2, ...): generate a random value from the sequence
- **Shuffle**(list): shuffles the elements in list in place, so they are in a random order
- **Randrange**(start, stop, step): generate a randomly selected element from range

&nbsp;

## What is Risk Analysis?

**Risk**: the probability of any unwanted incident

**Risk analysis**: the process of identifying the risks in applications or software that built and prioritizing them to test

Examples of **potential risks that can be encountered**:

- Use of new hardware
- Use of new technology
- Use of new automation tool
- The sequence of code
- Availability of test resources for the application

Examples of **risks that are unavoidable**:

- The time allocated for testing
- A defect leakage due to the complexity or size of the application
- Urgency from the clients to deliver the project
- Incomplete requirements

**Risk magnitude indicators**:

- **_High_**: the effect of the risk would be very high and non-tolerable. The company might face loss.
- **_Medium_**: it is tolerable but not desirable. The company may suffer financially but there is a limited risk.
- **_Low_**: it is tolerable. There lies little or no external exposure or no financial loss.

&nbsp;

### **Risk Identification**

**Sets of risks** included in the risk identification process:

- **Business Risks**: the most common risk. It is the risk that may come from the company or the customer, not from the project.
- **Testing Risks**: Be well acquainted with the platform working on, along with the software testing tools being used.
- **Premature Release Risk**: a fair amount of knowledge to analyze the risk associated with releasing unsatisfactory or untested software is required

- **Software Risks**: Be well versed with the risks associated with the software development process.

&nbsp;

### **Risk Assessment**

**Perspectives of Risk Assessment**:

- **_Effect_** - to assess risk by Effect. In case identifying a condition, event or action and try to determine its impact.
- **_Cause_** - to assess risk by Cause is opposite of by Effect. Initialize scanning the problem and reach the point that could be the most probable reason behind that.
- **_Likelihood_** - to assess risk by Likelihood is to say that there is a probability that a requirement won’t be satisfied.

&nbsp;

## What is Dependency Injection?

**Dependency or dependent means relying on something for support**. Like if I say we are relying too much on mobile phones then it means we are dependent on them.

**Dependency injection**: a technique whereby one object (or static method) supplies the dependencies of another object. A dependency is an object that can be used (a service).

So, transferring the task of creating the object to someone else and directly using the dependency is called **dependency injection**.

&nbsp;

**Types of dependency injection**:

- **_Constructor injection_**: the dependencies are provided through a class constructor.
- **_Setter injection_**: the client exposes a setter method that the injector uses to inject the dependency.
- **_Interface injection_**: the dependency provides an injector method that will inject the dependency into any client passed to it.

**Dependency injection’s responsibility**:

- Create the objects
- Know which classes require those objects
- Provide them all those objects

**Benefits of using DI**:

- Helps in Unit testing.
- Boiler plate code is reduced, as initializing of dependencies is done by the injector component.
- Extending the application becomes easier.
- Helps to enable loose coupling, which is important in application programming.

**Disadvantages of DI**:

- It’s a bit complex to learn, and if overused can lead to management issues and other problems.
- Many compile-time errors are pushed to run-time.
- Dependency injection frameworks are implemented with reflection or dynamic programming.
