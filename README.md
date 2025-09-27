a = int(input("Enter first number: "))
b = int(input("Enter second number: "))
list_a = []
list_b = []
common = []
for i in range(1,a//2,1):
    if a % i == 0:
        list_a.append(i)
for i in range(1,b//2,1):
    if b % i == 0:
        list_b.append(i)
for a in list_a:
    if a in list_b:
        common.append(a)
print("HCF is",max(common))
