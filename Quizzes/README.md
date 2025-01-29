**1. Independent Questions**
   
The *independent-questions* package aims to provide easy-to-customize commands.
The questions are said to be independent because it creates one `Verify` and one `Reset` button for each question.

General remarks.
- Each question is identified by a counter `QuestionNum`. Its value is used to regroup different OCGs for the buttons linked to the possible answers and to the Verify/Reset functions.
- Because most PDF viewers do not deactivate buttons in an invisible OCG, it is not possible to create a single well-behaved button that applies both the Verify and the Reset functions.
By well-behaved, I mean that would suck if the button were to reset your answers when displaying the verification message.
- Single and Multiple answers are treated differently. If there is only one answer, then a RadioButtonGroup prevents the user to check more than one box.
