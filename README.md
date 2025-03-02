# Control Flow Lab

## Instructions for lab submission

1. Fork the assignment repo
1. Clone your Fork to your machine
1. Complete the lab
1. Push your changes to your Fork
1. Submit a Pull Request back to the assignment repo
1. Paste a link to of your Fork on Canvas and submit

## Question 1

What will be printed when the code below is run?  Select all that apply.

```swift
let conditionOne = !(4 < 5) || !(3 > 8)
let conditionTwo = !(!true)

if conditionOne {
 print("A")
} else if conditionTwo {
 print("B")
}
if conditionTwo {
 print("C")
}
print("D")
```

- A
- B
- C
- D

answer below: 

A, C, D
***
## Question 2

What will the code block below print?  Select all that apply:

```swift
let appInfo = (name: "myCoolApp", version: 0.4)
switch appInfo {
 case (_, 0.0..<1.0):
 print("\(appInfo.0) hasn't released yet")
 case ("myCoolApp", _):
 print("Thanks for looking at myCoolApp!")
 default:
 print("I'm not quite sure what you are looking at")
}
```

- appInfo.0 hasn't released yet
- myCoolApp hasn't released yet
- Thanks for looking at myCoolApp!
- I'm not quite sure what you are looking at
- It will give a compile-time error

answer below:

myCoolApp hasn't released yet


***
## Question 3

What will be printed to the console when the code below is run?  Select all that apply.

```swift
let x: Int = 4
switch x {
case 0..<4:
 print("A")
case 5..<10:
 print("B")
case is Double:
 print("C")
default:
 print("D")
}
```

- A
- B
- C
- D

answer below:

D

***
## Question 4

What are the errors in the code below for the switch statement? Select all that apply.

```swift
let candyType : String = "skittles"

switch candyType {
case "mAndM":
 print("Melts in your mouth, not in your hand")
case "skittles":
 print("Taste the rainbow")
case "snickers":
 print("Hungry? Grab a Snickers")
}
```

- No parentheses around the conditions
- No opening and closing brackets in each of the cases
- No default case in the switch statement
- No print statement right outside the switch statement

answer below:

- No default case in the switch statement


***
## Question 5

Given the current weather conditions (rain, sunny, snow), use a switch statement to print an appropriate message to the user

```swift
let currentWeather = "rain"

// enter code below

switch currentWeather {
case "rain" :
    print("It's currently raining today.")
case "sunny":
    print("It's currently sunny today.")
case "snow":
    print("It's currently snowing today.")
default:
    print("No clue what weather you're having.  Good luck mate.")
}

```

***
## Question 6

Given the first name and last name of a Fellow, declare `fullName` variable and use string interpolation to concatenate the Fellow's full name and print to the console e.g The Fellow's full name is John Appleseed

```swift
let firstName = "John"
let lastName = "Appleseed"

// enter code below

let fullName = "\(firstName)" + " \(lastName)"
print (fullName)
```

***

## Question 7

Convert the if/else statement below into a switch statement.

```swift
if temperatureInFahrenheit <= 40 {
 print("It's cold out.")
} else if temperatureInFahrenheit >= 85 {
 print("It's really warm.")
} else {
 print("Weather is moderate.")
}

//Re-written statement here

switch temperatureInFahrenheit {
case ...40:
    print("It's cold out.")
case 85...:
    print("It's really warm out.")
default:
    print("Weather is moderate.")
}

```

***

## Question 8

Complete the following code so that "You win!" is printed.

```swift
if {
 print("You win!")
} 
else {
 print("You lose!")
}

answer below: 

let badNews = "Someone stole your bike."

if badNews == "Someone stole your bike." {
    print("You win!")
} else {
    print("You lose!")
}
```
***

## Question 9

Given a variable called numberOfSides, write code using a switch so that it prints out the name of the shape. Account for shapes with 3 to 10 sides and print an error message if out of range.

var numberOfSides = 6

```swift
Example 1:

Input:
var numberOfSides = 4

Output:
Square

Example 2:

Input:
var numberOfSides = 2

Output:
Error

answer below:

switch numberOfSides {
case 3:
    print("Triangle.")
case 4:
    print("Quadrilaterals.")
case 5:
    print("Pentagon.")
case 6:
    print("Hexagon.")
case 7:
    print("Septagon.")
case 8:
    print("Octagon.")
case 9:
    print("Nonagon.")
case 10:
    print("Decagon.")
default:
    print("Out of range.")
}


```
***

