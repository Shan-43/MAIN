# MAIN
public class MyClass {
    static int staticCounter = 0;    // static
    int instanceCounter = 0;        // non-static

    public void increment() {
        staticCounter++;
        instanceCounter++;
    }

    public void display() {
       System.out.println("Static: " + staticCounter);
       System.out.println("Instance: " + instanceCounter);
    }

    public static void main(String[] args) {
        MyClass obj1 = new MyClass();
        MyClass obj2 = new MyClass();

        obj1.increment();
        obj2.increment();

        obj1.display();
        obj2.display();
    }
}
