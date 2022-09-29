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
