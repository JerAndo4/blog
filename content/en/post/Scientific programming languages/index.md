---
title: Scientific programming languages
subtitle: Today we will talk about scientific programming languages

# Link this post with a project
projects: []

# Date published
date: '2022-05-19T00:00:00Z'

# Date updated
lastmod: '2022-05-19T00:00:00Z'

# Is this an unpublished draft?
draft: false

# Show this page in the Featured widget?
featured: false

# Featured image
# Place an image named `featured.jpg/png` in this page's folder and customize its options here.
image:
  caption: 'Image credit: []()'
  focal_point: ''
  placement: 2
  preview_only: false

authors:
  - admin

tags:
  - 4 week

categories:
  - post 4

---

## **Overview**

There are at least 2 programming languages:

1. Julia programming language

2. GNU Octave programming language

Today we will talk about them.

## **1. Julia**

Julia is a high—level, high-performance free programming language with dynamic typing, created for mathematical calculations. It is also effective for writing general-purpose programs.The syntax of the language is similar to the syntax of other mathematical languages (for example, MATLAB and Octave), but it has some significant differences. Julia is written in C, C++ and Scheme. The standard package includes a JIT compiler based on LLVM, due to which, according to the authors of the language, applications written entirely in the language are practically not inferior in performance to applications written in statically compiled languages like C or C++. Most of the standard library of the language is written in the same language. The language also has built-in support for a large number of commands for distributed computing.

The language is dynamic, but uses JIT compilation. Thanks to this, a high speed of applications written in a "pure" language is achieved, without the use of low-level libraries and vector operations. Overloading of functions and operators (which are actually also functions) is supported, while optionally you can specify the type for function arguments, which is usually not available in dynamically typed languages. This allows you to create specialized versions of functions and operators to speed up calculations. The most appropriate version of the function is selected automatically during execution. Also, thanks to operator overloading, it is possible to create new data types that behave like built-in types.

One of the priorities in the development of the language is the support of distributed computing. There are a large number of standard constructions for parallelizing code.

## **2. GNU Octave**

GNU Octave is a free software system for mathematical calculations using a high—level language compatible with MATLAB.

Octave is an interactive command interface for solving linear and nonlinear mathematical problems, as well as conducting other numerical experiments. In addition, Octave can be used for batch processing. The Octave language operates with arithmetic of real and complex scalars, vectors and matrices, has extensions for solving linear algebraic problems, finding the roots of systems of nonlinear algebraic equations, working with polynomials, solving various differential equations, integrating systems of differential and differential-algebraic equations of the first order, integrating functions on finite and infinite intervals. This list can be easily expanded using the Octave language (or using dynamically loaded modules created in C, C++, Fortran, etc.).
You can use any numbers in the numbered list — it doesn't matter. When converted to HTML or another format, the numbers will become correct and consistent (1, 2, 3, etc.).

Octave is an interpreted programming language. It is similar to C and supports most of the basic functions of the C standard library, as well as basic Unix commands and system calls. On the other hand, it does not support passing arguments by reference (a design feature).

The syntax of the language is very similar to MATLAB, and well-written scripts will run in both Octave and MATLAB.