## Question 10

Create a switch statement that will convert a number grade into a letter grade as shown below:

```swift
Numeric Score 	Letter Grade
100 	A+
90 - 99	A
80 - 89	B
70 - 79 	C
65 - 69 	D
Below 65 	F

answer below:

let numberGrade = 92
let letterGrade : String

switch numberGrade {
case 100:
    letterGrade = "A+"
case 90...99:
    letterGrade = "B"
case 80...89:
    letterGrade = "C"
case 70...79:
    letterGrade = "D"
case 65...69:
    letterGrade = "E"
default:
    letterGrade = "F"
}

```
***

## Question 11

What is wrong with the block of code below?  Correct it so it behaves as expected.

```swift
let firstName = "Peter"

if firstName == "Peter" {
 let lastName = "Gabriel"
} else if firstName == "Phil" {
 let lastName = "Collins"
}
let fullName = firstName + " " + lastName

answer below:

let firstName = "Peter"
var lastName : String = ""

if firstName == "Peter" {
    lastName = "Gabriel"
} else if firstName == "Phil" {
    lastName = "Collins"
}

let fullName = "\(firstName)" + " " + "\(lastName)"


```
***

## Question 12

Write an if statement that prints out what decade of life someone is in (e.g "You are in your twenties). Then, write it as a switch statement.

```swift
let nameAndBirthYear: (String, Int)

answer below: 

let nameAndBirthYear = (name: "Ahad", year : 1997)
if nameAndBirthYear.year < 2010 && nameAndBirthYear.year > 2000 {
    print("You're in your tens.")
} else if nameAndBirthYear.year < 2000 && nameAndBirthYear.year > 1990 {
    print("You're in your twenties.")
} else if nameAndBirthYear.year < 1990 && nameAndBirthYear.year > 1980 {
    print("You're in your thirties.")
} else if nameAndBirthYear.year < 1980 && nameAndBirthYear.year > 1970 {
    print("You're in your fourties.")
} else {
    print("You're too old.")
}

switch nameAndBirthYear.year {
case 2000..<2010:
    print("You're in your tens.")
case 1990..<2000:
    print("You're in your twenties.")
case 1980..<1990:
    print("You're in your thirties.")
case 1970..<1980:
    print("You're in your fourties")
default:
    print("You're too old.")
}

```
***


## Question 13

Consider the below switch statement. What should your system currently print?

```swift
let number = 42

switch number {
case 365:
 print("Days in year")
case 1024:
 print("Bytes in a Kilobyte")
case 0:
 print("Where arrays start")
case 42:
 print("The answer to life, the universe and everything")
default:
 print("Some uninteresting number")
 
 answer below:
 
 The answer to life, the universe and everything.
```
What happens when you change number to:

-a. 365?

-b. 1024?

-c. 65?

answer below:

a. Days in year
b. Bytes in a Kilobyte
c. Some uninteresting number

What happens when you remove the default clause?

answer below:

you get an error : switch must be exhaustive.

***


## Question 14

Consider the variable below called population and the if-condition.

a. Add an else-if-condition that states if population is less than 10000 but greater than 5000, then message changes to say it's "a medium size town".

b. Add an else-condition where message changes to say it's a mid-size town.

c. Convert your final if-else statement to a switch statement.

```swift
var population: Int = 10000
var message = String()

if population > 10000 {
 message = "\(population) is a large town"
}

answer below:

if population > 10000 {
 message = "\(population) is a large town"
} else if population < 10_000 && population > 5_000 {
    print("\(population) is a medium size town.")
} else {
    print("\(population) is a mid-size town.")
}

switch population {
case 10_000:
    print("\(population) is a large town.")
case 5_001..<10_000:
    print("\(population) is a medium size town.")
default:
    print("\(population) is a mid-size town.")
}
```
***

## Question 15

Complete the code below so that it prints out and tells the user if the sum of the two numbers in the tuple is at least 15.

a. Using a conditional

b. Using a switch statement

```swift
let myTuple: (Int, Int) = (5, 10)

answer below:

print(myTupleSum >= 15 ? "Sum of the numbers in the tuple is at least 15" : "Sum is less than 15")

switch myTupleSum {
case 15...:
    print("Sum of the numbers in the tuple is at least 15")
default:
    print("Sum is less than 15.")
}


```

***
