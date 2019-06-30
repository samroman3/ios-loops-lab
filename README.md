# Loops Lab

## Instructions for lab submission

1. Fork the assignment repo
1. Clone your Fork to your machine
1. Complete the lab
1. Push your changes to your Fork
1. Submit a Pull Request back to the assignment repo
1. Paste a link to of your Fork on Canvas and submit


## Question 1

Write code that prints all the numbers from 1 to 150, **inclusive.**

for index in 1...150 {
print(index)
}
***
## Question 2

Write code that prints all the numbers from 142 to 159, **exclusive.**

for index in 142...<160 {
print(index)
}

***
## Question 3

Write code that prints only the even numbers from 15 to 80, **inclusive.**

for index in 15...80 where index % 2 == 0 {
print(index)
}

***
## Question 4

Write code that prints only the odd numbers from 19 to 51, **inclusive.**
for index in 19...51 where index % 2 != 0 {
print(index)
}
***
## Question 5 TODO

Write code that prints all the numbers that end in a **5** from 1 to 100, **exclusive.**
for index in 1...100 where index % 5 == 0 && index % 2 != 0 {
print(index)
}

***
## Question 6 TODO

Write code that prints all the numbers that end in a 7 from 1 to 40, **inclusive.**


***
## Question 7

Given a range of numbers from 20 to 150 inclusive, print out all the numbers that follows these conditions:

`Numbers that are divisible by 3`

***
for index in 20...150 where index % 3 == 0 {
print(index)
}
## Question 8

Given a range of numbers from 20 to 150 inclusive, print out all the numbers that follows these conditions:

`Numbers that are divisible by 2 and 3`

for index in 20...150 where index % 3 == 0 && index % 2 == 0 {
print(index)
}

***
## Question 9 TODO

Given a range of numbers from 20 to 150 inclusive, print out all the numbers that follows these conditions:

`Numbers that end with a 4`

if num - 

***
## Question 10

Given a range of numbers from 20 to 150, print out all the numbers that follows these conditions:

`Print out numbers: 31, 35, 40 to 60.`
for index in 20...150 where index == 31 || index == 35 || index == 40 || index == 60 {
print(index)
}
***
## Question 11

Without using Xcode, how many times will the loop below run?  Explain why.

```swift
var i = 5

while (i > 3) {
    i += 1
}

// Your explanation here
```
it will run endlessly because it keeps adding 1 to index and will continue to do so without a break

***
## Question 12 

Change the code below to make the loop stop executing when i reaches 9.

```swift
var i = 5
repeat {
i += 1
} while i <= 9

```

***
## Question 13

Change the code below to make the loop stop executing after it has run 1,000 times.

```swift
var i = 5

repeat {
i += 1
} while (i > 3) && (i <= 1004)
```

***
## Question 14

Change the code below to make the loop stop executing after it has run 1,000 times and also make it print out the current value of i **only if i is an even number.**

```swift
var i = 5

repeat {
i += 1
} while (i > 3) && (i <= 1004) ;
if i % 2 == 0 {
print(i)
}
```

***
## Question 15

What's the difference in syntax between the following two while loops?  Will their outputs be different?  Explain why or why not.

```swift
var i = 1
//loop one
while i <= 10 {
    print("i = \(i)")
    i += 1
}

//loop two
var i = 1

repeat {
    print("i = \(i)")
    i += 1
} while i <= 10
```
loop two has a repeat and will execute a single pass before evaluating the condition. They will have the same output. 
***
## Question 16

What's the difference between `break` and `continue`?  Give an example that demonstrates their differences.

``break and continue are used in nested if statements to tell the computer whether to break or continue the loop if a condition is met.

***
## Question 17

Without using Xcode, what will the loop below print? Select all that apply.

```swift
for i in 1...10 {
    if (i >= 4 && i <= 7){
        continue
    }
    print(i)
}
```

[]4
[]5
[]6
[]7

***
## Question 18

Without using Xcode, what will the loop below print? Select all that apply.

```swift
for i in 1...10 {
    if (i >= 4 && i <= 7){
        break
    }
    print(i)
}
```

[]1
[]2
[]3

***
## Question 19

Without using Xcode, what will the loop below print?  Explain below.

```swift
outerloop: for x in 1...3 {
    innerloop: for y in 1...3 {
        if y == 2{
            continue outerloop
        }
        print("x = \(x), y = \(y)")
    }
}



```
outerloop will go through range and print x = 1, x = 2,x=3. while y while only print y = 1 due to the if conditional
***
## Question 20 ?????

Write code that prints out all the points in the area bounded by (0,0), (10,0), (0,10) and (10,10) **where** x and y are both integers.

outerloop: for x in 0...10 {
innerloop: for y in 0...10 {
print("x = \(x), y = \(y)")
}   
}
***
## Question 21

Write code that prints out all the points in the area bounded by (0,0), (10,0), (0,10) and (10,10) **where** the difference of x and y is at least 5, and x and y are both integers.

outerloop: for x in 0...10 {
innerloop: for y in 0...10 {
if (x - y) == 5 || (x - y) == -5 || (x - y) >= 5 || (x - y) <= -5 {
print("x = \(x), y = \(y)")
}
}
}

***
## Question 22

Print the first `N` square numbers. A **square number**, also called perfect square, is an integer that is obtained by squaring some other integer; in other words, it is the product of some integer with itself (ex. 1 = 1*1, 4 = 2 * 2, 9 = 3* 3 …).

Example:
Input: `var N = 5`

Output:
```swift
1
4
9
16
25
```
for i in 1...N {
print(i*i)
}

***
## Question 23

Given an integer N draw a square of N x N asterisks. Look at the examples.

Example 1:
Input: `var N = 2`

Output:
```swift
**
**
```

Example 2:
Input: `var N = 3`

Output:
```swift
***
***
***
```

Hint 1
Try printing a single line of * first.

Hint 2
You can use print("") to print an empty line.

***
