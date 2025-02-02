# LaTeX
Small packages made to automate specific LaTeX problems

## Quizzes

### Independent Questions
   
The *independent-questions* package aims to provide easy-to-customize commands.
The questions are said to be independent because it creates one `Verify` and one `Reset` button for each question.

General remarks.
- Each question is identified by a counter `QuestionNum`. Its value is used to regroup different OCGs for the buttons linked to the possible answers and to the Verify/Reset functions.
- Because most PDF viewers do not deactivate buttons in an invisible OCG, it is not possible to create a single well-behaved button that applies both the Verify and the Reset functions.
By well-behaved, I mean that would suck if the button were to reset your answers when displaying the verification message.
- Single and Multiple answers are treated differently. If there is only one answer, then a RadioButtonGroup prevents the user to check more than one box.

## Print mode

Have you ever made a fancy presentation with pristine equations and layout, but with so many dark images/background elements that it would be a shame to print it? A partial solution is here to remedy this common issue, whether you're motivated by ink economy and/or ecology.

This small package redefines the usual `\includegraphics` command from the `graphicx` package to allow automatic substitution of an image by a more ink-economic other image with the same content. More precisely, if you put in the same directory an image with path `image.ext`, and a print-optimized image `image-print.ext' (with the suffix `-print`), then the optimized version will be systematically printed. Furthermore, two PDF layers are created to regroup online-only and print-only elements.
