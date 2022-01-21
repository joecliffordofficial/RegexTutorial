# Regex Tutorial - Phone Number

<a href = "user-story"></a>

## User Story

```md
AS A web development student
I WANT a tutorial explaining a specific regex
SO THAT I can understand the search pattern the regex defines
```

## Acceptance Criteria

```md
GIVEN a regex tutorial
WHEN I open the tutorial
THEN I see a descriptive title and introductory paragraph explaining the purpose of the tutorial, a summary describing the regex featured in the tutorial, a table of contents linking to different sections that break down each component of the regex and explain what it does, and a section about the author with a link to the author’s GitHub profile
WHEN I click on the links in the table of contents
THEN I am taken to the corresponding sections of the tutorial
WHEN I read through each section of the tutorial
THEN I find a detailed explanation of what a specific component of the regex does
WHEN I reach the end of the tutorial
THEN I find a section about the author and a link to the author’s GitHub profile
```

<a href = "summary"></a>

## Summary

This is a Regex tutorial on how to use an expression to define a phone number! We will be using this expression: 

```
^(\+\d{1,2}\s)?\(?\d{3}\)?[\s.-]\d{3}[\s.-]\d{4}$
```

Below you will find what each piece of the expression means and how it works!

## Table of Contents

- [User Story](#user-story)
- [Summary](#summary)
- [Expression](#expression)
- [Author](#author)

<a href = "expression"></a>

# Expression

```
^(\+\d{1,2}\s)?\(?\d{3}\)?[\s.-]\d{3}[\s.-]\d{4}$
```

## Beginning

^ - This expression begins with the '^' symbol, this matches the beginning fo the string or the beginning of the line if the multiline flag (m) is enabled.

## Capturing group 1

(\+\d{1,2}\s) - '(Everything inside the parenthesis)' This groups multiple tokens tgether and creates a capture group for extracting a substring or using a backreference.

## Escaped character

\+ - This matches a '+' character (char code 43).

## Digit

\d - Matches any digit character (0-9).
  
  ### Quantifer
  
  {1,2} - The Quantifer is a match between 1 and 2 of the preceding token.

## Whitespace

\s - Matches any whitespace character (spaces, tabs, line breaks). 

  ### Quantifer
  
  ? - Match between 1 and 0 of the preceding token.
  
## Escaped character

\( - Matches a '(' character (char code 40).

  ## Quantifer
  
  ? - Match between 1 and 0 of the preceding token. 

## Digit 

\d - Matches any digit character (0-9)
  
   ### Quantifer
   
   {3} - Match 3 of the preceding token. 
   
 ## Escaped character 
 
 \) - Matches a ')' character (char code 41). 

  ### Quantifer
  
  ? - Match between 0 and 1 of the preceding token.
  
## Character Set

[ - Match any character in the set.

  ### Whitespace
  
  \s - Matches any whitespace character (spaces, tabs, linebreaks). 
  
  ### Character 
  
  . - Matches a '.' character (char code 46). 
  
  ### Character 
  
  - - Matches a '-' character (char code 45).
  
] - end character set. 

## Digit 

/d - Matches any digit character (0-9).

  ### Quantifer
  
  {3} - Match 3 of the preceding token.

## Character Set 

[ - Match any character in the set.

    ### White Space
    
    \s - Match any whitespace character (spaces, tabs, linebreaks).
    
    ### Character
    
    . - Matches a '.' character (char code 46).
    
    ### Character 
    
    - - Matches a '-' character (char code 45). 
] - end character set. 
    
  ## Digit
  
  \d - Matches any digit character (0-9).
  
    ### Quantifer
     
    {4} - Match 4 of the preceding token. 
     
 ## End
 
 $ - Matches the end of the string, or the end of a line if the multiline flag (m) is enabled. 

<a href = "author"></a>

## Author

This was a brief tutorial on how a regex expression works! Let me know if you have any questions or any improvements!

You can find me here:

[GitHub](https://github.com/joecliffordofficial)
