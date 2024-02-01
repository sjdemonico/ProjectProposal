# Part 2.1: Implement Function Stubs

By now, you should have completed at least one draft of your project proposal.
The first thing you should do for your project is to create "stubs" for the
functions you will write. This will allow you to start testing each of your
components independently of each other.

If you're having trouble remembering how functions work, you can review them in CodeHS:
[LINK](https://codehs.com/lms/assignment/71997567)

## 1. For each function in your proposal, create a function stub

Next, take each function flowchart and write a function stub for your project.

### Example: GetRandomWord()

For example, in the [Wordle](Examples/Wordle.md) proposal we have the following function flowchart:

![Get Random Word](images/GetRandomWord.png)

This function has 0 parameters and returns a `string`. The function stub will look
like this:

```python
def GetRandomWord()
    return 0
```

Then, add in the algorithm steps you wrote as comments within the function. These
will be TODO steps for you to finish the function:

```python
def GetRandomWord()
   # 1. Load a filed called `words.txt`
   # 2. Store each line as a separate word in a list named `words`
   # 3. Generate a random number between 0 and `len(words)` and store the result in
   #    a variable called `ix`
   # 4. Return the word at position `ix`. (e.g. `words[ix]`)
    return 0
```

### Example: FindInsertionPoint(values, newScore)

For example, in the [High Score Tracker](Examples/HighScoreTracker.md) proposal
we have the following function flowchart:

![Find Insertion Point](images/HighScoreTracker-FindInsertionPoint.png)

This function has 2 parameters and returns an `int`. The function stub will look
like this:

```python
def FindInsertionPoint(values, newScore)
    return -1
```

Then, add in the algorithm steps you wrote as comments within the function. These
will be TODO steps for you to finish the function:

```python
FindInsertionPoint(values, newScore)
    # 1. Initialize a counter variable, insertAt, to 0.
    # 2. Loop through each value in values
    #    * If the new score is greater than the current value, we should insert above
    #      that score so we return `insertAt`.
    #    * Otherwise, the new score should not be inserted above this score so we
    #      increment `insertAt` by 1 and continue.
    # 3. If we reach the end of the list, `insertAt` should be the length of the list
    #    so we return `insertAt`.
    return -1
```

## 3. Add a Documentation Comment to Each of your Functions

Finally, you should add a documentation comment to each of your functions. If you
completed your proposal function section, these should be straight forward.

For example, in the [Random Name
Generator](Examples/Random%20Name%20Generator.md) proposal there is a function
called `GetPositiveInt(prompt)` which accepts a string and returns an
`int`. The documentation comment for this function would look like this:

```python
# <summary>
# Given a prompt to show to the user, displays the prompt then reads
# input from the keyboard until the user enters a positive number. If
# the user enters a non-positive number, this function displays an error
# message and prompts the user again.
# </summary>
# <param name="prompt">The message to display to the user</param>
# <returns>The positive number the user chose</returns>
def GetPositiveInt(prompt)
    return -1
```

