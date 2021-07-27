# Classes and Objects, Pytest

## Classes and Objects

- **Objects** are an encapsulation of variables and functions into a single entity.
- Objects get their variables and functions from **classes**.
- **Classes** are essentially a **template** to create **objects**.

&nbsp;

## Thinking Recursively in Python

A **recursive function** is a function defined in terms of itself via self-referential expressions, this means that the function will continue to call itself and repeat its behavior until some condition is met to return a result.

&nbsp;

## Pytest Fixtures and Coverage

### **Fixtures**

When the tests were more complex, we'll want to have some objects available to all of the tests.

Those objects might contain data that want to share across tests, or they might involve the network or filesystem.

These are often known as **"fixtures"** in the testing world, and they take a variety of different forms.

In pytest, define fixtures using a combination of the **pytest.fixture decorator**, along with a **function definition**

### **Coverage**

When software gets larger and more complex, it's not going to be so easy to eyeball it.

That where to want to have **"code coverage"**, **checking that the tests have run all of the code**.

&nbsp;

## Pytest Fixtures

Fixtures define the **steps and data that constitute the arrange phase of a test**.

In pytest, they are **functions defined that serve this purpose**.

The services, state, or other operating environments set up by fixtures are accessed by test functions through arguments

We can tell pytest that a particular function is a fixture by decorating it with **@pytest.fixture**

### **Fixtures capabilities:**

- Fixtures have **explicit names** and are activated by declaring their use from test functions, modules, classes, or whole projects.

- Fixtures are implemented in a **modular manner**, as each fixture name triggers a fixture function that can itself use other fixtures.

- Fixture management scales from **simple unit to complex functional testing**, allowing to parametrize fixtures and tests according to configuration and component options, or to re-use fixtures across function, class, module, or whole test session scopes.

- **Teardown logic can be easily and safely managed**, no matter how many fixtures are used, without the need to carefully handle errors by hand or micromanage the order that cleanup steps are added.
