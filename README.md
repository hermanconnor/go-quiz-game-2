# Exercise #1: Quiz Game

[![exercise status: released](https://img.shields.io/badge/exercise%20status-released-green.svg?style=for-the-badge)](https://gophercises.com/exercises/quiz)

## Exercise details

This exercise is broken into two parts to help simplify the process of explaining it as well as to make it easier to solve. The second part is harder than the first, so if you get stuck feel free to move on to another problem then come back to part 2 later.

**NOTE:** _CSV files may have questions with commas in them. Eg: `"what 2+2, sir?",4` is a valid row in a CSV. I suggest you look into the CSV package in Go and don't try to write your own CSV parser._

### Part 2

Adapt your program from part 1 to add a timer. The default time limit should be 30 seconds, but should also be customizable via a flag.

Your quiz should stop as soon as the time limit has exceeded. That is, you shouldn't wait for the user to answer one final questions but should ideally stop the quiz entirely even if you are currently waiting on an answer from the end user.

Users should be asked to press enter (or some other key) before the timer starts, and then the questions should be printed out to the screen one at a time until the user provides an answer. Regardless of whether the answer is correct or wrong the next question should be asked.

At the end of the quiz the program should still output the total number of questions correct and how many questions there were in total. Questions given invalid answers or unanswered are considered incorrect.

## Bonus

As a bonus exercises you can also...

1. Add string trimming and cleanup to help ensure that correct answers with extra whitespace, capitalization, etc are not considered incorrect. _Hint: Check out the [strings](https://golang.org/pkg/strings/) package._
2. Add an option (a new flag) to shuffle the quiz order each time it is run.
