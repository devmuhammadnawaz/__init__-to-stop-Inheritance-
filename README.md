# __init__-to-stop-Inheritance-
class Person:
    def __init__(self, fname, lname):
        self.firstname = fname
        self.lastname = lname
    def printname(self):
        print(self.firstname, self.lastname)
class Student(Person):
    def __init__(self, fname, lname):
        Person.__init__(self, fname, lname)
x = Stdent("Muhammad", "Nawaz")
x.printname()
