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
