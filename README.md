# 4.12
python code 4.12
# Jake test 1
service_schedule = {"-": 0,"Oil change" : 35, "Tire rotation" : 19, "Car wash" : 7, "Car wax": 12}
first_service = ""
second_service = ""
print("Davy's auto shop services")
print("Oil change -- $35")
print("Tire rotation -- $19")
print("Car wash -- $7")
print("Car wax -- $12")
print("")

first_service = input("Select first service:\n")

second_service = input("Select second service:\n")
print()

print("Davy's auto shop invoice")
print()
if(first_service == "-"):
  print("Service 1: No service")
else:
  print("Service 1:", first_service, service_schedule[first_service])
  
if(second_service == "-"):
  print("Service 2: No service")
else:
  print("Service 2:", second_service, service_schedule[second_service])

invoice = service_schedule[second_service] + service_schedule[first_service]
print("Total:", invoice)


#james johnson
# Type your code here
service_schedule = {"-": 0,"Oil change" : 35, "Tire rotation" : 19, "Car wash" : 7, "Car wax": 12}
first_service = ""
secondservice = ""

print("Davy's auto shop services")
print("Oil change -- $35")
print("Tire rotation -- $19")
print("Car wash -- $7")
print("Car wax -- $12")
print("")

first_service = input("Select first service:\n")

secondservice = input("Select second service:\n")
print()

print("Davy's auto shop invoice")
print()
if(first_service == "-"):
  print("Service 1: No service")
else:
  print("Service 1:", first_service, service_schedule[first_service])
  
if(secondservice == "-"):
  print("Service 2: No service")
else:
  print("Service 2:", secondservice, service_schedule[secondservice])

invoice = service_schedule[secondservice] + service_schedule[first_service]
print("Total:", invoice)
#james zybooks code passed all

service_schedule = {"-": 0,"Oil change" : 35, "Tire rotation" : 19, "Car wash" : 7, "Car wax": 12}
first_service = ""
secondservice = ""
invoice_total = 0
print("Davy's auto shop services")
print("Oil change -- $35")
print("Tire rotation -- $19")
print("Car wash -- $7")
print("Car wax -- $12")
print("")

first_service = input("Select first service:\n")
secondservice = input("Select second service:\n")
print()

print("Davy's auto shop invoice")
print()
if(first_service == "-"):
  print("Service 1: No service")
else:
  print("Service 1: %s, $%d" %(first_service, service_schedule.get(first_service)))
  
if(secondservice == "-"):
  print("Service 2: No service")
else:
  print("Service 2: %s, $%d" %(secondservice, service_schedule.get(secondservice)))

invoice = service_schedule.get(first_service) + service_schedule.get(secondservice)
print()
print("Total: $%d" % (invoice))
# 5.13

import random
num_two = 0
num_three = 0
num_four = 0
num_five = 0
num_sixes = 0
num_sevens = 0
num_eight = 0
num_nine = 0
num_ten = 0
num_eleven = 0
num_twelve = 0
num_rolls = int(input('Enter number of rolls:\n'))

while num_rolls >= 1:
    for i in range(num_rolls):
        die1 = random.randint(1,6)
        die2 = random.randint(1,6)
        roll_total = die1 + die2

        #Count number of sixes and sevens
        if roll_total == 2:
            num_two = num_two + 1
        if roll_total == 3:
            num_three = num_three + 1
        if roll_total == 4:
            num_four = num_four + 1    
        if roll_total == 5:
            num_five = num_five + 1
        if roll_total == 6:
            num_sixes = num_sixes + 1
        if roll_total == 7:
            num_sevens = num_sevens + 1
        if roll_total == 8:
            num_eight = num_eight + 1
        if roll_total == 9:
            num_nine = num_nine + 1
        if roll_total == 10:
            num_ten = num_ten + 1
        if roll_total == 11:
            num_eleven = num_eleven + 1
        if roll_total == 12:
            num_twelve = num_twelve + 1
        print('Roll %d is %d (%d + %d)' % (i, roll_total, die1, die2))
        num_rolls = num_rolls - 1
    num_two = '*' * num_two
    num_three = '*' * num_three
    num_four = '*' * num_four
    num_five = '*' * num_five
    num_six = '*' * num_six
    num_seven = '*' * num_seven
    num_eight = '*' * num_eight
    num_nine = '*' * num_nine
    num_ten = '*' * num_ten
    num_eleven = '*' * num_eleven
    num_twelve = '*' * num_twelve
    print('\nDice roll statistics:')
    print('2s:', num_two)
    print('3s:', num_three)
    print('4s:', num_four)
    print('5s:', num_five)
    print('6s:', num_sixes)
    print('7s:', num_sevens)
    print('8s:', num_eight)
    print('9s:', num_nine)
    print('10s:', num_ten)
    print('11s:', num_eleven)
    print('12s:', num_twelve)
