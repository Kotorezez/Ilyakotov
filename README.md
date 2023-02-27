# Ilyakotov
abstract class Animal {
    String say;
    abstract void eat();
    abstract void sleep();
    abstract void talk();
}

class Hare extends Animal {
    Hare(){
      say="AA";
    }
    public void eat() {
        System.out.println("Заяц ест.");
    }

    public void sleep() {
        System.out.println("Заяц спит.");
    }

    public void talk() {
        System.out.println(say);
    }
}

class Tiger extends Animal {
    String eat22="тигр ест";
    String sleep12="тигр спит";
    Tiger(){
      say="RR";  
    }
    public void eat() {
        System.out.println(eat22);
    }

    public void sleep() {
        System.out.println(sleep12);
    }

    public void talk() {
        System.out.println(say);
    }
}

class Cat extends Tiger {
    Cat(){
        eat22="Кошка пьет";
    sleep12="Кошка дышит";
        
    }
    
}

public class AnimalProgram {
    public static void main(String[] args) {
        Animal chert = new Animal() {
            
            public void eat() {
                System.out.println("Animal ест.");
            }

            public void sleep() {
                System.out.println("Animal спит.");
            }

            public void talk() {
                System.out.println("Animal кричит");
            }
        };

        Hare hare = new Hare();
        Tiger tiger = new Tiger();
        Cat cat = new Cat();
        cat.say="mew";

        chert.eat();
        chert.sleep();
        chert.talk();

        hare.eat();
        hare.sleep();
        hare.talk();

        tiger.eat();
        tiger.sleep();
        tiger.talk();

        cat.eat();
        cat.sleep();
        cat.talk();
    }
}
