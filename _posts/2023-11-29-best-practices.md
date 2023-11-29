---
layout: post
title: Coding Best Practices
date: 2023-11-29
tags: general-skills
---

`"If you make something up, make sure to stick with it" - Asher`
`"You can break laws… you’ll just face consequences" - Jakob`

# Communicating

In software engineering, you are beholden to yourself, your team, and no-one else. While you don’t have to listen to official standards (they are still helpful), you do have to listen to your teammates.

Before you get too far into a project, make sure your group has a standard convention (a set of rules governing code syntax). Having a consistent convention makes it easier to read, edit, and debug code, especially when it isn’t yours. As a result, convention is extremely important in group projects. 

When you are working on a short project alone, however, you can disregard most of these rules without any serious consequence.

# Comments

## Casual commenting

Generally speaking, comments are meant to (1) explain what is not intuitive or difficult to understand and (2) warn of any oddities to watch for (3) provide structure for layout and if something needs to be filled in.

Beware of overcommenting. If what a function does is simple and short, there is no need to comment.

## (More) professional commenting

Most major coding languages have API documentation generators that create documentation from comments. All of them have slightly different syntax for taking comments and generating documentation.

When using an API documentation generator, generally you should put a block quote for every class, method, and function. The comment should include a brief sentence on the code’s purpose, a list of inputs or parameters with types, a list of returns with types, explanations of any specific behaviors (like what happens if it receives empty values), and a bit on how complex parts of it work if necessary.

If you find yourself writing extremely long comments, your function is too large and should be broken up.
Variables
Your variables names should be both descriptive and concise. You should be able to tell the use of the variable from just the name, but you don’t want to write a paragraph every time you use a variable. Long names make code hard to read and hard to write.

The exact format of a variable name depends on your language and preferences. Some common formats include:

- PascalCase (UpperCamelCase)
- camelCase (lowerCamelCase)
- snake_case
- SCREAMING_SNAKE_CASE
- kebab-case

Camel case is used in most languages, including JS, while snake case is used in primarily Python.

Variable names can convey information about the type of a variable. For example, classes are often distinguished from regular variables by using pascal case instead of camel case or snake case. Additionally, underscores at the start of a name normally show that a variable in a class (an attribute) is a private variable.

You should often also notate the specific type of a variable (integer, character, etc.) when creating it, either with type hints (where allowed, such as in Python), or more commonly by declaring a variable as a specific type (these are generally required in languages that allow them and you should use them as much as possible).

Variable declarations should also tell the reader whether a variable will change or not. This is done in most languages by making a variable a constant and making the variable’s name fully uppercase. Many languages with looser variables, such as Python, use only the second method.

One of the most important aspects of managing variables is getting rid of them. Your code should only save a variable as long as is necessary: don’t make a variable global when it should be local.

Let’s say we are coding in Javascript and need to return the nth value in the fibonacci sequence. We need a variable to store the current value in the sequence, which we will be naming here. The declaration will look like this:

`var currentFibonacciNumber = 1;`
or
`var currNum = 1;`

Since this is not a function and we will be changing the variable in Javascript, we will be using lowerCamelCase.

This declaration will be inside the function, so the variable is cleared as soon as it is no longer needed.

Either of these are okay. Which you choose comes down to personal preference.

# Using Whitespace

There has been a perennial war among coders online on whether to use tabs or spaces for indentation. In practice, the problem has been essentially solved: use an editor like VS Code which will automatically convert tabs to spaces.

Another issue then is how many spaces to use for an indent. Typically four spaces per indent is nice but some indent-heavy languages like HTML and CSS prefer two spaces per indent. Ultimately, it comes down to preference.

Use blank lines to separate out code such as between functions, declaring different types of variables, separating imports, etc. This makes it easier to read rather than staring at massive, confusing blocks. Spacing out sections of code like this also pairs well with commenting.

Additional resource: avoiding excessive nesting [https://youtu.be/CFRhGnuXG-4](https://youtu.be/CFRhGnuXG-4)

# Linting and Code Formatters

Most code editors will have add-ons to format your code and ensure it follows given style guides. It is highly recommended to use them for larger projects. In fact, certain frameworks will give you the option to add a linter during setup.

# Optional Homework

For this week’s homework, you will be trying out a standard. To do so, we recommend following these steps:

- Find a standard for your preferred language. We have a few common ones here, but you will be able to find one for nearly any language.
  - Python: [https://peps.python.org/pep-0008/](https://peps.python.org/pep-0008/)
  - JS: [https://google.github.io/styleguide/jsguide.html](https://google.github.io/styleguide/jsguide.html)
- Skim the standard, making sure you can answer the following questions at minimum:
- How does the standard name variables? Functions?
- How many spaces does the standard use?
- Sign up for LeetCode at [https://leetcode.com/](https://leetcode.com/). This site was made to help practice competitive programming, but it is also good for general practice.
- Try problem 118 at [https://leetcode.com/problems/pascals-triangle/](https://leetcode.com/problems/pascals-triangle/) and use the style from your standard.
- Once your solution works, go back and write comments. Don’t fill the file, but make sure the code is understandable.
- Try other problems on LeetCode
