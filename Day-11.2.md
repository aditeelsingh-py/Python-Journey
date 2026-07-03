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
