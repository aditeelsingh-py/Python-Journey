25-june-26. 10:23am THURSDAY


# Q2 A company wants to identify whether an employee is eligible for a bonus based on attendance percentage and performance rating. 
 

CODE:- 

class Employee:
  def __init__(self,name,attendance,rating):
    self.name=name
    self.attendance=attendance
    self.rating=rating
  def CheckBonus(self):
    if self.attendance>90 and self.rating>8:
      print(f"{self.name} is Eligible for bonus")
    else: 
      print("not eligible for bonus")

emp=Employee("Aditee" ,95 ,9)
emp.CheckBonus()

# Q3 Create a program to check whether a given username and password match predefined credentials. 


class User:
  def __init__(self,new_username, new_password):
    self.new_username=new_username
    self.new_password=new_password
  def CheckPassword(self):
    old_username=input("enetr username")
    old_password=input("enter password")
    if self.new_username == old_username and self.new_password == old_password:
      print("Credentials matched")
    else:
      print("Credentials not matched")
user=User("Aditee","diva")
user.CheckPassword()

