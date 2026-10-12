# ESEP Grade Calculator

This library is a simple utility to calculate your grades.

The calculataor allows you to set a weight for each category: Assignments, Exams and Essays

Imagine a split like the following: 

Assignments: 50% 
Exams: 35% 
Essays: 15%

The final grade would be calculated by multiplying the average from each category times its weight. 

Let's say the student has a 300/500 for Assignment, a 450/500 for Exams, and a 300/300 for Essays. 

(300/500 x 0.50) + (450/500 x 0.35) + (300/300 x 0.15) = 0.765 or essentially a 76.5%. 


The letter grades are as follows:

A >= 90 
B >= 80
C >= 70
D >= 60
F < 60

Passing requires a C or better. 


A 76.5 would therefore be translated as a C, passing grade. 

Runtime requirements:
Golang 1.24+

Run unit tests:
```
cd grade-calculator/
go test ./...
```

Run unit tests with code coverage:
```
cd grade-calculator/
go test -coverprofile=coverage.txt ./...
```