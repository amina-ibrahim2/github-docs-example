# Writing Good Documentation
## Step 1-Using Codeblocks

Codeblocks in markdown make it *very easy* for tech people to **copy, paste, and share** code. 
A good _Cloud Engineer_ uses codeblocks whenever possible. 

Because it allows others to copy and paste their code to replicate or research issues. 


In order to create codeblocks in markdown you need to use three backticks(where the ~ is on keyboard) Not to confuse with quotation (')

Good Cloud Engineers use codeblocks for both Code and Errors that appear in the console. 

> Here is an example of using a codeblock for an error that appears in bash

```bash
# Define a custom exception class
class CustomError(Exception):
    def __init__(self, message):
        super().__init__(message)

# Example function that raises the custom error
def divide_numbers(a, b):
    if b == 0:
        raise CustomError("Division by zero is not allowed")
    return a / b

# Test the function
try:
    result = divide_numbers(10, 0)
except CustomError as e:
    print(f"Error: {e}")
else:
    print(f"Result: {result}")
```
````
def factorial(n):
    if n == 0:
        return 1
    else:
        return n * factorial(n - 1)

# Test the factorial function
number = 5
result = factorial(number)
print(f"The factorial of {number} is {result}")
```
When you can, you should attempt to apply syntax highlighting to your codeblocks 

````python
```
def factorial(n):
    if n == 0:
        return 1
    else:
        return n * factorial(n - 1)

# Test the factorial function
number = 5
result = factorial(number)
print(f"The factorial of {number} is {result}")
```

````
To add an image: the syntax looks like ![Alt text](image link)

![Map of Africa.pdf](https://github.com/amina-ibrahim2/github-docs-example/files/12705491/Map.of.Africa.pdf)

## Step 3- Use Github Task Lists 

Github extends Markdown to have a list where you can check off items. 

- [x] Finish Step 1 
- [] Finish Step 2
- [] Finish Step 3

## Step 4 -Github Flavored Markdown Emojis 

Github Flavored Markdown (GFM) supports emoji shortcodes. 
Here are some examples: 

| Name | Shortcode | Emoji| 
| -- | -- | -- |
| Cloud | `:cloud:` | ☁
| Cloud with Lightning | `:cloud_with_ligtning:` | 🌩️


## References 
- [Google](www.google.com) <sup>[1]
- [Educative.io](https://www.educative.io/answers/adding-images-to-readmemd-in-github)
- [GFM-Task Lists]()




