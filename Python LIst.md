import ctypes
class MeraList:
    def __init__(self):
      self.size=1
      self.n=0
      self.A = self.MakeArray(self.size)
# Create Array
    def MakeArray(self, capacity):
     return(capacity*ctypes.py_object)()
# Print
    def __str__(self):
      result=' '
      for i in range(self.n):
        result += str(self.A[i]) + ','
      return '[' + result[ : -1] + ']'
# Append
    def append(self,item):
      if (self.n==self.size):
        self.resizeArray(self.size*2)

      self.A[self.n] = item
      self.n +=1
# Resize Array
    def resizeArray(self, newCapacity):
     B= self.MakeArray(newCapacity)
     self.size=newCapacity
     for i in range(self.n):
       B[i] = self.A[i]
     self.A = B

# POP
    def pop(self):
      if(self.n==0):
        return "Empty"
      self.n = self.n-1
      return (self.A[self.n-1])
      

# insert 
    def insert(self,index,item):
      if self.n==self.size:
          self.resizeArray(self.size*2)

      for i in range(self.n,index,-1):
        self.A[i] = self.A[i-1]
      self.A[index]=item
      self.n +=1

# clear
    def clear(self):
      self.n=0
      self.size=1

# find
    def find(self,item):
      for i in range(self.n):
        if self.A[i]==item:
         return i
      return -1

# length
    def length(self):
       return self.n
