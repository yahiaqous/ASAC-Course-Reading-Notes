# Data Analysis with Python (Jupyter Lab & NumPy)

## Jupyter Lab

JupyterLab is a next-generation web-based user interface for Project Jupyter. It enables to work with documents and activities such as **Jupyter notebooks**, **text editors**, **terminals**, and **custom components** in a flexible, integrated, and extensible manner.

Documents and activities integrate with each other, enabling new workflows for interactive computing, for example:

- **Code Consoles** provide transient scratchpads for running code interactively, with full support for rich output.

- **Kernel-backed documents** enable code in any text file (Markdown, Python, R, LaTeX, etc.) to be run interactively in any Jupyter kernel.

- **Notebook cell outputs** can be mirrored into their own tab, side by side with the notebook, enabling simple dashboards with interactive controls backed by a kernel.

- **Multiple views of documents** with different editors or viewers enable live editing of documents reflected in other viewers.

&nbsp;

## NumPy: Data Analysis with Python

NumPy is a **Python package** for data analysis. It stands for **"Numerical Python"**. It is a library consisting of multidimensional array objects and a collection of routines for processing of array.

NumPy can speed up the workflow, and interface with other packages in the Python ecosystem, like scikit-learn, that use NumPy under the hood.

Using NumPy, a developer can perform the following operations:

- **Mathematical and logical** operations on arrays.

- **Fourier transforms and routines** for shape manipulation.

- **Operations related to linear algebra**. NumPy has in-built functions for linear algebra and random number generation.

The most important object defined in NumPy is an N-dimensional array type called **ndarray**.

NumPy array can be created by using the numpy.array function. If we pass in a list of lists, it will automatically create a NumPy array with the same number of rows and columns.

### **Data Type Objects (dtype)**

A data type object describes **the interpretation of a fixed block of memory corresponding to an array**, depending on the following aspects:

- **Type of data** (integer, float, or Python object)

- **Size of data**

- **Byte order** (little-endian or big-endian)

- In the case of structured type, **the names of fields, the data type of each field, and part of the memory block taken by each field**.

- If the data type is a subarray, **its shape, and data type**
