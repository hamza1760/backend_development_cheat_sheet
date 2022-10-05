# backend_development_cheat_sheet

# Java 
**Q- what is jdk jre and jvm?**
- JDK(Java development Kit). It internally contains JRE and JVM. It is responsible for the development of java program.
- JRE(Java Runtime Environment). It internally contains JVM. It is resposible for the execution of java program.
- JVM)(Java virtual machine). It is the software in the form of interpreter through which we can execute our java program.

**Q- What is compiler?**
A- Compiler is responsible for converting the source code to machine language.

**Q- Why is java platform independent?**
A- Java compiler converts the java source code into bytcode rather than converting them for specific machine language. So if we want to run java application in any platform that platform must have installed the JVM which is responsible for converting the bytecode in to the respective machine language using JIT compiler. 

**Q- What is JIT compiler?**
A- JIT compiler stands for just in time compiler which convert the bytcode line by line into the machine language of a platform we want to run java application.

**Q- What are variables in Java?**

A- Variable is container to store value. that value can be changed accordingly.

**Rules for declaring a variable:**
 - they cannot be start with digit. 
 - they should not have spaces. 
 - they cannot be a keyword ie. void.

## Types of Variables:
- Local Variable
- Instance Variable
- Static Variable

	## Local Variable:
	- Variable that are declared inside the methods.
	- They can only be accessible within the method.
	- They are stored inside the stack area.
	- They does not have the default value , value should be provided to them while declaring them.
	- Access modifiers cannot be used with them.

	## Instance Variable:
	- Variable that are declared in the class.
	- They can be accessed anywhere within the class.
	-  They are stored inside heap area.
	- They have default values.
	- Access modifiers can be used with them.
	- They can be accessed from the other class by creating 
	the object of the class they are declared in.

	## Static Variable:
	- Variable that are declared in the class with static keyword.
	- They can be accessed anywhere within the class.
	- They are stored inside the memory area.
	- They have default values.
	- Access modifiers can be used with them.
	-  They can be accessed from the other class directly by using the class name.
	


**Q-  Data types in java?**
A- There are two types of data type in java
**primitive data type:**
These are data types which are defined by java. there object cannot be created
**non-primitive data type:**
These are data types which are defined by the programmer. there object can be created.

**Q-  keywords in java?**
A- words which are reserved by java.


# OOP
**Q- What is oop?**
A- OOp is a programming model based on the concept of objects. Everything we see in real life is an object and we can determine them programatically
by using oop programming model. The main advantages of oop is **code reusability and security**.

**Q-What are the four pillars of oop?**
A- The four pillars of oop are: Encapsulation,Inheritance,Polymorphism and Encapsulation.

**Q-What is encapsulation?**
A-Encapsulation in java is a mechanism of wrapping variable and methods together as a single unit. Encapsulation can aslo be referred to as data hiding because the variables of the class will be hidden from the other classes and they could only be accessible through the public methods of the current class.

**Q-What is abstraction?**
A- Abstraction is hiding implementations detail and showing only the main part to the user. In java we can acheive abstraction in two ways one is abstract class and another is interface. Through interface we can achieve 100 percent abstraction and through abstract classs we can achieve 0-100 percent abstraction. 

**Q- What is polymorphism?**
A- Ploymorphism means many forms for example water has many forms i.e solid , liquid . gas. We can achieve polymorphism in java through methods.
 - **Method overloading.**
 - **Method Overriding.**

**Q-What is inheritance?**
A- Inheriting the property of parent class into child class. The main **advantage** of inheritance is **code reusabilty**. We can also **achieve polymorphism** using inheritance. But the biggest **disadvantage** of inheritance is that the classes are **tightly coupled**.

**Types of Inheritance:**

 - Single Inheritance 
 - Multilevel Inheritance 
 - hierarchical inheritance
 - multiple inheritance( **not supported by java**)
 - hybrid inheritance( **not supported by java**)

**Q- Does all the property of parent class got inherited by the child class?**
A- no, constructor and private methods of variable cannot be inherited.

**Q- Super keyword in java?**
- Super keyword  refers to the immediate parent class instance variable.
- Super keyword can be used to call parent class method.
- Super keyword can be used to invoke parent class constructor.

**Q- This keyword in java?**
- This keyword refers to the current class instance variable.
- This keyword can be used to invoke current class method .
- this() can be used to invoke current class constructor.

**Q- Static keyword in java?**
- It cannot be used local variable.
- They are used for make memory usage efficient.

**Q- difference b/w Final , finally ,and finalize()?**

