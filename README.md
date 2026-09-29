# 29.092026
exercise 4 
for i in range(26):
    print(repr(chr(97 + i)), 97 + i, repr(chr(65 + i)), 65 + i)
    exercise 5 
x = int(input())
y = int(input())
M = max(x, y)
m = min(x, y)
r = M % m 
while r != 0:
    M = m
    m = r
    r = M % m
    print(m)
exercise 6 
n = int(input())
a = int(input())
asc = True
desc = True
for i in range(n - 1):
    b = int(input())
    if b <= a:
        asc = False
    if b >= a:
        desc = False
    a = b
if asc:
    print("ascending sequence")
elif desc:
    print("descending sequence")
else:
    print("neither ascending nor descending sequence")
    exercise7
    n = int(input())
a = float(input())
b = float(input())
max1 = max(a, b)
max2 = min(a, b)
for i in range(n - 2):
    x = float(input())
    if x > max1:
        max2 = max1
        max1 = x
    elif x > max2:
        max2 = x
print(max1, max2)
