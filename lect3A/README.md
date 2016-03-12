# Lecture 3A

https://www.youtube.com/watch?v=2QgZVYI3tDs

## 2016/3/11

(this is everything I typed into my interpreter while watching the lecture)

```
(define (+vect v1 v2)
  (make-vector
    (+ (xcor v1) (xcor v2))
    (+ (ycor v1) (ycor v2))))
```

```
(define (scale s v)
  (make-vector (* s (xcor v))
               (* s (ycor v))))
```

```
(define make-vector cons)
(define xcor car)
(define ycor cdr)
```

```
(define make-segment cons)
(define seg-start car)
(define seg-end cdr)
```

```
(make-segment (make-vector 2 3)
              (make-vector 5 1))
```

```
(cons (cons 1 2) (cons 3 4))
```

```
(cons (cons 1 (cons 2 3)) 4)
```

```
(define nil '())
(cons 1 (cons 2 (cons 3 (cons 4 nil))))
```

```
(list 1 2 3 4)
```

```
(define 1-to-4 (list 1 2 3 4))
```

```
(car (cdr 1-to-4))
```

```
(car (cdr (cdr 1-to-4)))
```

## 2016/3/12

