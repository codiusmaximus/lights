This repo is designed to serve the two medium articles.

1. [Solving your first linear program in Python](https://towardsdatascience.com/solving-your-first-linear-program-in-python-9e3020a9ad32?source=your_stories_page---------------------------)
2. [How to write a code that solves logical constraints instead of testing them](https://medium.com/@a.bhaskar.is/how-to-write-a-code-that-solves-logical-constraints-instead-of-testing-them-57d7575e8070)

## 1. Solving your first linear program in Python

The notebook **cake.ipynb** contains a full solution of the problem outlined in the article, along with the question posed to the reader, i.e. 'add the equation and break the flour - eggs degeneracy'.

The notebook is written with the following setup

- Python 3.8.2
- SciPy 1.18.1
- Numpy 1.4.1
- Cvxopt 1.2.3 (optional)

## 2. How to write a code that solves logical constraints instead of testing them

This post aims at solving a simple logic puzzle in Python without writing a loop. The puzzle is paraphrased below.

A person goes to a carousel operator at the fair. The carousel operator tells him that anyone who can guess what happens to the 5 lights when he turns on all 5 swtiches gets free rides for life. The 5 switches do the following:

1. Turns on red when yellow is on
2. Red and green are never on together
3. Blue and green can only be on and off together
4. Blue and purple can not be off at the same time
5. If purple is on, blue and yellow have to be on

One can arrive to the with some logical ballet, and the answer is that blue and green are always on when the operator throws all 5 switches together.

The Python setup is the same as in the previous case and the notebook is called **milp_carousel.ipynb**.

