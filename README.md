# JVM
## Код для исследования
```java

public class JvmComprehension {

    public static void main(String[] args) {
        int i = 1;                      // 1
        Object o = new Object();        // 2
        Integer ii = 2;                 // 3
        printAll(o, i, ii);             // 4
        System.out.println("finished"); // 7
    }

    private static void printAll(Object o, int i, Integer ii) {
        Integer uselessVar = 700;                   // 5
        System.out.println(o.toString() + i + ii);  // 6
    }
}

```
## 
- ClassLoader'ы беспечивает загрузку классов Java. загружаем JvmComprehension загружается в Application
- области памяти (стэк (и его фреймы), хип, метаспейс)  
метаспейс
JvmComprehension.class
system.classes
В стаэке хранятся фреймы
main (int i,o, Integer ii = 2)
printAll (o,int i, Integer ii, Integer uselessVar)
toString(o)
System.out.println(o,i,ii)
хип
 Object
 String

- сборщик мусора
