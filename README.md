# HW

def array(age):
    nums = []
    while age > 0:
        b = age % 10
        nums.append(b)
        age //= 10
    return(list(reversed(nums)))

age = int(input('Введіть свій рік: '))
a = array(age)

if len(set(a)) != len(a):
    print('Який цікавій вік')
else:
    print('А білетів вже не має')

if age < 7:
    print("Де твої батьки?")
if age < 16:
    print("Це фільм для дорослих")
if age > 65:
    print("Покажіть пенсійне посвідчення")
