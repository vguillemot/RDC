---
title       : Control-flow constructs in R
description : Practise with conditional statements (if, then, else) and loops (for, while)

--- type:NormalExercise lang:r xp:100 skills:1 key:5d5d437f54

## Conditions

Conditional statements are highly used in computer programming.
It is necessary to know how to use them to understand and to write an R program.

*** =instructions
- Randomly assign to `x` a value between 0 and 1.
- If this value is greater than 0.5, print the following message: "x > 0.5".

*** =hint
- Use `runif`.
- The syntax for the `if` statement is the following: `if (boolean) instruction`.

*** =sample_code
```{r}
# Generate a random value between 0 and 1

# If x is greater than 0.5, print "x > 0.5"

```

*** =solution
```{r}
# Generate a random value between 0 and 1
x <- runif(1)
# If x is greater than 0.5, print "x > 0.5"
if (x > 0.5) print("x > 0.5")
```

*** =sct
```{r}
# SCT written with testwhat: https://github.com/datacamp/testwhat/wiki

test_function("runif", args="1") # to check whether runif was correctly used
test_object("x") # to check whether x was correctly defined

test_if_else(if_cond_test = test_student_typed(c("x > 0.5","x>0.5")), 
  if_expr_test = test_function("print", "x > 0.5")) 
success_msg("Good work!")
```

--- type:NormalExercise lang:r xp:100 skills:1 key:d055601343
## Loops

Loops are ubiquitous in statistical algorithms and programming.
They allow to explore and create multidimensional objects through a fixed (or not) number of iterations.

*** =instructions
- With a `for` loop, print the integers from 1 to 5

*** =hint
- The syntax for the `for` statement is the following: `for (i in 1:n) instruction depending on i`.

*** =sample_code
```{r}
# Use a for loop to print integers

```

*** =solution
```{r}
# Use a for loop to print integers
for (i in 1:5) print(i)
```

*** =sct
```{r}
# SCT written with testwhat: https://github.com/datacamp/testwhat/wiki

test_for_loop(cond_test = test_student_typed("in 1:5",
                                             not_typed_msg = "You can use `i in 1:5` to define your for loop."),
              expr_test = test_function("print", "x", eval = FALSE),
              not_found_msg = "Make sure to code a for loop in the first place!")
success_msg("Good work!")
```
