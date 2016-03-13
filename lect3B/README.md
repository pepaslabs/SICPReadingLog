# Lecture 3B

https://www.youtube.com/watch?v=X21cKVtGvYk

```
(define deriv
  (lambda (f)
    (lambda (x)
      (/ (- (f (+ x dx))
            (f x))
          dx))))
```

(takes a procedure and returns a procedure)

