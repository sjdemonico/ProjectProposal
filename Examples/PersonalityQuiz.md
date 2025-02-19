# Personality Quiz

## Description

This Personality Quiz will help you determine which **INSERT POPULAR TV SHOW**
character you are! Are you more of a **INSERT MAIN CHARACTER'S NAME** or are you
secretly a **INSERT VILLAIN NAME HERE**? Take this quiz to find out today!

## Overview

The purpose of the Personality Quiz is to provide entertainment to the user. The
program outputs questions to the user and accepts their answer as input via the
keyboard. Finally, at the end of the quiz, the program displays the result of
the quiz.

## High Level Design

At a high level, the Personality Quiz works in the following way:

1. Initializes a list of scores to 0 (each score represents one of the possible outcomes)
2. Creates a list of questions and answers (each possible answer will increase
   one of the scores by 1)
3. Loops through each question and
   * Prompts the user to answer the question
   * Increases the appropriate score by 1
4. When all of the questions have been answered, use the highest score to
   display the result of the quiz.

### Flowchart

![Personality Quiz](../images/PersonalityQuiz.png)

## Functions

The Personality Quiz has several complexities. To help manage this, I have
chosen to create a `Question` list as well as breaking my program's logic 
into 3 functions: 

* `AskQuestion(question)`
* `GetValidAnswer(answers);`
* `static string GetResult(scores, results);`

### Question List

For this program, it is important to group together the question and answers. To
manage this, I've created a List of tuples, and each tuple contains: a `Question` string
which will be the question being asked and an `Answers` List which will
be a list of the possible answers to that questions.

![Question Class](../images/PersonalityQuizQuestionClass.png)

### AskQuestion(q)

Displays the specified question along with each of its answers. Then, prompts
the user to select one of the answers. Finally, returns the index of the answer
the player selected.

![Ask Question](../images/PersonalityQuizAskQuestion.png)

1. Display the question
2. Loop through each answer and display it
3. Use the `GetValidAnswer` function to get the user's response
4. Return the user's response


### GetValidAnswer(answers)

Given a list of answers, prompts the user to enter a number corresponding to one
of the answers. If the user enters a number that is not within the specified
range, the user is asked to enter another value.

![Get Valid Answer](../images/PersonalityQuizGetValidAnswer.png)

1. Validate that there is at least 1 possible answer.
2. If the list of answers is empty, throw an exception
3. Otherwise, Display a message asking the user to select an option.
4. Store the user's response in a variable name choice
5. Validate that choice is one of the possible answers
6. If it is not a valid answer
   * Display an error message
   * Go to 3
7. Otherwise, return the user's choice. 

### GetResult(scores, results);

Given two lists, one representing the scores for each possible result and one
representing each possible result, determines which score is the highest and
returns the corresponding string from the results list.

![Get Result](../images/PersonalityQuizGetResult.png)

1. Initialize highest to 0. This variable represents the highest score we have
   seen so far.
2. Initialize highestIx to 0. This variable represents the index of the highest
   score we have seen so far.
3. Loop through each score in scores, tracking the index in a variable currentIx
   * If the score is greater than the highest score
     * Update highest to store the score (this is the highest score we have
       seen so far)
     * Update highestIx to store the currentIx (this is the index of the highest
       score we have seen so far)
4. After we have checked each score, highestIx should be the index of the
   highest score.
5. return results[highestIx];
