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
# #Jake Try 1
while True:
        str = input('Enter input string: ')
        print("\n".rstrip("\n"))
        if(str!='q'):          
            str=str.replace(' ', '')
            if ',' in str:
                
                str=str.split(',')
            
                print ('First word: ' + str[0])
                print ('Second word: ' + str[1])
                print("\n".rstrip("\n"))
            else:
                print('Error: No comma in string.\n')
        else:
          break
#

  input_string = input('Enter input string with commas: ')
  if ',' in input_string:
    continue
  else:
    print('Error No commas')
    break
 


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
# CHAPTER 8 8.16
# 8.16 Ch 8 Warm up: People's weights (Lists) (Python 3)
entered_weights = []

i = 0

while i < 4:

    weight = float(input('Enter weight %i:\n' % (i+1)))

    entered_weights.append(weight)

    i += 1

print('Weights:', entered_weights)

print('\nAverage weight: %.2f' % (sum(entered_weights)/len(entered_weights)))

print('Max weight: %.2f' % (max(entered_weights)))



list_index_for_weights = int(input('\nEnter a list index (1 - 4):\n'))

print('Weight in pounds: %.2f' % (entered_weights[list_index_for_weights - 1]))

print('Weight in kilograms: %.2f' % (entered_weights[list_index_for_weights - 1] / 2.2))



print('\nSorted list:', sorted(entered_weights))

# Chapter 8 additional exercises 
# rainfall

mntName=["Jan","Feb","Mar","Apr","May","Jun","July","Aug","Sep","Oct","Nov","Dec"]

totRain=[0]*12

sum=0

for i in range(12):

    totRain[i]=int(input("Enter Total Rain in "+mntName[i]+": "))

sum+=totRain[i]

print("""\n\nTotal Rainfall: """+str(sum)+"""\nAverage Monthly Rainfall: """+str(sum/12)+"""

\nLowest Rainfall: """+str(min(totRain))+""" In month of """+str(mntName[totRain.index(min(totRain))])+"""

\nHighest Rainfall: """+str(max(totRain))+""" In month of """+str(mntName[totRain.index(max(totRain))]))



# number 3 encrypting and decoding

codes ={'A':'!','B':'@','C':'#','D':'$','E':'%','F':'^','G':'&','H':'*','I':'(',
                      'J':')','K':'-','L':'_','M':'+','N':'=','O':'`','P':'~','Q':'{','R':'[',
                      'S':'}','T':']','U':':','V':';','W':'"','X':'<','Y':'>','Z':'0','a':'1',
                      'b':'2','c':'3','d':'4','e':'5','f':'6','g':'7','h':'8','i':'9','j':'a',
                      'k':'b','l':'c','m':'d','n':'e','o':'f','p':'g','q':'h','r':'i','s':'j',
                      't':'k','u':'l','v':'m','w':'n','x':'o','y':'p','z':'q'}

for encrypted_codes in codes.values():
    print(encrypted_codes)


# Created List

top_films1 = ['Bohemian Rhapsody', 'The Nutcracker and the Four Realms',
             'Nobody''s Fool', 'A Star is Born', 'Halloween']
topfilms2 = ['Venom', 'Smallfoot', 'Goosebumps 2', 'Hunter Killer' , 'The Hate You Give']
print(top_films1)
print()
print(topfilms2)
top_ten_films = top_films1 + topfilms2
print()
print('Top ten films:', top_ten_films)
top_ten_films.sort()
print()
print('Sorted top ten films:', top_ten_films)
print()
print('Top five movies:', top_ten_films[0:5])
print()
print('Number one film:', top_ten_films[0])

# Dictionary

top_films1 = {'Bohemian Rhapsody': 1, 'The Nutcracker and the Four Realms': 2,
             'Nobody''s Fool': 3, 'A Star is Born': 4, 'Halloween': 5, 'Venom': 6
              , 'Smallfoot': 7, 'Goosebumps 2': 8, 'Hunter Killer': 9}
print(top_films1)
top_films1['The Hate You Give'] = 10
top_films1['Red'] = 11
print()
print(top_films1)
print()
del top_films1['Red']
print(top_films1)
print()
movie = input('Enter a movie to see if its in the top ten')
if 'movie' in top_films1:
    print(top_films1[Red2])
