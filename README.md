# Bhumi_4th-2025
Aim: Create a class Animal with a method makeSound() that outputs a generic sound.The class should further contain derived classes Dog and Cat that override the makeSound() method to output specific sounds for each animal. Demonstrate polymorphism by creating an Animal reference that can hold objects of both Dog and Cat, and call the overridden makeSound() method at runtime.
code:
// Base class Animal
class Animal {
    // Method to be overridden by derived classes
    public void makeSound() {
        System.out.println("Some generic animal sound");
    }
}

// Derived class Dog
class Dog extends Animal {
    // Override the makeSound method to provide Dog-specific sound
    @Override
    public void makeSound() {
        System.out.println("Bark");
    }
}

// Derived class Cat
class Cat extends Animal {
    // Override the makeSound method to provide Cat-specific sound
    @Override
    public void makeSound() {
        System.out.println("Meow");
    }
}

public class Main {
    public static void main(String[] args) {
        // Creating objects of Dog and Cat
        Animal myDog = new Dog(); // Animal reference to Dog object
        Animal myCat = new Cat(); // Animal reference to Cat object
        
        // Calling the makeSound method using the references
        myDog.makeSound(); // Outputs: Bark
        myCat.makeSound(); // Outputs: Meow
    }
}

output:
Bark
Meow
