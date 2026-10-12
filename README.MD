# ESEP Grade Calculator

This library is a simple utility to calculate your grades.

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

Project Structure

esep-grade-calculate/
    README.MD
    grade-calculator/
        go.mod #module esep/grade-calculator
        grade-calculator.go #library code
        grade_calculator_test.go #unit tests


Running tests

All commands run from inside grade-calculator/.

 Task                          Command                                   

 Run all tests                 go test ./...                   
 Run with per-test output      go test -v ./...            
 Run a single test             go test -run TestGetGradeA ./...    
 Show coverage percentage      go test -cover ./...    
 Write a coverage profile      go test -coverprofile=coverage.out ./...
 View coverage line-by-line    go tool cover -html=coverage.out

Category         Weight

Assignments      50%   
Exams            35%
Essays           10%

Letter           Score 

A                >= 90
B                >= 80
C                >= 70
D                >= 60
F                < 60

