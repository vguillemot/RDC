---
title       : R objects
description : Manipulate and practice with R most classical objects like vectors, facteors and matrices

--- type:NormalExercise lang:r xp:100 skills:1 key:3b6476edc3
## Operations

R can 

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
