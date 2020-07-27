# Module Project: React Components and Components State - American Football Scoreboard

This project allows you to practice the concepts and techniques learned in this module and apply them in a concrete project. This module explored React components and component state. During the module, you studied what React is, what React components are and how to build them, what state is and how to make a component stateful, and how to change a components state with a click handler. In your project you will demonstrate proficiency of these subjects and principles by creating an application using each of these.

## Introduction

**Read these instructions carefully. Understand exactly what is expected _before_ starting this project.**

### Commits

Commit your code regularly and meaningfully. This helps both you and your team lead in case you ever need to return to old code for any number of reasons.

### Description

In this project, you build an app that displays a scoreboard for an American football game. There will be two buttons for each team - one will increment that team's score by three points (for a "field goal") and the other will increment that team's score by seven points (for a "touchdown" and "extra point"). The css is already done for you. You should focus your efforts on the functionality of the app.

## Instructions

### Task 1: Project Set Up

- [x] Create a forked copy of this project.
- [x] Add your team lead as collaborator on Github.
- [x] Clone your OWN version of the repository in your terminal
- [x] CD into the project base directory `cd american-football-scoreboard`
- [x] Download project dependencies by running `npm install`
- [x] Start up the app using `npm start`
- [x] Create a new branch: git checkout -b `<firstName-lastName>`.
- [x] Implement the project on your newly created `<firstName-lastName>` branch, committing changes regularly.
- [x] Push commits: git push origin `<firstName-lastName>`.

### Task 2a: Minimum Viable Product

1. Hold each team's current score in a state value
2. Render each team's current score that is in state to the DOM.
3. Be able to click the different buttons to increment the appropriate team's score by the correct amount

#### Adding Team Scores to the Component's State

- [x] Import the `useState` hook
- [x] Set up the state values for the Lions team score using the state hook

```js
const [value, setValue] = useState(); // Give these better names, and decide whether you want to pass an initial score into the state hook as the initialValue
```

- [x] Set up the state value for the Tigers team score using a second state hook call

#### Render the Scores to the DOM

- [x] The scores in the JSX are currently hardcoded to 32 points each. Remove the hardcoded values
- [x] Render the state values from what we just set up in steps 1 and 2
- [x] Play around with different initial values to test if they are rendering on the DOM correctly

#### Add Click Functionality to Increment the Scores

- [x] Add the `onClick` handler to each function
- [x] Determine how much you will need to increment the score for each button
  - [x] A touchdown is worth 7 points (assume the following extra point is made)
  - [x] A field goal is worth 3 points
- [ x Inside the click handlers on each button, use the setter functions for each team to increment the appropriate team's score by the correct amount.

### Task 2b: Exit Ticket

Once you begin, you will have 15 minutes to answer the questions [here](https://app.codesignal.com/public-test/R4yNg7CrXix4qryxQ/wrFc7AbwWfnACu).

The completion of these questions is mandatory for MVP. However, passing the quiz doesn't affect your standing as a Lambda School student whatsoever. This is Lambda School testing itself! Please answer honestly and to the best of your ability without using external references.

### Task 3: Stretch Problems

After finishing your required elements, you can push your work further. These goals may or may not be things you have learned in this module but they build on the material you just studied. Time allowing, stretch your limits and see if you can deliver on any the following optional goals:

#### Stretch Goal 1

- [ ] Break out parts of App component into smaller components and compose multiple components together to make the UI
- [ ] Write a "handler" function in App component that takes in a team name and an amount. This function will then be passed to each button's click handler. It will increment the correct team's score by the passed in amount
- [ ] Play around with the styling and make this project your own! Maybe make it a soccer (non-American football) scoreboard, or a rugby or baseball scoreboard
- [ ] Add a button that changes which quarter the game is in, and then render the state quarter value on the scoreboard
- [ ] Make the entire board fully functional with buttons and state! (If you want to make a timer, you'll have to look into useEffect)

#### Stretch Goal 2

Start building a game of **Tic Tac Toe** in React. The positions of the 'Xs' and the 'Os' over time need to be maintained in a slice of state at the top-level component, so that the JSX may display the contents of the 3 x 3 grid correctly. Only empty squares may be selected by the human player, and the event handler that deals with these clicks will have to include quite a bit of logic:

  1. Does the latest move by the human player mean **the game is over**? (Game over, then!)
  1. Is the game **immediately winnable by the computer** by making a certain move? (Do it!)
  1. Can the computer **block the human from winning on their next move** by making certain move? (Do it!)
  
The move by the computer should probably be random if the previous checks turn out negative, but you'll be surprised at how smart the "game engine" will feel.

Have fun!

## Submission Format

* [ ] Submit a Pull-Request to merge `<firstName-lastName>` Branch into `main` (student's  Repo). **Please don't merge your own pull request**
* [ ] Fill out your module retrospective form [here](https://forms.lambdaschool.com/module-retrospective) with a link to your PR
