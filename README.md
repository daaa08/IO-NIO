#### IO

- IO : Input Output
- 입출력 방식 : Stream
- 버퍼방식 : non-buffer
- 비동기여부 : 지원안함
- 입력과 출력 두개가 필요

####  NIO  
###### (IO가 향상된 것)

- NIO : New Input Output
- 입출력 방식 : Channel (버퍼를 입출력하기위한 구조)
- 버퍼방식 : buffer
- 비동기여부 : 지원
- 입출력이 하나

![enter image description here](http://cfile3.uf.tistory.com/image/264BEE3455E13BC12F4759)


**그렇다면 왜 스트림을 쓰는가?**
-> 채널을 사용할 경우 쓰지 않는 일을 추가적으로 하기때문임... 자원 절약!
 
**대용량일 경우에는?**
-> IO가 효율적임. 왜냐, 메인 스레드가 돌고있기 때문임. NIO는 스레드를 생성해야 하기때문에 좀 더 느림. (IO도 스레드 생성은 가능)



#


###### _Buffer_ : 일정한 영역에 버퍼 메모리를 생성하여 미리 할당한 부분에서 입출력을 함 (처리 속도를 향상)

###### _~~Stream_ : 문자 이외에 모든 입출력이 가능

###### _~~Reader/Writer_ : 문자열만 입출력 가능

###### _스레드_ : 프로그램 실행의 단위로 하나의 프로세스는 여러개의 스레드로 구성이 가능(두가지 또는 그 이상을 동시에 실행 가능)

###### _동기_ : 상대방 신호를 받고 다음 동작을 실행

###### _비동기_ : 상대방의 상태와 관계없이 일방적으로 실행

###### _java.util_ : 자바 프로그래밍에서 유용한 유틸리티 클래스가 포함되어 있음
