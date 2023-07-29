# Basics

## 1- String equal with or without Case

```java
package test;
import java.util.Scanner;

public class Main {
    public static void main(String[] args) {
        Scanner input = new Scanner(System.in);

        System.out.print("Enter Your Site: ");
        String site = input.next();
        String xSite = "www.ali.net";

        if(xSite.equalsIgnoreCase(site)){
            System.out.println("ok");
        }else {
            System.out.println("Not ok");
        }

    }
}
```

----

## 2- Array

```java
//way 1:

package test;

public class Main {
    public static void main(String[] args) {
       int[] z = new int[5];

       z[0] = 1;
       z[1] = 2;
       z[2] = 3;
       z[3] = 4;

        System.out.println(z[0]);
        

    }
}
```

```java
//Way 2:
package test;

public class Main {
    public static void main(String[] args) {
        int[] z = {1, 2, 3, 4};
        System.out.println(z[3]);
    }
}
```

```java
package test;

public class Main {

    public static int[] createArray(int size){

        return new int[size];
    }

    public static void main(String[] args) {
        //Variable size array
        int[] z = createArray(5);
        System.out.println(z.length);

        //fixed size array
        int[] x = new int[8];
        int[] y = {1, 2, 3};

    }
}
```

```java
package test;

public class Main {

    public static void main(String[] args) {

        int [] a = {1, 2, 3, 4};
//       way 1 to access array
        System.out.println("=======================Way 1================");

        for(int i = 0; i < a.length; i++){
            System.out.println(a[i]);
        }
//       way 2 to access array
        System.out.println("=======================Way 2================");

        for(int value : a){
            System.out.println(value);
        }

    }
}
```

```jav
// 2-D array
package test;

public class Main {

    public static void main(String[] args) {

        int [][] x = {
                {1, 2, 3},
                {4, 5, 6},
                {7, 8, 9}
        };

        System.out.println(x[2][0]);


    }
}
```


