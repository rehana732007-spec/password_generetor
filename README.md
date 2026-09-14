import random
letters=['q','w','e','r','t','r','t','y','u','i','o','p','a','s','d','f','g','h','j','k','l','z','x','c','v','b','n','m',
         'Q','W','E','R','T','Y','U','I','O','P','A','S','D','F','G','H','J','K','L','Z','X','C','V','B','N','M']
numbers=['1','2','3','4','5','6','7','8','9','0']
symbles=['!','@','#','$','%','^','&','*','(',')','_','-','+','/','{','}']
print("Welcome to password generator:")
n_letters=int(input("Enter the letter:"))
n_numbers=int(input("Enter the numbers:"))
n_symbles=int(input("enter the symbles:"))
password=[]
for i in range(0,n_letters):
    char=random.choice(letters)
    password+=char
# print(password)
for i in range(0,n_numbers):
    char=random.choice(numbers)
    password+=char
# print(password)
for i in range(0,n_symbles):
    char=random.choice(symbles)
    password+=char
# print(password)
random.shuffle(password)
# print(password)
password_list=""
for char in password:
    password_list+=char
print(password_list)

