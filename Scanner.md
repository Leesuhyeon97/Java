<h1>Scanner</h1>



*Scanner 객체 생성 방법

```java
import java.util.Scanner;
---
Scanner sc = new Scanner(System.in) 
```



*Scanner의 메소드

```java
import java.util.Scanner;

public class Main{
    public static void main(String args[]){
        Scanner sc = new Scanner(System.in)
            
            byte a = sc.nextByte();
        	short b = sc.nextShort();
        	int c = sc.nextInt();
        	long d = sc.nextInt();
        
        	float e = sc.nextFloat();
        	double f = sc.nextDouble();
        
        	boolean g = sc.nextBoolean();
        
        	String h = sc.next();//공백기준 단어읽기
        	String i = sc.nextLine();//라인개행기준 줄읽기
        *char : String으로 받은 뒤, charAt()메소드로 반환
    }
}
```