else:
    print('Not in the top ten movies')

# Chapter 9 
  #JAKE
class ItemToPurchase:

    def __init__(self):

        self.item_name = "none";
        self.item_price = 0;
        self.item_quantity = 0;
  
def print_item_cost(self):

    print(" " + self.item_name + " " + str(self.item_quantity) + " @ $" + str(self.item_price) + " = $" + str( self.item_price * self.item_quantity ));
  

def main():

  
    print("\n Item 1 \n");

i1 = ItemToPurchase();
  

i1.item_name = input(' Enter the item name: ');
i1.item_price = int(input('\n Enter the item price: '));
i1.item_quantity = int(input('\n Enter the item quantity: '));
  
print("\n\n\n Item 2 \n");
  

i2 = ItemToPurchase();
  

i2.item_name = input(' Enter the item name: ');
i2.item_price = int(input('\n Enter the item price: '));
i2.item_quantity = int(input('\n Enter the item quantity: '));
  
print("\n\n\n TOTAL COST \n\n");
  

i1.print_item_cost();
i2.print_item_cost();
  
  
total = (i1.item_price * i1.item_quantity) + (i2.item_price * i2.item_quantity);
  
  
print("\n\n Total: $" + str(total));
  

main()

    
   #JAMES
def main():
    print('Item 1')
    name_of_item_1 = input('Enter the item name:\n')
    price_of_item_1 = int(input('Enter the item price:\n'))
    quantity_of_item_1 = int(input('Enter the item quantity:\n\n'))   
    
#James
def __init__(self):

        self.item_name = "none";
        self.item_price = 0;
        self.item_quantity = 0;
  
def print_item_cost(self):
    self.print_cost = (self.item_quantity * self.item_price)

    print(" " + self.item_name + " " + str(self.item_quantity) + " @ $" + str(self.item_price) + " = $" + str( self.item_price * self.item_quantity ));
  

def main():

  
    print("\n Item 1 \n");


  

item1_name = input(' Enter the item name: ');
item1_price = int(input('\n Enter the item price: '));
item1_quantity = int(input('\n Enter the item quantity: '));
  
print("\n\n\n Item 2 \n");
  


  

item2_name = input(' Enter the item name: ');
item2_price = int(input('\n Enter the item price: '));
item2_quantity = int(input('\n Enter the item quantity: '));
  
print("\n\n\n TOTAL COST \n\n");
  

Item1.print_item1_cost();
Item2.print_item2_cost();
  
  
total = (i1.item_price * i1.item_quantity) + (i2.item_price * i2.item_quantity);
  
  
print("\n\n Total: $" + str(total));

# Ch. 9 Additional
#Cellphone

class CellPhone:
    def __init__(self, man, model, price):
        self.manufact = man
        self.model = model
        self.retail_price = price

    def set_manufact(self, man):
        self.manufact = man

    def set_model(self, model):
        self.model = model

    def set_retail_price(self, price):
        self.retail_price = price

    def get_manufact(self):
        return self.manufact

    def get_model(self):
        return self.model

    def get_retail_price(self):
        return self.retail_price

man = input('Enter the manufacturer: ')
model = input('Enter the model number: ')
price = float(input('Enter the retail price: '))
phone = CellPhone(man, model, price)
print('Here is the data that you have entered')
print('Manufacturer: ' + phone.get_manufact())
print('Model Number: ' + phone.get_model())
print('Retail Price: $' + '%.2f' % phone.get_retail_price())

#Name Selects
class Person:

    def init(self, name, ID, Department):
        self.Personname = name
        self.PersonID = ID
        self.PersonDepartment = Department 
    def str(self):
        return self.Personname+ " " + self.PersonDepartment+ ", " + str(self.PersonID)

class Employee(Person):

    def init(self, name, ID, Department, Title):
        super().init(name, ID, Department)

        self.StaffTitle = Title
    def str(self):
        return super().str() + ", " +  self.StaffTitle

x = Employee("Susan Meyers", 47899, "Accounting", "Vice president")
y = Employee("Marke Jones", 39119, "IT", "programming")
z = Employee("Joy Rogers", 81774, "Manufacturing", "Engineering")

print(x)
print(y)
print(z)
