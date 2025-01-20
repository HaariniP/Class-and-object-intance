# Class-and-object-intance
class Car 
    String brand;
    String color;
    int speed;
    Car(String brand, String color, int speed) {
        this.brand = brand;
        this.color = color;
        this.speed = speed;
    }
    void displayDetails() {
        System.out.println("Brand: " + brand);
        System.out.println("Color: " + color);
        System.out.println("Speed: " + speed + " km/h");
    }
    void accelerate(int increase) {
        speed += increase;
        System.out.println("The car has accelerated. New speed: " + speed + " km/h");
    }
}
public class Main {
    public static void main(String[] args) {
        Car myCar = new Car("Toyota", "Red", 120);
        myCar.displayDetails();
        myCar.accelerate(30);  // Accelerate the car
    }
}
