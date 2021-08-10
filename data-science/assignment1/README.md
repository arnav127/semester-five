#+TITLE: Data Science
#+SUBTITLE: Assignment 1
#+AUTHOR: Seshal Jain
#+OPTIONS: num:nil toc:nil ^:nil
#+DATE: August 6, 2021
#+LATEX_CLASS: assignment
#+EXPORT_FILE_NAME: 191112436

#+begin_src python :tangle src.py
import math
import numpy as np

# Name: Seshal Jain
# DoB: 11/06/2001
# Mobile Number: 7389061102
# Format: DD MM YY YY 73 89 06 11

x = np.array([11, 6, 20, 1, 73, 89, 6, 11])
y = np.array([20, 9, 20, 1, 77, 48, 95, 89])

n = 8

num = n * np.sum(x * y) - np.sum(x) * np.sum(y)
denom = math.sqrt((n * np.sum(np.square(x)) - np.sum(x)**2) * (n * np.sum(np.square(y)) - np.sum(y)**2) )

# Pearson Correlation Coefficient
print(num/denom)
#+end_src

#+RESULTS:
: None
** Output
#+begin_export
0.2653451664681723
#+end_export
