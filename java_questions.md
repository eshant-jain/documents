# General
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

# Java 8

# Multi-Threading
Why object class has wait(), notify(), notiftAll() methods in Java?  
Difference between yield(), sleep() and wait()?  
Multi-Threading in Colections?  
What do you mean by synchronized?
What is this in synchronized block(this)
Class level and Object level synchronization  
BlockingQue?

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
How HashMap works in Java?  
How ConcurrentHashMap works in Java?  
How SynchronizedHashMap works in Java?  
Multimap(Not from Guava, write your implementation)
How to sort values in HashMap?

Scenario based:
Can we override static method?  
if no whether it will be runtime error or compile time?  
If I have a student class with int id and String name and I put this in hashMap/TreeMap what will happen?  
Apply encapsulation in your Employee class    
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


# Additional Info:
use of '_' as an identifier might not be supported in releases after Java SE 8
