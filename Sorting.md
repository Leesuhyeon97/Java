<h1>Sorting</h1>

> Arrays.sort();

<h4>기본적으로 객체는 Comparable이 구현되어 있음
</h4>



* int 배열 정렬 (오름,내림 차순)

-defalut값은 오름차순

```java
int[] array = {1, 26, 19, 98, 77, 52, 34}; 

Arrays.sort(array); //배열 정리

System.out.println(Arrays.toString(array)); // 배열 정리된 값을 출력

---Output
    [1, 19, 26, 34, 52, 77, 98]
```



-내림차순

```java
Integer[] array = {1, 26, 19, 98, 77, 52, 34}

Arrays.sort(array, Collection.reverseOrder());

System.out.println(Arrays.toString(array));

--Output
    [98, 77, 52, 34, 26, 19, 1]
```



* int 배열 부분정렬

-전체를 정렬하는게 아닌 지정된 Index 범위만 정렬

```java
int[] array = {1, 26, 19, 98, 77, 52, 34}; 

Array.sort(array,0,5); //원하는 범위 설정 (배열, 시작, 끝)

System.out.println(Arrays.toString(array));

--Output
    [1, 19, 26, 77, 98, 52, 34]
```



* String 배열 정렬

-Integer와 동일하게 구현 (아스키 값으로 비교 정렬해줌)

```java
String[] array = {"Apple", "Kiwi", "Orange", "Banana", "Watermelon", "Cherry"};

Arrays.sort(array);

System.out.println(Arrays.toString(array));

--Output
    [Apple, Banana, Cherry, Kiwi, Orange, Watermelon]
    
*내림차순

Arrays.sort(array, Collection.reverseOrder());

System.out.println(Arrays.toString(array));

--Output
    [Watermelon, Orange, Kiwi, Cherry, Banana, Apple]

```



* String 배열, 문자 길이 순서대로 정렬

-직접 문자열 길이를 비교하는 Comparable을 구현해서 값을 출력해야함

```java
String[] array = {"Apple", "Kiwi", "Orange", "Banana", "Watermelon", "Cherry"};

//Compare 구현
Arrays.sort(array, new Comparator<String>(){
    //배열안의 String을 비교
    @Override
    public int compare(String s1, String s2){
        return s1.length()- s2.length();
    }
});

System.out.println(Arrays.toString(array));

--Output
    [Kiwi, Apple, Orange, Banana, Cherry, Watermelon]
```

 







*참고 https://codechacha.com/ko/java-sorting-array/