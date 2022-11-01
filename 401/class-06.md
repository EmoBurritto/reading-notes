# Reading Class 06

## Java OO Tutorial (review Object and Class, read the rest)

An object is a software bundle of related state and behavior

A class is a blueprint or prototype from which objects are created

Inheritance provides a powerful and natural mechanism for organizing and structuring your software

An interface is a contract between a class and the outside world

A package is a namespace for organizing classes and interfaces in a logical manner

Hiding internal state and requiring all interaction to be performed through an object's methods is known as data encapsulation

class Bicycle {

    int cadence = 0;
    int speed = 0;
    int gear = 1;

    void changeCadence(int newValue) {
         cadence = newValue;
    }

    void changeGear(int newValue) {
         gear = newValue;
    }

    void speedUp(int increment) {
         speed = speed + increment;   
    }

    void applyBrakes(int decrement) {
         speed = speed - decrement;
    }

    void printStates() {
         System.out.println("cadence:" +
             cadence + " speed:" + 
             speed + " gear:" + gear);
    }
}

class BicycleDemo {
    public static void main(String[] args) {

        // Create two different 
        // Bicycle objects
        Bicycle bike1 = new Bicycle();
        Bicycle bike2 = new Bicycle();

        // Invoke methods on 
        // those objects
        bike1.changeCadence(50);
        bike1.speedUp(10);
        bike1.changeGear(2);
        bike1.printStates();

        bike2.changeCadence(50);
        bike2.speedUp(10);
        bike2.changeGear(2);
        bike2.changeCadence(40);
        bike2.speedUp(10);
        bike2.changeGear(3);
        bike2.printStates();
    }
}
class MountainBike extends Bicycle {

    // new fields and methods defining 
    // a mountain bike would go here

}

class ACMEBicycle implements Bicycle {

    int cadence = 0;
    int speed = 0;
    int gear = 1;

   // The compiler will now require that methods
   // changeCadence, changeGear, speedUp, and applyBrakes
   // all be implemented. Compilation will fail if those
   // methods are missing from this class.

    void changeCadence(int newValue) {
         cadence = newValue;
    }

    void changeGear(int newValue) {
         gear = newValue;
    }

    void speedUp(int increment) {
         speed = speed + increment;   
    }

    void applyBrakes(int decrement) {
         speed = speed - decrement;
    }

    void printStates() {
         System.out.println("cadence:" +
             cadence + " speed:" + 
             speed + " gear:" + gear);
    }
}

(reference: https://docs.oracle.com/javase/tutorial/java/concepts/)

## Java Static Keyword

If we want to access class members without creating an instance of the class, we need to declare the class members static

Static methods are also called class methods. It is because a static method belongs to the class rather than the object of a class

class StaticTest {

    // non-static method
    int multiply(int a, int b){
        return a * b;
    }

    // static method
    static int add(int a, int b){
        return a + b;
    }
}

public class Main {

   public static void main( String[] args ) {

        // create an instance of the StaticTest class
        StaticTest st = new StaticTest();

        // call the nonstatic method
        System.out.println(" 2 * 2 = " + st.multiply(2,2));

        // call the static method
        System.out.println(" 2 + 3 = " + StaticTest.add(2,3));
   }
}
(reference: https://www.programiz.com/java-programming/static-keyword)

## Java Singleton Class




(reference: https://www.programiz.com/java-programming/singleton)

## Questions

1. What is the difference between an Object and a Class in Java?

An object is a software bundle of related state and behavior

A class is a blueprint or prototype from which objects are created

2. What is a Design Pattern? Describe one or two with analogies from your previous work experience.

3. Static methods are also called what? Why?

Static methods are also called class methods. It is because a static method belongs to the class rather than the object of a class