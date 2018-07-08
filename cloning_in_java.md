   **Summary**
1. implements Cloneable
2. __super.clone__ throws **CloneNotSupportedException** if the CLass overriding clone method does not **implement Cloneable**  
3. override Object's clone method and call __super.clone()__
4. two types of cloning : **Deep copy** __vs__ **Shallow Copy**



1. implements Cloneable
  Cloneable is a **Marker interface**. A marker interface is an interface that does not contain any method. Its sole purpose is to tell the JVM that the class implementing this interface need the clone of it. Marker Interfaces are not written after JAVA 5 as they were replaced by Annotations after that.
  
2. __super.clone__ throws **CloneNotSupportedException** if the CLass overriding clone method does not **implement Cloneable**  
   Object class has protected clone method as below:
   ```
   protected native Object clone() throws CloneNotSupportedException;
   ```
   In order to create a clone we have to override this method and call **super.clone** expicitly,   which makes JVM to create copy for the specified object. But, for this it checks if the class overriding this method implements Cloneable interface or not, if not it throws **CloneNotSupportedException**
   
   3. override Object's clone method
   super.clone() creates copy of all the primitives and its Wrapper(i.e immutable classes) and assign it to the new Object.  
   So, Default behavior of super.clone() in this scenario works fine
   ```
   public Object clone() throws CloneNotSupportedException{
   		return super.clone();
   	}
   ```
  Hence, Every time you 
  
**Deep Copy vs Shallow Copy  
**Why do we need to clone?  
**Default java   
**How to Clone Object in Java?  
