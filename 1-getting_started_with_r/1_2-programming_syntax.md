
## 1.2 Programming Syntax

### Hello World!

When programming, usually the first “program” you’ll learn in a language
is the `Hello World` program. This is essentially teaching you how to
print the phrase “Hello World” to your console. `R` has built-in
**functions** that are essentially bits of code that have been
constructed by developers to help users perform “higher level” tasks.

Let’s take a look at the `Hello World` program:

``` r
print("Hello World!")
```

    ## [1] "Hello World!"

Components to note:

-   The `print()` function will take in a string of characters and
    output it onto the console. While this seems intuitive, that’s
    because R is a higher-level programming language; lower level
    programming languages such as `C` would require 4-6 lines of code
    simply to print this statement!
-   Strings are characterized in `R` via quoted blocks. If you tried to
    run `print(Hello World)`, you’d receive an error because unquoted
    characters imply either functions or variables that you’ve
    previously defined. In this case, `print(Hello World)` would fail
    simply because R would assume `Hello` and `World` are both variables
    with some additional meaning, but there isn’t an operation between
    the two (only whitespace).

### Arithmetic Operations

R can also be seen almost like a custom calculator. You’ll have your
basic arithmetic operators:

    + addition
    - subtraction
    * multiplication
    / division
    ^ exponent

Examples of them in use:

``` r
1 + 2
```

    ## [1] 3

``` r
3 - 8
```

    ## [1] -5

``` r
9 * 8
```

    ## [1] 72

``` r
216 / 4
```

    ## [1] 54

``` r
9 ^ 3
```

    ## [1] 729

### R Scripts

Let’s get started with our first `.R` file. `.R` files are files
formatted to be interpreted using the R language. In RStudio, you can
start a new file in one of two ways:

-   `File --> New File --> R Script`
-   Using the keyboard shortcut `Cmd + Shift + N`, which will open up an
    `Untitled` R script (if you haven’t updated the settings of your
    RStudio view, you’ll see a new pane pop up above your `Environment.`
    This is our `Source` pane, where we can read/edit files).

![](/Users/michaellok4/projects/DSCI101-data-viz/images/1-new_file.png)

### Comments

When you start getting complex with your code, it’s sometimes hard to
remember what you were trying to do when revisiting files. Comments are
helpful to give some context of what is being performed. When you want
to begin a comment, use the `#` symbol. This will ensure that any
characters written on the line after the `#` will not be executed.

Here’s an example of how we can “take notes” on what we’ve learned today
in our new file.

![](/Users/michaellok4/projects/DSCI101-data-viz/images/1-comments.png)

*You’ll notice that our `Untitled1` file has an `**` at the end of the
name in the Source pane. In RStudio, if a file has been changed since it
was opened, the `**` indicates that these changes have not been saved
and helps remind users to save. Saving can be done by going to
`File --> Save` or using the keyboard shortcut `Cmd + S`.*

### Executing Code in R Files

Previously, we’ve been writing code in our console and execute by simply
pressing the `Return` key. If you are in an R file, you can execute code
line-by-line by pressing `Cmd + Return`. If the line your cursor
currently resides on does not have any “code”, R will look for the next
available line/block of code to execute (**examples** looking at the
screenshot of our `Untitled1` file, line 8 has a comment but no code. If
we were to execute that line, R would search for the next available
snippet of code that could be executed, which is at line 9
`print("Hello World!")`).

In summary, there are two shortcuts to remember when executing code:

-   `Cmd + Return` will execute the line of code your cursor is
    currently on.
    -   You can also highlight snippets of code and pressing
        `Cmd + Return` will execute each of those lines.
-   `Cmd + Shift + Return` will execute all the code in your current
    script.
