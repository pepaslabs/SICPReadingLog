# 2015/12/6

## 1

Quote by John Locke:

The acts of the mind are:
* composition of ideas
* relation of ideas to one another
* abstraction of ideas

concepts:

* computational process
* data
* program
* debugging
* modularization

### Programming in Lisp

concepts:

* Lisp
* interpreter
* atoms & lists
* Scheme
* Lisp evolution and dialects
* performance
* procedures
  * can be manipulated as data

## 1.1 The Elements of Programming

# 2016/2/29

## Exercise 1.1

Console output from `scm` interpreter:

```
> 10
10
> (+ 5 3 4)
12
> (- 9 1)
8
> (/ 6 2)
3
> (+ (* 2 4) (- 4 6))
6
> (define a 3)
#<unspecified>
> (define b (+ a 1))
#<unspecified>
> (+ a b (* a b))
19
> (= a b)
#f
> (if (and (> b a) (< b (* a b))) b a)
4
> (cond ((= a 4) 6)
> ((= b 4) (+ 6 7 a))
> (else 25))
16
> (+ 2 (if (> b a) b a))
6
> (* (cond
> ((> a b) a)
> ((< a b) b)
> (else -1))
> (+ a 1))
16
```
