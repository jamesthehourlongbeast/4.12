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


#james
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
