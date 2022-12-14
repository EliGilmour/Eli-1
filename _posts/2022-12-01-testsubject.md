---
toc: true
layout: post
Badges: true
comments: false
author: Eli gilmour
categories: [fastpages, markdown]
title: Unit section 5-7 Homework
---

# 3.5 Binary Hacks

## Binary Practice
Using psuedocode operators determine if the statements are true or false. The number type will be indicated in parentheses.

**1. 90(D) = 1000(B)**

- A. True
- B. False
Answer = B, number B is larger then number D

**2. 10(D) ≠ 0110(B)**

- A. True
- B. False
Answer = A, because binary D is not equal to B

**3. 56(D) ≥ 111000(B)**

- A. True
- B. False
Answer B, 56 is not equal to B

**3. 99(D) < 1110011(B)**

- A. True
- B. False
Answer = A, because Binary B is larger than binary D

<html>
<style>
    table, th, td { 
        border:2px solid white;
    }
</style>
    <div>AND Operator</div>
    <div>
        <table>
            <tr>
                <th>Value 1</th>
                <th>Value 2</th>
                <th>Result</th>
            </tr>
            <tr>
                <td>1</td>
                <td>1</td>
                <td>1</td>
            </tr>
            <tr>
                <td>1</td>
                <td>0</td>
                <td>0</td>
            </tr>
            <tr>
                <td>0</td>
                <td>1</td>
                <td>0</td>
            </tr>
            <tr>
                <td>0</td>
                <td>0</td>
                <td>0</td>
            </tr>
        </table>
    </div>
    <div>OR Operator</div>
    <div>
        <table>
            <tr>
                <th>Value 1</th>
                <th>Value 2</th>
                <th>Result</th>
            </tr>
            <tr>
                <td>1</td>
                <td>1</td>
                <td>1</td>
            </tr>
            <tr>
                <td>1</td>
                <td>0</td>
                <td>1</td>
            </tr>
            <tr>
                <td>0</td>
                <td>1</td>
                <td>1</td>
            </tr>
            <tr>
                <td>0</td>
                <td>0</td>
                <td>0</td>
            </tr>
        </table>
    </div>
    <div>Not operator</div>
    <div>
        <table>
            <tr>
                <th>Not</th>
                <th>Value</th>
                <th>Result</th>
            </tr>
            <tr>
                <td>Not</td>
                <td>1</td>
                <td>0</td>
            </tr>
            <tr>
                <td>Not</td>
                <td>0</td>
                <td>0</td>
            </tr>
        </table>
    </div>
</html>


# Testing out relational operators
# Practice with these statements

print(20 > 20) # How can you change the operator to print a value of False?

x = 30
y = 20
z = 10
print(x >= y + z) # How can this return true by only manipulating the operator?

# 3.6 Hacks

## AP Prep

**1. What is displayed by this code?**
- result <-- 75
- IF result < 80 {
    DISPLAY("Please schedule a retake.")
}
- ELSE {
    DISPLAY("Nice job!")
}

1. Nice job!
2. Display
3. Please schedule a retake. (answer)
4. 75
(75 is lower than 80)
**2. How is an if statement different from an if-else statement.**

1. Extra words.
2. An if statement will only go through a process if a condition is met. An if-else statement will go through code no matter the conditions. (answer)
3. They are the exact same.
4. An if statement will go through the entire code segment every single time and the if-else statement is always used in an algorithm, no matter the conditions.
(statement must be made in order to go through the code)
**3. What would be most appropriate for this situation? Ben wants to check his bank account. If his car fuel is full, he will go to the bank. Otherwise, he will go home. If he goes to the bank, he will withdraw money only if his balance is above $1000.**

1. If statement
2. If-else statement (answer)
(if he had gas he would go, but no gas means don't go)
**4. What would be most appropriate for this situation? Luke wants to play basketball. If it is sunny outside he will go to the park to play basketball.**

1. If statement (answer)
2. If-else statement
(doesn't say what he's doing when not sunny)
## Using Python

animals = ["lion", "tiger", "wildebeest", "shark", "jellyfish", "blobfish", "raven"]

for i in animals:
    if i == "shark": # What boolean value does this statement cause?
        print("Fun Fact: The smallest shark is the dwarf lantern shark, and it is small enough to hold in your hand!")
    else:
        print(i)
for i in animals:
    if i == "lion" or "wildebeest" or "raven":
        print("This animal lives in the desert")

# Practice
# Using only one more if statement, alter the code to print out a statement saying if an animal lives in the desert, based on booleans


# Write code here
beefWellington = {
    "meat": True,
    "prepTime": 150,
    "name": "Beef Wellington"
}

cheeseQuesadilla = {
    "meat": False, 
    "prepTime": 10,
    "name": "Cheese Quesadilla"

}

chickenAlfredo = {
    "meat": True, 
    "prepTime": 60,
    "name": "Chicken Alfredo"
}

def cookMeal(dish):
    if dish["prepTime"] <= 30: 
        if dish["meat"] == False:
            print("You can cook a", dish["name"])
        else:
            print("Sorry, you do not have meat and cannot cook a", dish["name"] )
    else:
        print("Sorry, you do not have enough time and cannot cook a", dish["name"] )

cookMeal(beefWellington)
cookMeal(cheeseQuesadilla)
cookMeal(chickenAlfredo)

## Exercise 2

Make a flowchart([here](https://www.lucidchart.com/pages/examples/flowchart-maker) is one we used) and write pseudocode for the following scenario.
- Mr. Yeung would like to grade live reviews. 
- He wants to see if each student has at least 2 issues on their project. If they don't they receive a score of 2.0.
- If they have at least 2 issues, check that they have completed at least 5 of their scrumboard tasks.
- If they have completed 5 scrumboard tasks, give the student a 2.7. If they have not completed 5 scrumboard tasks, give them a score of 2.5. If they have completed more than 5 tasks, give them a score of 3.0.
- How much would a student with 3 issues and 1 complete scrumboard task receive?

![photo]({{site.baseurl}}/images/flowchart hacks.png)

# Answer
- The person would recieve a 2.0 because they have three issues which is more than 2, but they can't get more points because they don't have 5 scrumboard tasks completed.