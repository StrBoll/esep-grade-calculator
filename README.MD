# ESEP Grade Calculator

This library is a simple utility to calculate your grades.

The calculataor allows you to set a weight for each category: Assignments, Exams and Essays

Imagine a split like the following: 

Assignments: 30% 
Exams: 35% 
Essays: 35%

The final grade would be calculated by multiplying the average from each category times its weight. 

Let's say the student has a 300/500 for Assignment, a 450/500 for Exams, and a 300/300 for Essays. 

(300/500 x 0.30) + (450/500 x 0.35) + (300/300 x 0.30) = 0.795 or essentially a 79.5%. 

Depending on the letter grade scale, a 79 could be C or C+. The letter grade translation is customizeable to the class/school's standards. 


Runtime requirements:
Golang 1.24+

Run unit tests:
```
cd grade_calculator/
go test ./...
```

Run unit tests with code coverage:
```
cd grade_calculator/
go test -coverprofile=coverage.txt ./...
```