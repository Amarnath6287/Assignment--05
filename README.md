# Base class
class Grandparent:
    def __init__(self):
        print("Grandparent constructor called")
    
    def grandparent_method(self):
        print("This is the grandparent's method")

# Derived from Grandparent
class Parent(Grandparent):
    def __init__(self):
        super().__init__()
        print("Parent constructor called")
    
    def parent_method(self):
        print("This is the parent's method")

# Derived from Parent
class Child(Parent):
    def __init__(self):
        super().__init__()
        print("Child constructor called")
    
    def child_method(self):
        print("This is the child's method")

# Create an instance of Child
c = Child()

# Call methods from all levels of inheritance
c.grandparent_method()
c.parent_method()
c.child_method()
