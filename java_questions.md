# General
What are the packages that you used in java?  
Is java pass by value or pass by reference?  
Can I instantiate Abstract class?  
Difference between Interface and Abstract class, and when should I use what?  
Can Interface extend another Interface?    
Can abstract Class extend Interface?  
What is difference in abstract Class extending Interface and normal Class extending Interface?  
Difference between Comparable and Comparator
  
# Generics

# Design Related/ Design Patterns
How many design patterns GOF(Gang of Four) have defined?  
What is immutable?
Why do we want an immutable class?  
How to make class Immutable?  
How to make class Singleton with clone scenario?
Factory Design pattern

# Java 8

# Multi-Threading
Why object class has wait(), notify(), notiftAll() methods in Java?  
Difference between yield(), sleep() and wait()?  
Multi-Threading in Colections?  
What do you mean by synchronized?
What is this in synchronized block(this)
Class level and Object level synchronization  
BlockingQue?
What is concurrent counterpart for LinkedBlockingQueue?

What is Executor framework?  
Executor Service?  
Advantages of Executor framework over normal Threading?  
Difference between execute() and submit() method?  
Difference between shutDown() and shutDownNow() in Executor?

# Exception Handling 
Exception Hierarchy?  
What is Exception Handling and why do we us it?  
Use of finally Block?  
What needs to be done to create my userdefined exception class?  
Extends Throwable is better or Extends Exception?  

# Collections
Difference between array and arrayList?  
Different implementations of List, Set and Map?  
When should you use ArrayList and when should you use LinkedList?  
Write your implementation of LinkedList?  
Write a List having features(Advantages) of both LinkedList and ArrayList?  

Difference between HashSet and TreeSet?  
How Treeset Works?  

Which datastructure HashMap internally uses to store data?  
Difference between HashMap and HashTable?  
Can we have null key in HashMap/TreeMap/HashTable
Why hash-code is required? why overriding equals is not Sufficient?
How HashMap works in Java?  
How ConcurrentHashMap works in Java?  
How SynchronizedHashMap works in Java?  
Multimap(Not from Guava, write your implementation)
How to sort values in HashMap?

# String
How many objects will be created for : String s = new String ("ABC"); 


# Scenario based:
Can we override static method? If no whether it will be runtime error or compile time?  
Ans: this instance method cannot override the static method from parent  

If I have a student class with int id and String name and I put this in hashMap/TreeMap what will happen?  

Apply encapsulation in your Employee class?    

Overriding: A a = new B(); a.i; a.j; // i is in A j is in B  

Can two Threads access two methods of same class simultaneously?  
  ```
    class Employee{
      void methodA(){

      }
      void methodB(){

      }
    }
  ```
a: Now I have two threads ThreadA and ThreadB, ThreadA wants to access methodA and ThreadB wants to access methodB, is it possible at the same time?  
  Ans: It is possible only if one is static so that it will acquire class level lock and other is non static and hence it will acquire instance level   lock
b: if I make both methods static but not synchronized, Then can they access it simultaneously? Yes  
c: if 1 method is static and another is non static?  

What will happen in below case?
```
<bean id = "123" class = "Employee">
<bean id = "456" class = "Employee">
```
Ans: it will work fine as a new instance with 456 is created for Employee class.


# Additional Info:
use of '_' as an identifier might not be supported in releases after Java SE 8

# Rest
Which Framework you have used and why?  
How did you configure the said framework?  
How did you handle CORS?  

# Hibernate
How ORM Works?  
Object life-cycle?    
LazyInitializationException?
What is LazyLoading in Hibernate?  
What are the types of cache?  
Why do we need Secondary cache(Advantages)?  


# Spring
Spring bean life cycle?    
When are the beans initialized in Spring?  
A: All singleton beans are initialized as context initialization while using applicationContext and at getBean when BeanFactory is used.  
What is Dependency Injection and it types?  
What is BeanFactory?   
Does BeanFactory support Annotations?  
Difference between BeanFactory and ApplicationContext?  
What is Autowiring?  
Types of Autowiring?  
Difference between @Service and @Component and @Resource?  
@Component, @Resource, @Service?  
How to get property file in Spring?  
Explain Spring MVC and filters in it?    
How Aspects work?   
What is connection pool and why do we use it?  
How to configure spring boot?  
How WSDL are generated in SOAP for Spring Boot app?  
How to configure transaction via Spring?  
What is Proxy and why?  

@Component, @Resource, @Service?  
Ans: In Spring 2.0 and later, the @Repository annotation is a marker for any class that fulfills the role or stereotype (also known as Data Access Object or DAO) of a repository. Among the uses of this marker is the automatic translation of exceptions.

Spring 2.5 introduces further stereotype annotations: @Component, @Service, and @Controller. @Component is a generic stereotype for any Spring-managed component. @Repository, @Service, and @Controller are specializations of @Component for more specific use cases, for example, in the persistence, service, and presentation layers, respectively.

Therefore, you can annotate your component classes with @Component, but by annotating them with @Repository, @Service, or @Controller instead, your classes are more properly suited for processing by tools or associating with aspects. For example, these stereotype annotations make ideal targets for pointcuts.

Thus, if you are choosing between using @Component or @Service for your service layer, @Service is clearly the better choice. Similarly, as stated above, @Repository is already supported as a marker for automatic exception translation in your persistence layer.
| Annotation | Meaning                                             |
+------------+-----------------------------------------------------+
| @Component | generic stereotype for any Spring-managed component |
| @Repository| stereotype for persistence layer                    |
| @Service   | stereotype for service layer                        |
| @Controller| stereotype for presentation layer (spring-mvc)      |

How to get property file in Spring?  
A: PropertyPlaceHolderConfigurer.  

# Others
JMS? and why do we use it?  
Unit test framework?

# JDBC
Difference between statement and preparedStatement?  


