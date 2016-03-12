# Lecture 3A

## 2016/3/11

https://www.youtube.com/watch?v=2QgZVYI3tDs

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

https://youtu.be/2QgZVYI3tDs?t=14m59s

```
(define 1-to-4 (list 1 2 3 4))
(define nil '())
```

```
(define (scale s l)
  (if (null? l)
    nil
    (cons (* s (car l))
          (scale s (cdr l)))))
```

```
(scale 10 1-to-4)
```

```
(define (map f l)
  (if (null? l)
    nil
    (cons (f (car l))
          (map f (cdr l)))))
```

```
(define (scale s l)
  (map (lambda (x) (* s x))
       l))
```

```
(define (square x) (* x x))
(map square 1-to-4)
```

```
(map (lambda (x) (+ x 10)) 1-to-4)
```

```
(define (foreach f l)
  (if (null? l)
      nil
      (cons (f (car l))
            (foreach f (cdr l)))))
```

----

https://youtu.be/2QgZVYI3tDs?t=28m28s
