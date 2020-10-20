Programming Assignment-4 Part-A (Inheritance and Polymorphism)
(Total Marks 70)
Q#1)
Create a class Vehicle with following attributes and functions

i.	Model
ii.	Year
iii.	Brand
iv.	Colour
v.	MilesperGallon 
vi.	Define constructor/constructors to populate data memebers
vii.	Setters and getters
viii.	fuelEconomy() //This function will return mainly MilesperGallon

Create 2 subclass of Vehicle i.e. HybridVehicle, EcoVehicle and override fuelEconomy() method as:
i.	For HybridVehicle add extra 50 miles to original MilesperGallon
ii.	For EcoVehicle add extra 10 miles to original MilesperGallon

Create Test class with main method and create objects of HybridVehicle and EcoVehicle each and store them in Array of Vehicle and iterate over it to display Model, MilesperGallon.

*You may have to use super() to call super class constructor and populate data members 


Q#2)

Create an Abstract class Book with following attributes and functions

i.	Title
ii.	NoofPages
iii.	Author
iv.	Publisher
v.	NoofCopies
vi.	Price
vii.	PriceperCopy() // this should be an Abstract method
viii.	Define setters and getters

Create two subclasses of Book as ScinetificTransaction and Academic, where 
i.	ScientificTransaction should have extra attributes ConferenecName, Loctaion,Date (Treat it as string value) and TotalExpense. Override abstract method PriceperCopy()  with following formula TotalExpense/NoofCopies for Price.
ii.	Academic should also Override abstract method that simply shows Price.

Create Test class with main method and create objects of ScinetificTransaction and Academic in it and display their data (You can use toString() which may need you to override in subclasses too).

Q#3 A)

Create class Account with following attributes and functions:
i)	AccountTitle
ii)	BranchName
iii)	AccountType
iv)	Amount
v)	Define constructor/constructors
vi)	Define getters and setters
vii)	CalculateProfit()// This will return original amount
Make sure this class cannot be inherited in future (Hint: Final class, Private constructor).


Q#3 B) Make Account class inheritable.
Create two subclasses of Account class with names SavingAccount and CurrentAccount.
i)	In SavingAccount override CalculateProfit that return 10% of Amount as profit
ii)	In CurrentAccount override CalculateProfit that return 15% of Amount as profit

Q#3 C)
Define Account class as Interface (Obviously there will be no Data members in it)
i)	Define public abstract method CalculateProfit() in it

Create a class AccountImpl that implements Account and do following:
i)	AccountTitle
ii)	BranchName
iii)	AccountType
iv)	Amount
v)	Define constructor/constructors
vi)	Define getters and setters
*Notice I did not ask you to implement CalculateProfit() in AccountImpl class, it should be defined as Abstract hence AccountImpl should be Abstract class

Create two subclasses of Account class with names SavingAccount and CurrentAccount.
i)	In SavingAccount override CalculateProfit that return 10% of Amount as profit
ii)	In CurrentAccount override CalculateProfit that return 15% of Amount as profit


Q#4)
Define an interface Person with following 
i)	Profession(String Title)

Define an interface Interests with following
i)	Sports(String SportName)

Define a class Affiliation with following:
i)	NameofInstitute
ii)	Address
iii)	Getters and Setters
iv)	Constructor
Create a class Student that extends Affiliation and implements Person, Interests. Do implement all Abstract methods

Create Test class with main method and define an object of Student and display its information (You can override toString() in student class).


Q#5) Create Interface Story with following
i)	Tell() 

Create sub interface ReadAble with following
ii)	Read()

Create class Student implement ReadAble and define abstract methods so that Tell() displays “Student tells a story” and Read() displays “Student reads a story”.

Create Test class and create object of Student and call Tell() and Read().

Q#6) Define an Interface CanFight with following
i)	Fight()

Define interface CanFly with following
i)	Fly()

Define interface CanSwim with following
i)	Swim()

Define a class ActionCharacter with following
i)	Fight() // This function displays message “Action Charcater can Fight”

Define class Hero that extends from ActionaCharcater and Implements CanFight, CanFly, CanSwim. Implement abstract method Fly() to display “Hero can fly” and Swim() to display “Hero can swim”.

*Did you observed one thing that class and interface have same method Fight() but you did not get any error to necessarily implement abstract method? In Java preference is always given to superclass over superinterface to avoid confusion.


Q#7) Create interface Calculator with following 
i)	Addition(int,int)
ii)	Multiplictaion(int,int)
iii)	Subtraction(int,int)
iv)	Division(int,int)

Create class OrdinaryCalculator implements Calculator with
i)	Implement all abstract methods in it
ii)	Define method Display()
// This displays “I am B&W Display”, make sure this method can not be overridden in subclasses. 
Hint: Static methods are class’s property other than these are Instance properties hence can be overridden

Create sub class of OrdinaryCaculator as AdvanceCalculator with
i)	Power(int,int) //You can use Math.pow() function to caculate power
ii)	Sqrt(int) //You can use Math.sqrt() function to caculate suqre root
iii)	Define method Display() // This displays “I am coloured Display”
//For above method write @Override before method signature, Error? Compiler is asking you to define an abstract method in super class. This shows that Static methods are never property of instance even super class OrdinarYCaculator has Display() but its statis.




