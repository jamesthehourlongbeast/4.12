# 4.12
python code 4.12
# Jake test 1
# Menu of Automotive Services
print('Davy's auto shop services')
print('Oil change -- $35')
print('Tire rotation -- $19')
print('Car wash -- $7')
print('Car wax -- $12')


#james
# Type your code here
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
print(first_service)
secondservice = input("Select second service:\n")
print(secondservice)

print("Davy's auto shop invoice")
print()
if(first_service == "-"):
  print("Service 1: No service")
else:
  print("Service 1:", first_service, service_schedule[first_service])
