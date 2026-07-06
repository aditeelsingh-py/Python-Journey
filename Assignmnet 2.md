# Q1
import csv
from abc import ABC, abstractmethod
class ReportFile(ABC):
    @abstractmethod
    def save(self,student_name,marks):
        pass
    @abstractmethod 
    def read(self):
        pass

class TextReport(ReportFile):
    def save(self,student_name,marks):
        with open("student.txt","a") as f:
            f.write(f"{student_name},{marks}\n")
    def read(self):
        with open("student.txt","r") as f:
            print("Text Report")
            print(f.read())
class CSVReport(ReportFile):
    def save(self,student_name,marks):
        with open("student.csv","a",newline="") as f:
            writer=csv.writer(f)
            writer.writerow([student_name,marks])
    def read(self):
        with open("student.csv","r") as f:
            reader=csv.reader(f)
            print("CSV Report")
            for row in reader:
                print(row[0], row[1])
students = [("Aditee",95), ("John", 88),("Emma",91),("Rahul",85),("Priya",99)]
reports=[TextReport(), CSVReport()]
for report in reports:
    for name, marks in students:
        report.save(name, marks)
    report.read()
    print("-"*30)