<img width="794" alt="Screenshot 2022-09-02 at 9 31 34 PM" src="https://user-images.githubusercontent.com/99591584/188198525-0c7d4bcd-e31b-451b-acfc-1d3ac9b54abf.png">

**Q- different between throw and throws?**
 - throw keyword is used to create an exception object manually.
 -  throws keyword is used to declare the exception. it indicates the caller method that given exception can occur so we have to handle it either using try-catch block or again declare it using throws keyword.

# Spring

**Q-What is Api?**
A- Api means application programming interface it allows two applications to talk to each other.

**Q-What is RestApi?**
A- Rest means Representational State Transfer. RestApi is a Api that follows some standards which are:

 -  A client-server architecture made up of clients, servers, and resources, with requests managed through HTTP.
 -   Stateless client-server communication, meaning no client information is stored between get requests and each request is separate and unconnected.
 - Cacheable data that streamlines client-server interactions.

**Q- What is spring?**
A- Spring is a dependency injection framework to make java application loosely coupled. Spring provide us Inversion of control and by using ioc we do dependency injection. it is developed by rod johnson is 2003.

**Q-What is Dependency Injection?**
A- It is a design pattern.
In software engineering, dependency injection is a technique whereby one object (or static method) supplies the dependencies of another object. 

**Q-What is inversion of control?**
A-   It means giving the control of creating the object of any class dependency to the Spring IOC container.

**Q-What is SpringBoot?**
A- It is the module of spring which help us to develop java application very fast. All the configuration that need to be done manually while using spring are done automatically using SpringBoot.

**What is JDBC?**
A- JDBC stands for Java Database Connectivity.It is an old way to save data in database and fetch data from database. Where we need to write SQL queries manually. ORM tools like hibernate and Spring data JPA solve this problem for us.

**Q- what is ORM?**
A- Object Relational Mapping. If we want to store data in database then orm takes the object from the program and store in the database.  And if we want to fetch the data from the database then orm takes the row from the table and convert it into object. if we don't use orm then we need to write SQL queries manually for storing and fetching data.

**Q-Spring Data JPA?**

 - JPA means Java Persistence API. JPA is an ORM tool(Object Relational Mapping). 
 
 - The implementation of JPA is done by hibernate. 
 
 - JPA provides us the interface EntityManagerFactory and EntityManagerFactory provide us EntityManager and EntityManager provide us the crud methods.

**Q- What is hibernate?**  

 - Hibernate is ORM tool. 
 
 - It is java framework that simplifies the
   development of java application to interact with the database. We no need to write SQL queries manually , Hibernate will automatically do this for us.
   
- Hibernate is non-invasive framework. means it won't force the programmers to extends/implements any class/interface.

**Q- How to use JPA and Hibernate in SpringBoot?**
A- Since every configuration is done automatically in springboot so we only need to add the dependency of spring-boot-starter-data-jpa.  Now lets suppose we have a entity class Named User we will make it the entity of the database by @entity and the we will make an interface named UserRepository and will we extend it with the interface which is provided to us by SpringBoot namely CrudRepository or its child JpaRepository. These both interfaces will provide us all the functions to work with database. but the major difference between them is CrudRepository provide us basic crud operations whereas JpaRepository provide us some extra operations.

