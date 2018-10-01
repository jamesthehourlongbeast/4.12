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

if num_rolls >= 1:
    for i in range(num_rolls):
        die1 = random.randint(1,6)
        die2 = random.randint(1,6)
        roll_total = die1 + die2

        #Count number of sixes and sevens
        if roll_total == 6:
            num_sixes = num_sixes + 1
        if roll_total == 7:
            num_sevens = num_sevens + 1
        if roll_total == 8:
            num_eight == num_eight + 1
        if roll_total == 9:
            num_nine == num_nine + 1
        print('Roll %d is %d (%d + %d)' % (i, roll_total, die1, die2))

    print('\nDice roll statistics:')
    print('6s:', num_sixes)
    print('7s:', num_sevens)
else:
    print('Invalid number of rolls. Try again.')
