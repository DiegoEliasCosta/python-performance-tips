This folder stores a set of examples of cythonized code that substantially improved the code's performance.



### Why Cythonize your Code?



I have compiled a set of arguments in favor and against the use of Cython, compared with current solutions for Python code optimization.

#### Numba

1. Numba is focused on speeding up array-oriented and math-heavy Python. Therefore, Numba optimizations rarely scape form this domain, while Cython is able to optimize a **broader range** of Python applications.



#### PyPy

1. PyPy does not offer the same level of **control** that Cython pro‐ vides—PyPy does what it does, and if the speedup is not satisfactory, there is little that can be done. Cython allows the end user to try many different approaches, moving more code into C or C++ to improve performance [1].

   



#### Jit Compilers in General

In general, Cython is **not as easy** to use as JIT compilers, given that it typically relies on inline static type declarations to generate efficient code.

On the other hand, because JIT compilers stress ease of use and work with pure-Python code, they do not provide the same level of **control** that a hybrid language like Cython does. 

* Cython also does not place any runtime dependencies on end users. 





##### References

1 [Cython - A Guide for Python Programmers](http://shop.oreilly.com/product/0636920033431.do)