## **example working:**

	**Hibernate working**:
	
	@Entity  
	public class Item {  
  
	@Id  
	private int itemId;  
    private int quantity;  
    private long upc;  
    private String color;  
    private double price;  
    private double discount;

	 **JPA working:**
	public interface ItemRepository extends JpaRepository<Item, Integer> {  
	}

  
## Memory Storage in Java:
<img width="1145" alt="memory storage" src="https://user-images.githubusercontent.com/99591584/187669783-6bb66094-8d0f-42d4-8055-4c6681a789cb.png">

# Strings In Java

**Q- what is string constant pool?** 
- It is also known as string literal pool. It is an area in heap memory where java stores String literal values.
-  Till java 1.6 SCP is present inside method area but after java 1.7 it is shifted in heap area.
- String s1 = "hamza" // it will create object inside SCP.
- String s1 = new String("hamza")// it will create object inside Heap Area as well as SCP means two object will be created.
- The object present inside SCP are not applicable for garbage collector because a reference variable is internally maintained by JVM. 

## working:
<img width="758" alt="Screenshot 2022-08-31 at 4 51 27 PM" src="https://user-images.githubusercontent.com/99591584/187672774-97a5cf6d-e0bb-41d2-95a5-9c28575e0622.png">

**Q-What is string immutablity?**
- immutable means unchangeable.

## **working:**
<img width="876" alt="Screenshot 2022-08-31 at 5 24 42 PM" src="https://user-images.githubusercontent.com/99591584/187677812-91f7449d-4093-458a-a802-101c51a275d6.png">

**Q- what is difference between == and .equals ?**
- == operator is used to compare address or refereence.
- .equals method of String class is used compare content. where as .equals method of Object class is used to compare address or reference.

**Q-  why character array are better choice for storing password rather than string?**

- Since string are immutable and they not applicable for garbage collector so if we store our password it will remain in the SCP forever and can be hacked easily.
- If we store something in character array and print it to console or anywhere else it will print the object of that char array while string will print the real value. so character array seems more secure.

**Q-  String , String Builder and String Buffer?** 

<img width="1161" alt="Screenshot 2022-08-31 at 8 23 07 PM" src="https://user-images.githubusercontent.com/99591584/187716725-be26e483-ca0e-4960-85a5-50da68aa711d.png">

# Arrays In Java

- Arrays are used to store the value that are of same data type.
- Each value in array is accessed by its index position.
- Index value of every array starts with zero and ends to its length-1.
- Super class of an array is Object class.
- Array occupies memory in heap area.

	##
		int[] array = new int[100];

	## Advantages
	- It can store multiple values at once.
	-  Arrays are faster than primitive data types.
	- We can store objects inside array.

	## Disadvantages
	- The size of the array is fixed we cannot increase or decrease its size in the runtime.
	- High chances of wastage of memory.
	- We can only store similar data type in array.
	- If we remove or insert an element in the middle of an array than we need traverse the whole array and shift values.

## Types Of Arrays:
 - Single Dimensional Array
 - Multi Dimensional Array
 
<img width="1342" alt="Screenshot 2022-09-08 at 8 24 30 PM" src="https://user-images.githubusercontent.com/99591584/189162181-ccf11c20-992f-4da8-a336-5222c0e78162.png">


## Single Dimensional Array

## One Dimensional Array:
- Declaration
<img width="1615" alt="Screenshot 2022-09-08 at 8 14 48 PM" src="https://user-images.githubusercontent.com/99591584/189160049-223fd0be-6b9f-4d54-acde-fd5e5e06cb9b.png">

- Creation
<img width="1615" alt="Screenshot 2022-09-08 at 8 16 06 PM" src="https://user-images.githubusercontent.com/99591584/189160203-0088a140-deff-4613-8b02-b584bbba676a.png">

- Initialization
![Screenshot 2022-09-08 at 8 16 44 PM](https://user-images.githubusercontent.com/99591584/189160365-066c62af-35ca-43e3-8a60-033594cbdf93.png)

- Retrieve
<img width="1615" alt="Screenshot 2022-09-08 at 8 17 19 PM" src="https://user-images.githubusercontent.com/99591584/189160458-8607c832-8cb7-435a-b5fd-1cd3f0614dc4.png">


## Multi Dimensional Array
## Two Dimensional Array:
## Three Dimensional Array:


	
	

# Multi Threading

**Q- Multitasking , Multi processing , Multi threading?**

**Multi Tasking:** 
- performing multiple task at single time.
-  increase the perfomance of the cpu.
- achieved by Multi Processing and Multi Tasking.

**Multi Processing:**
- Process based multi tasking.
- Multi software or multiple cpu.
- It is best suitable at os level.

**Multi Threading:**
- Thread based multi tasking.
- Tasks within the software are called thread.
- It is best suitable at programming level.

**Q- Different between process and thread?**

<img width="1063" alt="Screenshot 2022-08-31 at 9 10 24 PM" src="https://user-images.githubusercontent.com/99591584/187726893-6110a9f1-947f-4e29-9660-b84d2feb2d77.png">

# ** Multi Threading in java?**

We can create thread in java by two methods.
- Thread Class
- Runnable Interface 
- Runnable interfaces is implemented by thread class.

## Creating thread with Thread Class:
- Extending the Thread class in our class.
- Overriding run method which is overriden in  Thread class from the Runnable interface.
- Create the object of our class.
- Call the start() method which is available in Thread class.

## Creating thread with Runnable Interface:
- Implementing the Runnable interface in our class.
- Overriding the run method which is abstract in Runnable interface.
- Creating the object of our class.
- Creating the object of Thread class and passing our class object reference in the constructor of Thread class.

## Which way of creating thread is more efficient?
Creating thread with the runnable interface is more efficient because if our class is extending any other class and we still want to make it a thread so we could extend it with the thread class because multiple inheritance in not supported in java but we could implement the Runnable interface in our class.
**i.e:**
	Class A extends B implements Runnable

## Code for Performing single task from single thread:

<img width="364" alt="Screenshot 2022-08-31 at 10 36 51 PM" src="https://user-images.githubusercontent.com/99591584/187743362-b8a5c429-b73f-4eeb-a204-765d1ca85aed.png">


## Code for Performing single task from multiple thread:

<img width="434" alt="Screenshot 2022-08-31 at 10 38 36 PM" src="https://user-images.githubusercontent.com/99591584/187743702-9aa31d1f-fe32-4cac-a42c-15a42b3e1637.png">

## Code for Performing multiple task from multiple thread(MultiThreading Code):

<img width="503" alt="Screenshot 2022-08-31 at 10 44 30 PM" src="https://user-images.githubusercontent.com/99591584/187744929-01b72ec0-0ecf-4c56-92bc-2e7844debc31.png">

## Life cycle of thread( 5 stages)
<img width="452" alt="Screenshot 2022-08-31 at 9 27 31 PM" src="https://user-images.githubusercontent.com/99591584/187730423-65903548-400f-4ec2-97e5-4010452a368c.png">

# Syncronization

<img width="1544" alt="Screenshot 2022-09-07 at 5 28 58 PM" src="https://user-images.githubusercontent.com/99591584/188878810-3a1d0115-46a5-45b7-86a1-68d12fae2925.png">

## How To Achieve Synchronization:

<img width="1605" alt="Screenshot 2022-09-07 at 5 37 14 PM" src="https://user-images.githubusercontent.com/99591584/188880143-cd737d5b-76e3-4ea7-bf31-3dc5a1249605.png">

## Mutual Exclusive
- Synchronized Method:
	- It can be achieved by using the synchronized keyword with the method.
	- Its scope started from the start of method and ended to the end of 		 method.
	## working:
		synchronized void bookTicket(int seat)
		{
		//body
		}
- Synchronized Block:
	- It can be achieved by using the synchronized keyword with the logic part.
	- Its scope started from the start of logic part and ended to the end of logic.
	## working:
		void bookTicket(int seat)
		{
		synchronized(this) (
		if(logic)
		{
		//body
		}
		else
		{
		//body
		}
		)
		}

- Static Synchronization :
	- It is used for class level synchronization.
	- It can be acheived by using static synchronized keyword with the method.
	## working:
		static synchronized void bookTicket(int seat)
		{
		//body
		}

## Cooperation(Inter-thread communication in java)

<img width="1615" alt="Screenshot 2022-09-07 at 6 41 05 PM" src="https://user-images.githubusercontent.com/99591584/188897283-431e0081-fed0-4fd7-9972-384b576e597f.png">

## DeadLock
- Deadlock happens when one thread needs to acquire the lock on class or object but that class or object is acquire by another thread.
- Deadlock can be handled by releasing the lock at the particular time or by same ordering the acquiring of lock in both thread.

## LiveLock
- Livelock is also a deadlock but each thread is trying resolve the lock the lock for each other so the solution never comes up.

# Collection In Java 
## Collection hierarchy:

<img width="1033" alt="Screenshot 2022-08-31 at 11 10 08 PM" src="https://user-images.githubusercontent.com/99591584/187749439-560531a5-27e5-40c2-9c60-56a858816da4.png">

## **Q- Different between ArrayList and LinkedList?**

<img width="715" alt="Screenshot 2022-09-02 at 9 22 30 PM" src="https://user-images.githubusercontent.com/99591584/188197177-db478e5e-c026-4cfa-8c2a-074cc35c3947.png">



# Dbms

## Concept of All Normal Forms(Normalization):

<img width="1158" alt="Screenshot 2022-08-31 at 10 49 30 PM" src="https://user-images.githubusercontent.com/99591584/187745877-fb4ef4c5-1142-49a3-bce6-20425176a82f.png">


## keys in dbms:
- column which contain unique value can become key.
- keys in database are used to uniquely identify any record in a table.
- The are used to maintain integrity between tables.
- They are used to make relation between tables.

## Types of keys:
- SuperKey: combination of all keys.
- Candidate key: keys which form together to make superkey
- primary key: We can make any candidate key as our primary key according to our needs.
- Alternate key: Primary key is one all other key which not become primary key are called alternate key.
- Foreign key: The are used to make relation between table and to maintain refrential intigirity between tables.

## Joins
- Join is a cross product with some condition.
- Joins are used to bring multiple tables together.
- 
  
