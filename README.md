# inheritance 
               
               Inheritance in Python


Inheritance is one such concept in object oriented programming. Inheritance is
the capability of one class to derive or inherit the properties form another class.

Adventure of Inheritance:
Code reusability: We do not have to write the same code again and again,
We can just inherit the properties we need in a child class
It represents a real world relationship between parent class and child class.
It is transitive in nature. If a child inherits properties from a parent class,
then all other sub- classes of the child will also inherit the properties of the
parent class.

Example of inheritance:
01:
class student():
  def prin(self):  
    print(&quot;**Daffodil International University**\n &quot;)
class blood_Test(student):
  def __init__ (self,name,id,blood):
     self.name=name
     self.id=id
     self.blood=blood
  def blood_group(self):
     print(&quot;ID: &quot;f&#39;{self.id}&#39;,&quot;\nName: &quot;f&#39;{self.name}&#39;,
&quot;\nBlood Group: &quot;f&#39;{self.blood}&#39;)

obj=blood_Test(&quot;Tajul &quot;,&quot;191-15-2645&quot;,&quot;A+&quot;)

obj.prin()
obj.blood_group()     

02:
class Calculation1:  
    def Summation(self,a,b):  
        return a+b;  
class Calculation2:  
    def Multiplication(self,a,b):  
        return a*b;  
class Derived(Calculation1,Calculation2):  
    def Divide(self,a,b):  
        return a/b;  
d = Derived()  
print(d.Summation(10,20))  
print(d.Multiplication(10,20))  
print(d.Divide(10,20))

