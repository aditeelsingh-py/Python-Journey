class Animal:
  def __init__(self):
    print("animal constructor")
  def move(self):
    print("animal moves")
class Dog(Animal):
  def __init__(self):
    super().__init__()
    print("dog constructor")
  def move(self):
    super().move()
    print("dog moves")
d=Dog()
d.move()

# Bank Balance
class Person:
  def __init__(self,name,age,phone_number):
    self.name=name
    self.age=age
    self.phone_number=number
    
