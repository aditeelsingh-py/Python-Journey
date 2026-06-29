# Q4 A traffic monitoring system needs to determine whether a vehicle exceeded the speed limit.


speed_limit = int(input("enter speed limit"))
speed_vehicle = int(input("enter vehicles speed"))
if(speed_vehicle>speed_limit):
  print("limit exceeded")
else:
  print("no challan")

OUTPUT -1
enter speed limit23
enter vehicles speed80
limit exceeded
OUTPUT -2
[2]
6s
speed_limit = int(input("enter speed limit"))
speed_vehicle = int(input("enter vehicles speed"))
if(speed_vehicle>speed_limit):
  print("limit exceeded")
else:
  print("no challan")
enter speed limit40
enter vehicles speed30
no challan

# Q5 A bank wants to calculate simple interest for customers based on principal, rate, and time entered by the user.

principal = float(input("enter principal amount"))
rate = float(input("enter rate"))
time = float(input("enter time"))
simple_interest = (principal*rate*time)/100
print("the simple interest is", int(simple_interest))

OUTPUT -1
enter principal amount66
enter rate66
enter time4
the simple interest is 174

OUTPUT -2
enter principal amount4
enter rate5
enter time66
the simple interest is 13.2


# Q6 A movie theatre wants to assign ticket pricing based on age categories such as child, adult, and senior citizen.

age = int(input("enter age"))
if (age>=60):
  print("Senior Citizen Cost = 150")
elif (age>=30):
  print("Adult = 250")
else:
  print("Child = 200")

OUTPUT -1
enter age4
Child = 200
OUTPUT -2
enter age80
Senior Citizen Cost = 150

# Q7 Write a Python program to find the largest among three entered sales figures.

sale_figure1=float(input("enter sale figure1"))
sale_figure2=float(input("enter sale figure2"))
sale_figure3=float(input("enter sale figure3"))
print("the maximum sale figure is",max(sale_figure1,sale_figure2,sale_figure3))

OUTPUT -1
enter sale figure14000
enter sale figure249
enter sale figure3765
the maximum sale figure is 4000.0
OUTPUT -2
enter sale figure145
enter sale figure267
enter sale figure398
the maximum sale figure is 98.0

# Q8 A school wants to calculate grades for students based on marks obtained in five subjects.
english = float(input("enter english marks outoff 100"))
maths = float(input("enter maths marks outoff 100"))
science = float(input("enter science marks outoff 100"))
social_studies = float(input("enter social studies marks outoff 100"))
hindi = float(input("enter hindi marks outoff 100"))
percentage=(english+maths+science+social_studies+hindi)/5
if(percentage>=90):
  print("Grade A")
elif(percentage>=80):
  print("Grade B")
elif(percentage>=70):
  print("Grade C")
elif(percentage>=60):
  print("Grade D")

  OUTPUT -1
enter english marks outoff 10056
enter maths marks outoff 10078
enter science marks outoff 1006
enter social studies marks outoff 10088
enter hindi marks outoff 10077
Grade D

  OUTPUT -2

  








