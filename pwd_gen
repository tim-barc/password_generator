import random
import string

lower = string.ascii_lowercase
upper = string.ascii_uppercase
num = string.digits
symbols = '@%+\\/\'!#$^?:,(){}[]-'

print(r"""
 _____                                    _    _____                           _             
|  __ \                                  | |  / ____|                         | |            
| |__) |_ _ ___ _____      _____  _ __ __| | | |  __  ___ _ __   ___ _ __ __ _| |_ ___  _ __ 
|  ___/ _` / __/ __\ \ /\ / / _ \| '__/ _` | | | |_ |/ _ \ '_ \ / _ \ '__/ _` | __/ _ \| '__|
| |  | (_| \__ \__ \\ V  V / (_) | | | (_| | | |__| |  __/ | | |  __/ | | (_| | || (_) | |   
|_|   \__,_|___/___/ \_/\_/ \___/|_|  \__,_|  \_____|\___|_| |_|\___|_|  \__,_|\__\___/|_|                                                                                                                                                                                       
""")
print("Made by Tim")
print("-----------------------------------------------------------------------------------------------------")
print("""It is extremely important to use secure passwords. Weak passwords (such as dictionary words, date 
of birth, etc) are extremely vulnerable to a plethora of attacks such as brute force attacks, dictio-
nary attacks and more. This generator was created to influence people into using secure passwords 
by generating a pseudorandom password that users can copy and paste into password reset forms and/or 
when creating accounts. According to NIST, password length is the most important aspect when creating
a password. the longer the password, the longer/more difficult it is to decrypt or brute force it. 
It is recommended to use passwords that are equal to or great than 8 (16 is preferable).""")
print("-----------------------------------------------------------------------------------------------------")

print("Type 'lower' for lowercase password or 'upper' for uppercase password and 'nosymb' for no symbols")
option = input('Option: ')
print("-----------------------------------------------------------------------------------------------------")

while True:
    try:
        pwd_length = int(input('Password length: '))
        if pwd_length < 8:
            length = input("\nAny password shorter then 8 is vulnerable to brute force attacks.\nif you wish to continue type yes(y), otherwise type no(n): ")
            print("")
            strip = length.lower()
            if strip == 'yes' or strip == 'y':
                chars = lower + upper + num + symbols
                gen = random.sample(chars, pwd_length)
                pwd = "".join(gen)
            elif strip == 'no' or strip == 'n':
                break
        lwrcase_strip = option.lower()
        if lwrcase_strip == "lower":
            chars = lower + num + symbols
            gen = random.sample(chars, pwd_length)
            pwd = "".join(gen)
            print("Find the generated lowercase password below ↓\n" + pwd)
            break
        elif lwrcase_strip == "upper":
            chars = upper + num + symbols
            gen = random.sample(chars, pwd_length)
            pwd = "".join(gen)
            print("Find the generated uppercase password below ↓\n" + pwd)
            break
        elif lwrcase_strip == "nosymb":
            chars = lower + upper + num
            gen = random.sample(chars, pwd_length)
            pwd = "".join(gen)
            print("Find the generated password below (no symbols) ↓\n" + pwd)
            break

        #combining the characters
        chars = lower + upper + num + symbols

        #generating random password
        gen = random.sample(chars, pwd_length)

        #creating the password
        pwd = "".join(gen)

        print("Find the generated password below ↓\n" + pwd)
        break
    except:
        print('Please enter a valid integer (example: 8)')

print("Press ENTER to exit")
