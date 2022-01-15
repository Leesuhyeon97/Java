# Exception

> 예외





## Exception 처리

### try catch

### throws



* 서버에서 throws Exception 을 하면 클라이언트에서  throws 를 받아서 코드를 만들면 자동화 코드가 생성된다.

* 보안상의 문제로 잘 쓰지 않음

```java
package test2.exception;

public class DivideTest {

	public static void main(String[] args) {
		Divider d = new Divider();
		try {
			d.divide(100, 0);
		} catch (Exception e) {
			// 복구코드
			//e.printStackTrace(); 보안상에 문제가 생겨서 잘 쓰지 않음
		}
		System.out.println("뭔가 중요한 일");
	}
}
```

##  Exception 발생

### throw new ` @@`Exception

