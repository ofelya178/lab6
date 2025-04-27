import random

n = int(input('setr;'))  
m = int(input('sutun'))  

A = [[random.randint(-10, 10) for _ in range(m)] for _ in range(n)]

print("Massiv:")
for row in A:
    print(row)

print("\nCəmi mənfi olan sətrlər:")
for i, row in enumerate(A):
    if sum(row) < 0:
        print(f"{i}-ci sətrin cəmi mənfidir.")
