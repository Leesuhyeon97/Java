# Java

> Web을 target으로한 범용 언어

## 특징

> 개발자 편의성을 추구 <->성능 저하

---

* OOP

> Reuse

* Platform Independent

> WORA

* Multi -Thread

> Web 필수

* Security

> Web 필수

* Garbage Collector

> 메모리 관리

* Exception

> Robust 프로그램을 쉽게 구축

## Class

> program 단위

### abstract

* 상속으로만 사용
* 객체화 불가
* method에 override 강제
* 단일상속
* data는 상수만 가능, method는 all abstract
* less OOP

### interface

* 상속으로만 사용
* 객체화 불가 (생성자 불가)
* override 강제
* 다중상속
* data는 상수만 가능, method는 all abstract
* more OOP



## Data

> Object 속성

### Object

> Class의 Instance

모든 구체적 + 관념적 사물

### Data Type

#### Primitive

> 이름 + 값

* 정수
  * byte,short,int,long
* 실수
  * float,double
* 단문
  * char
* 논리
  * boolean

#### Reference

> 이름 + 주소

* Class, 배열, Interface, Enum

## Method

> Object 행위

## OOP 3대 개념

### Encapsulation

* Data-private
* Method-public
  * 제한 필요 : (defalut), protected 고려
* Setter/Getter

### Inheritance

* Extends 단일상속
  * 제외 : private member + 생성자

### Polymorphism

* Polymorphic variable
  * ex) Object o
* Overriding
  * Utility(Service)>biz(Super s)>Super의 하위 클래스들 = 제약 + 다양성
  * Shadow effect 발생 -> 해제 필요시(If사용, 타입체크, 타입캐스팅 필요 = 성능,확장성에 최악)
  * Shadow effect 해결하기 위해 Overriding 사용
* Overloading
  * 메소드를 같게

## Modifier

### access

### usage

* static : 객체 생성 없이 사용
  * class(inner class에서만)
  * data앞 : 공유데이터에서만
  * method앞
* final : 변경없이 사용
  * class앞 : 상속 불가 ex) String
  * data앞 : 상수
  * method앞 : override 불가 
* abstract : 상속으로만 사용
  * class앞 : 객체 생성 불가
  * method앞 : 구현 안된 메소드 ex) shape-area

## 배열

> 같은 type의 data를 모아놓을 수 있는 자료 구조

* 독립적인 program 단위 아님
* `type-(원소타입) []-(객체 타입) 이름 = new type-(원소타입) [];`
  * 이름[index] = 값; ->할당
  * 이름[index] -> 회수

## Exception

```java
try{
    catch(하위exception e){
    }
    catch(하위exception e){
    }
    catch(상위exception e){
    }
    finally{ //위의 exception에서 에러를 못잡아도 반드시 마지막에 수행하는 블락 ex) 자원해제
    }
}
```





