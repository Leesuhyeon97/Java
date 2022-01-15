<H1>Array</H1>

> 배열에 관한 문법



<h2>copyOf</h2>

> 배열 복사

```java
import java.util.Arrays;

public class Main{
    public static void main(String args[]){
        int [] arr1 ={1,2,3,4,5}; 
        int [] arr2 = Arrays.copyOf(arr1, arr1,length); // arr1을 복사 (복사할 배열, 배열의 길이)
        for(int i=0; i<arr2.length; i++){
            System.out.println(arr2[i]);
        }
    }
}
```

<h2>copyOfRange</h2>

> 배열 특정구간 복사

```java
import java.util.Arrays;

public class Main{
    public static void main(String args[]){
        int [] arr1 = {1, 2, 3, 4, 5}
        int [] arr2 = Arrays.copyOfRange(arr1, 0, 3); // arr1을 복사하는데 index0번부터 2번까지만 복사
        for(int i=0; i<arr2.length; i++){
            System.out.println(arr2[i]);
        }
    }
}


*arr1보다 범위를 크게 잡으면
    :초과된 범위값은 0으로 채워짐
```



