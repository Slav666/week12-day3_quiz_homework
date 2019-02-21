# Polymorphism & Composition Homework - Quiz

# Polymorphism

1. What does the ___word___ 'polymorphism' mean?

many forms

2. What does it mean when we apply polymorphism to OO design? Give a simple Java example.

For example, lets say we have a class Animal that has a method sound(). Since this is a generic class so we can’t give it a implementation like: Roar, Meow, Oink etc. We had to give a generic message.

public class Animal{
   ...
   public void sound(){
      System.out.println("Animal is making a sound");   
   }
}

Now lets say we two subclasses of Animal class: Horse and Cat that extends Animal class. We can provide the implementation to the same method like this:

public class Horse extends Animal{
...
    @Override
    public void sound(){
        System.out.println("Neigh");
    }
}
and

public class Cat extends Animal{
...
    @Override
    public void sound(){
        System.out.println("Meow");
    }
}
As you can see that although we had the common action for all subclasses sound() but there were different ways to do the same action.

3. What can we use to implement polymorphism in Java?

Implementing it in classes and casting.

4. How many 'forms' can an object take when using polymorphism?

As many as it has interfaces.

5. Give an example of when you could use polymorphism.

When two unrelated classes need to use the same Method, or when they need to be categorised together.

Let's say we what to create ZOO which is represented by different classes of animals, some animals
need to be able to perform the same action, but are otherwise unrelated. (all animals can make a sound but not all can eat meat)



# Composition

6. What do we mean by 'composition' in reference to object-oriented programming?

It describes a class that references one or more objects of other classes in instance variables.
This allows you to model a has-a association between objects.

7. When would you use composition? Provide a simple example in Java.

8. What is/are the advantage(s) of using composition?

When an Object is required to rely on a certain property of a series of subclasses. For example if a system requires the ability to output information (e.g. print it to screen), but the exact mechanism/class which implements this feature does not need to be set, or can be subject to change.

Stronger, reusable code.

9. What happens to the behaviours when the object composed of them is destroyed?

I don't know.
