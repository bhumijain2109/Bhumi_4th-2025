# Bhumi_4th-2025
Aim: Create a class Animal with a method makeSound() that outputs a generic sound.The class should further contain derived classes Dog and Cat that override the makeSound() method to output specific sounds for each animal. Demonstrate polymorphism by creating an Animal reference that can hold objects of both Dog and Cat, and call the overridden makeSound() method at runtime.
code:
class Animal {
    public void makeSound() {
        System.out.println("Some generic animal sound");
    }
}
class Dog extends Animal {
    public void makeSound() {
        System.out.println("Bark");
    }
}
class Cat extends Animal {
    public void makeSound() {
        System.out.println("Meow");
    }
}

public class Main {
    public static void main(String[] args) {
        Animal myDog = new Dog(); // Animal reference to Dog object
        Animal myCat = new Cat(); // Animal reference to Cat object
        myDog.makeSound(); // Outputs: Bark
        myCat.makeSound(); // Outputs: Meow
    }
}

output:
Bark
Meow