else:
    print('Invalid number of rolls. Try again.')
    
   

#5.14
triangle_char = input('Enter a character:\n')
triangle_height = int(input('Enter triangle height:\n'))
print('')
kv = 0

while kv < triangle_height:
    k = 0
    while k <= kv:
        print(triangle_char, end=' ')
        k += 1
    print('')
    kv += 1
#5.15
 arrow_base_height = int(input('Enter arrow base height:\n'))
arrow_base_width = int(input('Enter arrow base width:\n'))
arrow_head_width = int(input('Enter arrow head width:\n'))

while arrow_head_width <= arrow_base_width:
    print ('Enter arrow head width:')
    arrow_head_width = int(input())

print('')

for ib in range(arrow_base_height):
  for jg in range(arrow_base_width):
    print('*', end='')
  print('')

for ib in range(arrow_head_width):
  for jg in range(arrow_head_width - ib):
    print('*', end='')
  print('')

##
arrow_base_height = int(input('Enter arrow base height:\n'))
arrow_base_width = int(input('Enter arrow base width:\n'))
arrow_head_width = int(input('Enter arrow head width:\n'))

while arrow_head_width <= arrow_base_width:
    arrow_head_width = int(input('Enter arrow head width:\n'))
print('')

for i in range (arrow_base_height):
    i = ('*' * arrow_base_width)
    print(i)
for j in range(arrow_head_width):
    j = '*' * arrow_head_width
    print (j)
    arrow_head_width -= 1
# 6.18
def get_num_of_characters(inputStr):
    count = 0
    for i in range(len(inputStr)):
        count += 1
    return count

def output_without_whitespace(inputStr):
    inputStr = inputStr.replace(' ','')
    print('String with no whitespace: %s' %inputStr)

if __name__ == '__main__':
    inputStr = input('Enter a sentence or phrase:\n')
    
    print("You entered: ",inputStr)

    noOfChars=get_num_of_characters(inputStr);
    print("\nNumber of characters: ",noOfChars)

    stringWithoutSpace=output_without_whitespace(inputStr);
    print("String with no whitespace: ",stringWithoutSpace)
#ATTEMPTEMED NUMBER TWO
def get_num_of_characters(inputStr):
    count = 0
    for i in range(len(inputStr)):
        count += 1
    return count

def output_without_whitespace(inputStr):
    inputStr = inputStr.replace(' ','')
    print('String with no whitespace: %s' %inputStr)

if __name__ == '__main__':
    inputStr = input('Enter a sentence or phrase:\n')
    print()
    print("You entered: %s" %inputStr)
    print()
    print('Number of characters: %s' %(get_num_of_characters(inputStr)))
    output_without_whitespace(inputStr)

# 7.6


# Chapter 7 Additional Exercises
  # Print Names
#jake try1

def main():
    name = input("Enter in your First, Middle and last name:")    

split_name = name.split()

print(split_name)

main()

try2
string = input("Enter in your First, Middle and last name:")    

names = string.split()
for firstletter in names:
    print(firstletter[0] + ".")

  # Alphabetic Telephone #
phoneNum = input('Enter the number in the format of XXX-XXX-XXXX\n')

print(phoneNum)

newPhoneNumber = ''
for char in phoneNum:
    
    if char == 'A' or char == 'B' or char == 'C':
        
        char = '2'
    
    elif char == 'D' or char == 'E' or char == 'F':
        
        char = '3'
    
    elif char == 'G' or char == 'H' or char == 'I':
        
        char = '4'
    
    elif char == 'J' or char == 'K' or char == 'L':
        
        char = '5'
    
    elif char == 'M' or char == 'N' or char == 'O':
        
        char = '6'
    
    elif char == 'P' or char == 'Q' or char == 'R' or char == 'S':
        
        char = '7'
    
    elif char == 'T' or char == 'U' or char == 'V':
        
        char = '8'
    
    elif char == 'W' or char == 'X' or char == 'Y' or char == 'Z':
        
        char = '9'
    
    newPhoneNumber = newPhoneNumber + char
    
    #VOWELS
random_statement = input("Enter stament")



print(random_statement)

Number_of_vowels = 0
Number_of_Constants = 0
for char in random_statement:
    if char == 'a'or char == 'e' or char == 'i' or char == 'o' or char == 'u':
        Number_of_vowels += 1
    else:
        Number_of_Constants += 1

print(Number_of_vowels, Number_of_Constants)      

  # Pig Latin

def main():
    words = str(input("English Sentence: ")).split()
for word in words:
        print(word[1:] + word[0] + "ay", end = " ")
    print()

main()    



