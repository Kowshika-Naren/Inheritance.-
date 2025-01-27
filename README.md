# Inheritance.-
package studentinheritanceexample;
import java.io.PrintStream;
abstract class Shape {
public abstract double calculateArea();
}
class Circle extends Shape {
private double radius;
public Circle(double radius) {
this.radius = radius;
}
@Override
public double calculateArea() {
return Math.PI * radius * radius;
}
}
class Rectangle extends Shape {
private double length, width;
public Rectangle(double length, double width) {
this.length = length;
this.width = width;
}

@Override
public double calculateArea() {
return length * width;
}
}
class Square extends Shape {
private double side;
public Square(double side) {
this.side = side;
}
@Override
public double calculateArea() {
return side * side;
}
}

class Triangle extends Shape {
private double base, height;
public Triangle(double base, double height) {
this.base = base;
this.height = height;
}

@Override
public double calculateArea() {
return 0.5 * base * height;
}
}

public class Studentinheritanceexample {

    /**ape triangle = new Triangle(3, 5);

System.out.println("Circle Area: "+ circle.calculateArea());
System.out.println("Rectangle Area: "+ rectangle.calculateArea());
System.out.println("Square Area: " + square.calculateArea());
System.out.println("Triangle Area: "+ triangle.calculateArea());
    }
}
Output:
Circle Area: 78.53981633974483
Rectangle Area: 24.0
Square Area: 16.0
Triangle Area: 7.5
