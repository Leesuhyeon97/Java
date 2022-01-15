<h1>Buffered Writer/Reader</h1>

> 버퍼를 이용해서 입/출력



### Buffer

* 데이터를 전송할 때 일시적으로 데이터를 보관하는 임시 메모리 영역



### Buffered Writer

* 버퍼를 이용한 입력
* System.out.println(""); 과 동일하게 사용가능
* 개행을 직접 해주지 않아서 "\n"이나 newLine함수 사용

| Modifier and Type |                    Method and Description                    |
| :---------------: | :----------------------------------------------------------: |
|       void        |           close(): 스트림 닫기, 닫기 전에 flushing           |
|       void        |                    flush(): 스트림 비우기                    |
|       void        |                     newLine(): 라인개행                      |
|       void        | write(char[] cbuf, int offset, int length): 버퍼 offset 위치부터 length크기만큼 write를 씀. |
|       void        |                  write(int c): 한글자 쓰기                   |
|       void        | write(String s, int offset, int length): 문자열에서 offset부터 일정 길이만큼 write를 씀 |



### Buffered Reader

* 버퍼를 이용한 출력

* readLine() 을 사용하면 데이터를 라인단위로 읽기 가능

* readLine 함수로 받은 리턴값은 String 으로 고정됨 (다른 타입으로 받기위해선 형변환이 필수)

* 공백단위로 데이터를 읽기위해선 "StringTokenizer"의 'nextToken'함수를 사용하거나 "String"클래스의 'split'함수를 이용하면 된다.

  | Modifier and Type |                    Method and Description                    |
  | :---------------: | :----------------------------------------------------------: |
  |       void        |     Close(): 입력 스트림을 닫고 사용하던 자원들을 푼다.      |
  |       void        |    mark(int,readAheadLimit): 스트림의 현재 위치를 마킹함.    |
  |      boolean      | markSupported(): 스트림이 mark기능을 지원하는지 true/false로 알려줍니다. |
  |        int        | read(): 한 글자만 읽어서 정수형으로 반환해줌. (3을 입력하면 '3'으로 읽고 '3'의 정수형인 51을 반환) |
  |        int        | read(char[] cbuf, int offset, int length): cbuf의 offset 위치부터 length길이만큼 문자를 스트림으로부터 읽어옴. |
  |      String       |        readLine(): 라인 하나를 읽어서 String으로 반환        |
  |      boolean      |      ready(): 입력스트림 사용준비를 알려줌 준비완료시 1      |
  |       void        | reset(): 마킹이 있으면 그 위치부터 다시시작 , 그렇지 않으면 처음부터 다시 시작. |
  |       long        |              skip(long n): n개의 문자를 건너뜀.              |

  

### Buffer flush

* 버퍼에 남아있는 데이터를 출력 (버퍼를 비움)











-자료참고: https://jhnyang.tistory.com/92