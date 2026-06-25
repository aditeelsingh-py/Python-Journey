25-june-26. 10:23am THURSDAY


# Q2 A company wants to identify whether an employee is eligible for a bonus based on attendance percentage and performance rating. 
 

CODE:- 
_employeeName=input("enter name")
_attendance=float(input("enter attendance percentage"))
_performanceRating=float(input("enter performance rating"))
if (( _attendance >75) and (_performanceRating>3.5)):
  print(_employeeName, "is eligible for bonus")
else:
  print(_employeeName,"is not eligible for bonus")

OUTPUT -1
enter nameromio
enter attendance percentage80
enter performance rating5
romio is eligible for bonus


# Q3 Create a program to check whether a given username and password match predefined credentials. 


Username = 'aditee'
Password = 2311
newUsername = input("enter username")
newPassword = input("enter password")
if (Username == newUsername) and ( Password == newPassword):
  print("access allowed")
else:
  print("access denied")


OUTPUT -1
enter usernameaditee
enter password23
access denied 
OUTPUT -2
enter usernameaditee
enter password23
access allowed

