import java.util.ArrayList;

abstract class  Livestock{
    String name;
    int age;

    public Livestock (String name, int age) {
        this.name = name;
        this.age = age;
        
    }
    abstract String makeSound();
    String makeSound(int volume) {
        return makeSound() + "(Volume: "+ volume +")";
    }
    void graze() {
        System.out.println(name + "talbaid belchine.");
    }
     
    void graze(String food) {
        System.out.println(name + " " +food+ "iig belchine");
    }
}

interface WorkRole {
    String performTask();
}

class Horse extends Livestock implements WorkRole {
    public Horse(String name, int age) {
        super(name, age);
    }
    @Override
    String makeSound() {
        return "Yntsgaana";
    }
    @Override
    public String performTask() {
        return "Mori talbaid unalgad hereglegdene";
    }
}

class Sheep extends Livestock {
    public Sheep(String name, int age) {
        super(name, age);
    }
    @Override
    String makeSound() {
        return "Maa";
    } 
}

class Camel extends Livestock implements WorkRole {
    public Camel(String name, int age) {
        super(name, age);
    }
    String makeSound() {
        return "Builna";
    }
    @Override
    public String performTask() {
        return "Temee goviin teevert haerglegdene";
    }
}
class Goat extends Livestock implements WorkRole{
    public Goat(String name, int age) {
        super(name, age);
    }
    String makeSound() {
        return "mai";
    }
    @Override
    public String performTask() {
        return "suu bolon noos nooluuriin uuregtei";
    }
}
class Cow extends Livestock  {
    public Cow (String name, int age) {
    super(name, age);
    }
    @Override
    String makeSound() {
        return "Moorno";
    } 
}
class Herd {
    ArrayList<Livestock> livestock = new ArrayList<>();

    void addLivestock(Livestock animal) {
        livestock.add(animal);
    }
    
void dailyRoutine() {
    for(Livestock animal : livestock) {
        System.out.println(animal.name +": " + animal.makeSound()) ;
        if(animal instanceof WorkRole) {
            System.out.println(((WorkRole) animal). performTask());
            }
        }
    }
}
 public class NomadLivestockDemo {
   public static void main (String[] args) {
    
    Livestock[] animal = {
    new Horse("Dorj", 4),
    new Sheep("Bataa", 6),
    new Camel("Suhee", 5),
    new Goat ("Boldoo",3),
    new Cow  ("Idree",7)
    };
    for (Livestock a : animal){
    a.graze();
    }

    for(Livestock a : animal) {
    System.out.println(a.name + "\t" + ":" +a.makeSound(10));    
    }
  }
}
