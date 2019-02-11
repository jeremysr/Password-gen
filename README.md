# Password-gen
from random import randint
password = []
abc = ['a', 'b', 'c', 'd', 'e', 'f', 'g', 'h', 'i', 'j', 'k', 'l', 'm', 'n', 'o', 'p', 'q', 'r', 's', 't', 'u', 'v', 'w', 'x', 'y', 'z']
numbers = ['0','1','2','3','4','5','6','7','8','9']
special = ['!','#','@','$','%','^','&','*','(',')']
length = int(input("what length do you want: "))
num = 0
while length != num:
    numOrAbc = (randint(1,3))
    if numOrAbc == 1:
        randomAbc = (randint(0,25))
        password.append(abc[randomAbc])
    if numOrAbc == 2:
        randomSpecial = (randint(0,9))
        password.append(special[randomSpecial])
    else:
        randomNum = (randint(0,9))
        password.append(numbers[randomNum])
    num = num + 1
final = ''.join(password)
print(final)
