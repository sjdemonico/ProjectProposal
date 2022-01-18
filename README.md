# Project Overview

For this project, you will propose, design, and implement a project of your own
design. To receive a score of **Proficient** in the Computational Thinking
category this project must meet all of the requirements to receive 6 points as
an AP Computer Science Principles project submission.

* Student Handout for AP Project: [LINK](https://apcentral.collegeboard.org/pdf/ap-csp-student-task-directions.pdf?course=ap-computer-science-principles)
* Grading Rubric for AP Project: [LINK](https://apcentral.collegeboard.org/pdf/ap21-sg-computer-science-principles.pdf)
* Several example projects and their scores are available at the bottom of this
  page: [LINK](https://apcentral.collegeboard.org/courses/ap-computer-science-principles/exam)

- [Project Overview](#project-overview)
  - [Part 0: Create a Repository for your Project](#part-0-create-a-repository-for-your-project)
  - [Part 1: Write a Proposal](#part-1-write-a-proposal)
    - [Example Proposals](#example-proposals)
    - [Proficient Requirements](#proficient-requirements)
    - [Advanced Requirements](#advanced-requirements)
    - [Proposal Format](#proposal-format)
      - [Overview](#overview)
      - [High Level Flowchart](#high-level-flowchart)
      - [Methods](#methods)
  - [Part 2: Implement the project (~3 weeks)](#part-2-implement-the-project-3-weeks)
  - [Part 3: Written Response](#part-3-written-response)
  - [Project Ideas](#project-ideas)
    - [Level 1](#level-1)
    - [Level 2](#level-2)
    - [Level 3+](#level-3)

## Part 0: Create a Repository for your Project

Before starting, you should create a repository for your project. If you're not
sure how to do this, you can follow the steps here: [LINK](Setup.md)

Here are the high level steps:

1. Create a new repository (may be private)
2. Add Mx. Collard as a Collaborator
3. Clone the repository
4. Create a development branch
5. Initialize your project
6. Commit and push your initialized project
7. Create a pull request from `develop` to `main` branch
8. Add Mx. Collard as a reviewer

## Part 1: Write a Proposal

First, you will propose a project and create a design document to help you think
through all of the components that you will need to implement. It is very easy
to over scope and start working on a project that is too large to finish. I
recommend starting small, maybe implement a portion of a bigger project and
then, if there is extra time, add more onto it.

### Example Proposals

An example proposal of a guessing game called Wordle is here:
[LINK](Examples/Wordle.md)

An example proposal for a High Score Tracker: [LINK](Examples/HighScoreTracker.md)

### Proficient Requirements

To help you meet the proficient requirement, I've provided a list of additional
requirements that, if done properly should get you very close to a full 6
points.

Your project should meet all of these requirements:

1. Uses a list to store an arbitrary number of elements
2. Accepts user input
3. Has at least one method that:
    * Requires at least 1 parameter
    * Validates the input
    * Throws an exception if the input is not valid
    * Contains a loop that iterates (no `while(false)` loops)
    * Is a significant part of your overall program
4. Iterates over the list from #1. This can be done in your method for #3.

### Advanced Requirements

In your proposal, you must come up with one or more advanced features for
approval. The aim of these features should be to learn something new and
challenge yourself to learn and grow.

### Proposal Format

Your proposal will have 3 main sections: Overview, High Level Flowchart, and
Methods. Below you will find an overview of each section:

#### Overview

Write 3 - 5 sentences explaining your programs purpose and describing the user's
inputs and program's outputs. This will become a guide for the first section of
your written response.

#### High Level Flowchart

Think about what your program must do to accomplish its goal. Draw a high level
flowchart of the entire process from start to finish. In this flowchart, you may
gloss over hard to implement details that you're not sure how to write. This
flowchart should be a high level overview showing how the program transitions
from one part of your program to the next. This will start as a draft and you
will likely make revisions throughout the project to match any changes you make
during implementation.

#### Methods

After you have a high level flowchart of your project, find the complex sections
and break these out to create sub flowcharts. These will be your methods. You
should get as detailed as possible in each of these flowcharts breaking down the
process to the simplest commands. If you find the flowchart becoming complex,
consider breaking it into two or more sub flowcharts that are used to complete
the goal.

For each method flowchart, come up with a method signature and a comment. Use
the following questions as a guide:

1. What data do I need to pass to this method?
2. What are valid inputs?
3. What does the method accomplish?
4. What (if any) does this method return (produce)?
5. At a high level, what does this method do?
6. Based on #5, what is a short name I can give this method?

Finally, in English, write a step-by-step detailed explanation describing how
this method will be implemented.

## Part 2: Implement the project (~3 weeks)

You will receive roughly 4 block periods over the course of 3 weeks of in class
time to work on this project (about 5 hours). This will almost certainly not be
enough time to complete the entire project without coming prepared to class with
questions / specific goals for progress. This is where your student log will
become incredibly important: The expectation is that during these two weeks, you
are spending at least 2 hours of time outside of class each week on your
project.

## Part 3: Written Response

After you have finished your project. You will complete a written response which
matches the format of an AP Project submission. This includes recording a short,
less than 1 minute, video. The response template can be found here:
[LINK](WrittenResponse.md)


## Project Ideas

If you're having trouble coming up with a project idea, you can use any of the
following project ideas. **Note**: Each of the projects could range greatly in
difficulty depending on how it is implemented. However, an attempt to sort them
into difficulty categories was made. You should however take this with a grain
of salt as a Level 1 project could easily become a Level 3+ project without
properly scoping the project. Be sure to talk it through with Mx. Collard to get a
solid idea of how to meet the proficient requirements.

### Level 1

1. A guessing game like Mastermind or Wordle:
   [LINK](https://www.powerlanguage.co.uk/wordle/)
2. A High Score tracker
3. A Random Name Generator: [LINK](images/superhero-name.jpg)
4. A Personality Quiz:
   [LINK](https://ohmy.disney.com/quiz/2014/06/25/quiz-which-disney-princess-are-you/)
5. A binary to hex and hex to binary quiz program
6. Extend the Cipher assignment to use a dictionary to determine the correct
   message
7.  A program that prints text one character at a time (Dialogue System)
8.  A program that prints color text based on the words in the string (Dialogue
    System)
9.  A shopping cart / store in a video game
10. A To Do List
11. A hacker simulator: [LINK](https://hackertyper.net/)
12. A Loot Generator
13. Inspirational quote generator
14. ATM / Bank Account Simulator
15. Prime Number Generator
16. Conway's Game of Life: [LINK](https://playgameoflife.com/)

### Level 2

1. A turn based combat system
2. A MadLibs game
3. A text based adventure
4. A program that predicts the Weather using historical data:
    [LINK](https://www.ncdc.noaa.gov/cdo-web/search)
5. A flash card program for studying
6. A program that counts the number of occurrence of a word / words in a text file
7. A memory game like Simon or Bop-it: [LINK](http://www.freesimon.org/)
8. A Point and Click adventure / Escape Room game
9. An asteroids clone
10. A text template filler (Email Newsletter)
11. Snake game clone
12. Stock Market ticker: [LINK](https://finnhub.io/)
13. A Graphing Calculator to show what a function with a single variable looks
    like
14. Convert a CSV file to a line / bar / pie chart


### Level 3+

1. A Scrabble score calculator
2. A top down 2D game that stores maps as a text file
3. An app that displays the local Weather Forecast by getting live information
    from the internet: (https://openweathermap.org/api)
4. A Tower Defense Game [Tutorial](https://www.youtube.com/watch?v=beuoNuK2tbk&ab_channel=Brackeys)
5. A black jack game
6. Breakout clone
7. Sports Statistics App: [LINK](https://www.thesportsdb.com/)