---
title       : R objects
description : Manipulate and practice with R most classical objects like vectors, facteors and matrices

--- type:NormalExercise lang:r xp:100 skills:1 key:3b6476edc3
## Operations

R can do operations like any advanced calculator.

*** =instructions
- Add the integers from 1 to 5.
- Compute 2 to the power of 5.
- Compute the sine of $2 \times \pi$.

*** =hint
- Use `+`. Ex: `1+1`.
- Use `^` or `**`. Ex: `2^3`.
- Use `sin` and `pi`. Ex: `sin(pi)`.

*** =sample_code
```{r}
# Add 1, 2, 3, 4 and 5

# Compute 2 to the power of 5

# Compute the sine of 2 pi

```

*** =solution
```{r}
# Add 1, 2, 3, 4 and 5
1 + 2 + 3 + 4 + 5
# Compute 2 to the power of 5
2 ^ 5
# Compute the sine of 2 pi
sin(2 * pi)
```

*** =sct
```{r}
# SCT written with testwhat: https://github.com/datacamp/testwhat/wiki

test_student_typed("1+2+3+4+5",
                   not_typed_msg = "You need to use +")
test_student_typed("2^5",
                   not_typed_msg = "You need to use +")
test_student_typed("sin(2*pi)",
                   not_typed_msg = "You need to use +")
test_error()

success_msg("Good work!")
```

--- type:NormalExercise lang:r xp:100 skills:1 key:d5b1d777d1
## Assignment

Any operation can be assigned to an object that is stored in the current working environment and used for further calculations.

*** =instructions
- `:` is used to create vectors of integers. Try `1:10`
- Assign the result of the previous command to an object called `x` by typing `x <- 1:10`.
- Compute the square of all the integers from 1 to 10 by squaring directly `x`.
- Assign the previous result to a vector called `xsq`.

*** =hint
- Type `1:10`.
- Type `x <- 1:10`.
- Use `^`.
- Use `<-`.

*** =sample_code
```{r}
# Create a vector containing the integers from 1 to 10

# Assign it to x

# Compute x square

# Assign it to y

```

*** =solution
```{r}
# Create a vector containing the integers from 1 to 10
1:10
# Assign it to x
x <- 1:10
# Compute x square
x^2
# Assign it to y
xsq <- x^2
```

*** =sct
```{r}
# SCT written with testwhat: https://github.com/datacamp/testwhat/wiki

test_student_typed("1:10",
                   not_typed_msg = "Just type '1:10'")
test_student_typed("2^5",
                   not_typed_msg = "Just type 'x <- 1:10'")
test_student_typed("x^2",
                   not_typed_msg = "Use ^")
test_student_typed("xsq <- x^2",
                   not_typed_msg = "use ^ and <-")
test_error()

success_msg("Good work!")
```
