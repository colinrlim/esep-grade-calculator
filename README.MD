# ESEP Grade Calculator

A tiny Go library to compute a final course grade from assignments, exams, and essays.  
The final grade is a weighted average of the category averages.  

**Weights (per assignment spec):**  
- Assignments: 50%  
- Exams: 35%  
- Essays: 15%

## Requirements
- Go **1.24+** (module built for 1.24.4)
- Tested on **Go 1.25.1**

## Getting Started
```bash
cd grade-calculator
go test ./...
````

## Code Coverage

```bash
cd grade_calculator
go test -coverprofile=coverage.txt ./...
```

## Grade Scale

* A: >= 90
* B: >= 80
* C: >= 70
* D: >= 60
* F:  < 60

Rounding rule: The final numeric grade is rounded down to the nearest whole number before converting to a letter grade.
Empty categories: Empty categories contribute 0 to the final grade.