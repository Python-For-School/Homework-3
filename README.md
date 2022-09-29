# Homework-3

### Assignment 1:

```py
numOfStudents = int(input("Enter amount of students "))
weights = []

for index in range(numOfStudents):
    weights.append(int(input("Enter weight of student {}: ".format(index))))

min = max = weights[0]
for index in range(numOfStudents):
    if weights[index] > max: 
        max = weights[index]
    if (weights[index] < min):
        min = weights[index]
print(max - min)
```
### Assignment 2:

```py
scores = []
identicalThrows = 0

for index in range(8):
    scores.append(int(input("Enter points scored in throw - {}: ".format(index))))
for index in range(6):
    if scores[index] == scores[index + 1]:
        identicalThrows += 1
print(identicalThrows)
```
### Assignment 3:
```py
numbers = []

for index in range(10):
    numbers.append(int(input("Enter a digit: ")))
for index in range(10):
    appearences = 0
    for iteration in range(9):
        if numbers[iteration] == index:
            appearences += 1
    print("Appearences for number {} are: {}".format(index, appearences))
```
```py
numbers = []

for index in range(15):
    numbers.append(int(input("Enter a digit: ")))
maxappearences = 0
appearednumber = 0
for index in range(10):
    appearences = 0
    for iteration in range(9):
        if numbers[iteration] == index:
            appearences += 1
    if (appearences > maxappearences):
        maxappearences = appearences
        appearednumber = index
print("number {} has appeared: {} times".format(appearednumber, maxappearences))
```
