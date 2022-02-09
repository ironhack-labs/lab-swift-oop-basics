
![logo_ironhack_blue 7](https://user-images.githubusercontent.com/23629340/40541063-a07a0a8a-601a-11e8-91b5-2f13e4e6b441.png)

# Lab | OOP Basics

<br>

## Introduction

In this lab, we will create our own fantasy heroes! We will define a class `Character` to describe our fictional video game/movie characters. We will teach them how to wield weapons and spells and compare them with one another!

After completing this lab, you will be able to:

- Create a class with properties, defined with and without default values, as well as optional properties
- Create an init with some of its input parameters having a default value
- Instantiating objects of a class using overloaded inits
- Passing values from one object to a function of another

## Requirements

- Fork this repository.
<!-- - Add your instructor and the class graders to your repository and ensure that your repository is private. Public repositories will receive a zero on the assignment.
  - If you are unsure who your class graders are, ask your instructor or refer to the day 1 slide deck. -->
- Upload the code for all of the following prompts to your repository.

## Submission

- Upon completion, run the following commands:

  ```shell
  git add .
  git commit -m "done"
  git push origin main
  ```

- Create a Pull Request

When you make pull request in pair-programming: `student1,student2-nameOfTheExercise` <br>
When you make a pull request in individual-programming: `student-nameOfTheExercise`

<br>

## Starter code

No starter code needed/provided.

<br>

## Iterations

### Iteration 1

- Create a class `Character` with three properties: `name` (String), `age` (Int) and `race` (String)
- Create an init for all of the properties. In which case properties do not need to be set within the initializer?
- Set the age input parameter within the initializer to have a default value of 100.
- Create a few of your own fantasy characters as objects of a class `Character` (minimum 3). When initializing them, at least one of the objects should use the default age value and at least one should have its age defined manually within the initializer.

### Iteration 2

- Create a function `isOlderThan(age:)` that takes an input parameter and compares it to the class property. Returns Bool value as a result of the comparison if the class property is larger than the input parameter.
- Create a Boolean variable `isOlderThan`. This variable will be used to check if the age of one instance is older than another instance, immediately after the constructor is called. *Hint*: keyword "init" for example.
- Compare the character ages of any of your created `Character` objects at least 2 times and print the results.

### Iteration 3

- Create a new enum `Weapon` and give it a few possible values (like *Sword*, *Mace*, *Axe*, ...)
- Create an optional property `weapon` of type `Weapon` in the class `Character`.
- Create a new class property `knowsSpells` that is a Bool and has a default value `false`.


### Iteration 4

- Create a function `combatStyle` that returns a String.
- Depending on the value of the property `weapon`, return the string stating which weapon the character uses. If the property `weapon` is `nil`, return a string stating that they fight with their fists!

## Iteration 5

- Give at least one of your characters a weapon to fight with. This will be your warrior!
- Teach at least one of your characters how to use spells. This will be your mage!
- Leave one of your characters without either spells or a weapon. This will be your squire!
- Call each of the characters `combatStyle` function and print the result.

## Iteration 6 (Bonus)

- Within the `combatStyle` function, if the property `knowsSpells` is `true`, add a message to your return string saying that the characters also know spells! The previous weapon check logic should still happen regardless of this new logic, so the return string should now have 2 parts - 1 regarding their spell knowledge and the other regarding the weapon they use.
  - For example, a possible return string would be: "The character casts spells! They have no weapon so they fight with their fists!"

<br>

Happy coding! :heart:
