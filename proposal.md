Formalizing System Fc in Coq
============================

System Fc is an extension to System F which adds support for non-syntactic type equality.
That is, type A 

From the introduction to [Sulzmann, et al. '07][1]: 
> There are two main extensions:
> (i) explicit witnesses for type equalities, and
> (ii) open, non-parametric type functions, given meaning by top level equality
>      axioms.
> Unlike System F, Fc is expressive enough to serve as a target for several
> different source-language features, including Haskell's newtype, generalised algebraic
> datatypes, associated types, functional dependencies, and perhaps more besides.

This has since been implemented as the core language for GHC, and prompted the
major version bump between 7.* and 8. 
The goal of this project is to formalize this work in Coq. A [senior engineering project][2] at UPenn
undertook a similar project in 2015.

[1]: https://pdfs.semanticscholar.org/b49e/9c2d00acd25ada608170c3c3485880261980.pdf
     "System F with Type Equality Coercions. Sulzmann, Chakravarty, Jones, Donnelly. 2007."
          
[2]: http://www.seas.upenn.edu/~cse400/CSE400_2014_2015/reports/11_report.pdf 
     "Verification of System FC in Coq. Garsys, Mandel, Peña, Zilberstein"
