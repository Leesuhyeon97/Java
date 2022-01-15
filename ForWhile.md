# Java 

## 반복문

> 반복문을 활용해서 구구단을 출력하기
>
> 반복문에서 Continue 와 break 사용하기

### For 반복문

``` java
int i = 2;
for(int j=1; j<10; j++){
    System.out.print("2 * " + j + " = " + i*j);
}

//continue 사용
int i = 2;
for(int j=1; j<10; j++){
    if(j==4){continue;} // 4를 제외하고 반복되는 값을 출력됨
    System.out.print("2 * " + j + " = " + i*j);
}

//break를 안쓰는 이유는 반복의 범위가 정해져 있기 때문에. *(j<10)
```



### While 반복문

```java
i = 5; // i 대신 다른 변수를 적용해도 무관
int j = 0;
while(true){
    j++;
    System.out.print("5 * " + j + " = " + i*j);
}
/*변수의 값이 무한히 증가하기에 무한루프에 빠짐
해결책은 break를 사용하는 것.*/

//continue break 사용
i = 5;
int j = 0;
while(true){
    j++;
    if(j==4){continue;} // 4를 제외하고 반복되는 값을 출력
    System.out.print("5 * " + j + " = " + i*j);
    if(j==9){break;} // 무한히 반복하지 않고 9에서 반복을 멈춤
}
```



