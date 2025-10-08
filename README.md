num = []

for i in range(5):
    value = int(input(f"Enter value {i+1}: "))
    num.append(value)

print("Your list:", num)

# Initialize maxnumber and minnumber to the first element in the list
maxnumber = num[0]
minnumber = num[0]
odd = 0
even = 0

for x in num:
    if x % 2 == 0:
        even += 1
    else:
        odd += 1

    if x > maxnumber:
        maxnumber = x
    if x < minnumber:
        minnumber = x  # Fixed here

print(f"There are {even} even numbers and {odd} odd numbers")
print(f"The maximum number is {maxnumber}")
print(f"The minimum number is {minnumber}")

