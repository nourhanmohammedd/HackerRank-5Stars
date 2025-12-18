

[LOOPS.txt](https://github.com/user-attachments/files/24226270/LOOPS.txt)

n = int(input())
for i in range (0,n):
      print(i*i)

[Nested Lists.txt](https://github.com/user-attachments/files/24226273/Nested.Lists.txt)
n= int(input())
data = []

for i in range(n):
    name = input()
    score = float(input())
    data.append([score, name])

data.sort()

lowest = data[0][0]
second_lowest = None

for score, name in data:
    if score != lowest:
        second_lowest = score
        break

names = []
for score, name in data:
    if score == second_lowest:
        names.append(name)

names.sort()

for n in names:
    print(n)

    
