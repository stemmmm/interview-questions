# interview-questions
기술 면접 대비를 위한 아카이브입니다.

<br>

# 목차
- [Java](#Java)
- [프로그래밍 일반](#프로그래밍-일반)
- [컴퓨터구조](#컴퓨터구조)
- [자료구조](#자료구조)
- [알고리즘](#알고리즘)
- [운영체제](#운영체제)
- [네트워크](#네트워크)
- [데이터베이스](#데이터베이스)
- [디자인 패턴](#디자인-패턴)
- [Spring](#Spring)

<br>

# Java
- [자바의 컴파일 과정](https://velog.io/@stemmmm/자바의-플랫폼-독립성)
- [자바 가상 머신(Java Virtual Machine, JVM)](https://velog.io/@stemmmm/jvm)
- [가비지 컬렉션(Garbage Collection, GC)](https://velog.io/@stemmmm/gc)
- 기본 타입(Primitive type) vs 참조 타입(Reference type)
- Call by value vs Call by reference
  - 각각의 개념과 그 차이에 대해 설명하세요.
  - 과연 모든 언어에 이 개념이 존재할까요?
- `equals()`와 `hashCode()`
  - 각각의 메서드가 어떤 역할을 하는지, 그리고 두 메서드의 관계에 대해 설명하세요.
  - `hashCode()`를 직접 정의해야 한다면, 어떤 점을 염두에 두고 구현 하실건가요?
  - `equals()`를 재정의 해야 할 때, 어떤 점을 염두에 두어야 하는지 설명해 주세요.
- `String` vs `StringBuffer` vs `StringBuilder`
  - 각각의 개념과 그 차이에 대해 설명하세요.
  - Interend String에 대해 설명하세요.
- 업캐스팅과 다운캐스팅
- `static`
  - `static` 키워드가 붙은 변수나 함수는 어떻게 처리되나요?
  - 내부 클래스에서 `static` 키워드의 사용을 권장하는 이유를 설명해주세요.
- `final`
  - `final` 키워드가 붙은 클래스의 메서드는 어떻게 동작하나요?
- [래퍼(Wrapper) 클래스](https://inpa.tistory.com/entry/JAVA-☕-wrapper-class-Boxing-UnBoxing#)
- 접근 제어자 (Access modifier)
- [예외 처리](https://www.nextree.co.kr/p3239)
- Collection 프레임워크
  - [List](https://youtu.be/xvi-n11kym0?si=hrrp0Gp1sMtpqUBr)
  - [Map](https://youtu.be/ZBu_slSH5Sk?si=gynzgQ5bfDM-8F_X)
  - [Set](https://youtu.be/IkImFugfFQk?si=um8MLIsSuSvVXO28)
  - [HashMap 동작원리](https://d2.naver.com/helloworld/831311)
  - [Map과 `equals()`, `hashCode()`의 상관관계](https://youtu.be/Dmo3sG-ZFTw?si=aEElbcjDgOp2gLM_)
  - [Synchronized Collection vs Concurrent Collection](https://steady-coding.tistory.com/575)
- 쓰레드(Thread)
  - `Thread`의 활용 방법과 주의점에 대해 설명하세요. 
  - `ThreadLocal`에 대해 설명해 주세요. 
- [`synchronized`](https://velog.io/@stemmmm/Monitor와-Java의-synchronized-키워드)
  - 효율적인 코드 작성 측면에서, `synchronized`는 좋은 키워드일까요?
  - `synchronized`를 대체할 수 있는 자바의 다른 동기화 기법에 대해 설명하세요.
- Stream API와 람다식
  - Stream API의 개념과 활용법에 대해 설명하세요.
  - 람다식의 개념과 사용법에 대해 설명하세요.
  - Stream과 for문의 성능을 비교하세요.
  - Stream을 병렬처리 할 수 있나요?
  - Stream에서 사용할 수 있는 함수형 인터페이스에 대해 설명해 주세요.
  - 가끔 외부 변수를 사용할 때, `final` 키워드를 붙여서 사용하는데 왜 그럴까요? 꼭 그래야 할까요?
- 직렬화(Serialization)
- 리플렉션(Reflection)
    - 리플렉션의 개념과 사용법에 대해 설명하세요.
    - 의미만 들어보면 리플렉션은 보안적인 문제가 있을 가능성이 있어보이는데, 실제로 그렇게 생각하시나요? 만약 그렇다면, 어떻게 방지할 수 있을까요?
    - 리플렉션을 언제 활용할 수 있을까요?
- 어노테이션(Annotation)
  - 자바에서 어노테이션은 어떤 기능을 하나요?
  - 별 기능이 없는 것 같은데, 어떻게 Spring에서는 어노테이션이 그렇게 많은 기능을 하는 걸까요?
  - Lombok의 @Data를 잘 사용하지 않는 이유는 무엇일까요?
- 인터페이스와 추상 클래스의 차이
- [제네릭(Generic)](https://dev.java/learn/generics/)
  - [Heap pollution](https://inpa.tistory.com/entry/JAVA-☕-제네릭-힙-오염-Heap-Pollution-이란) 
- 레코드(Record)

<br>

# 프로그래밍 일반
- [프로그래밍 패러다임](https://velog.io/@stemmmm/프로그래밍-패러다임)
  - [객체 지향 프로그래밍(Object-Oriented Programming, OOP)](https://velog.io/@stemmmm/oop)
    - [SOLID](https://velog.io/@stemmmm/solid)
    - Composition의 개념과 활용 방법
    - 왜 클래스는 단일 상속만 가능한데, 인터페이스는 2개 이상 구현이 가능할까요?
  - 함수형 프로그래밍(Functional Programming)
    - 순수 함수와 함수형 프로그래밍 매커니즘의 연관성에 대해 설명하세요.
    - Side-effect가 무엇인가요? 이를 모두 없애는 프로그래밍이 이상적이라고 할 수 있을까요?
    - 왜 함수형 프로그래밍 매커니즘을 사용할까요?
    - 순수 함수는 thread-safe 한가요? 그렇다면 왜 그럴까요?
    - 고차 함수에 대해 설명하세요.
- [프레임워크 vs 라이브러리](https://github.com/stemmmm/interview-questions?tab=readme-ov-file)
- RESTful API
- Blocking vs Non-blocking I/O
- Synchronous와 Asynchronous의 차이
- TDD(Test Driven Development)
- 애자일 소프트웨어 개발
- 데브옵스(DevOps)
- Git과 GitHub
- 가상화와 가상 머신
  - 가상화와 가상 머신의 차이를 설명하세요.
  - 그렇다면 도커(Docker)는 둘 중 어디에 속하나요? 왜 사람들이 도커를 많이 채택할까요?
  - 하나의 Host OS에서 돌아간다면, 한 컨테이너가 다른 컨테이너에 간섭할 수 있는 위험이 있지 않을까요? 이를 어떻게 방어할 수 있을까요?
  - 도커 위에 도커를 올릴 순 없을까요?
- 인증 vs 인가
- OAuth
- JWT(JSON Web Token)
  - JWT 인증 방식에 대해 설명하세요.
  - Signature는 어떻게 만들어지나요?
  - 만약 access token이 탈취되면, 어떻게 대응해야 할까요?
  - 반대로 refresh token이 탈취되면, 어떻게 대응해야 할까요?
- Base64 인코딩

<br>

# 컴퓨터구조
- 폰 노이만 구조
- 컴퓨터의 구성 요소
- 중앙 처리 장치(CPU)
  - 32비트와 64비트 컴퓨터의 차이는 무엇인가요?
  - 32비트와 64비트 컴퓨터에서 사용할 수 있는 메모리의 최대 크기는 얼마인가요? 왜 그런건가요?
  - CPU의 작동 원리에 대해 설명하세요.
- 캐시 메모리
- 고정 소수점 표현 방식과 부동 소수점 표현 방식
- 패리티 비트와 해밍 코드

<br>

# 자료구조
- 시간 복잡도와 공간 복잡도
  - Big-O, Big-Theta, Big-Omega 표기법에 대해 설명하세요.
  - 다른 표기법 사용하지 않고, Big-O를 사용하는 이유가 있을까요?
  - O(1)은 O(n^2)보다 무조건 빠른가요?
- 배열(Array)
- ArrayList vs 배열
- 연결 리스트 (Linked List)
  - 연결 리스트를 배열과 비교하며 설명하세요.
  - 연결 리스트를 사용해서 구현할 수 있는 다른 자료구조에 대해 설명하세요.
- 스택(Stack)과 큐(Queue)
  - 스택과 큐의 개념과 주요 연산에 대해 설명하세요.
  - 스택 2개로 큐를 만드는 방법과 그 시간 복잡도를 설명하세요.
  - 큐 2개로 스택을 만드는 방법과 그 시간 복잡도를 설명하세요.
  - 시간 복잡도를 유지하면서, 배열로 스택과 큐를 구현할 수 있을까요?
  - Prefix, infix, postfix 표기법에 대해 설명하고, 이를 스택을 활용하여 계산하는 방법에 대해 설명하세요.
  - 덱(Deque)은 어떻게 구현할 수 있을까요?
- 그래프(Graph)
  - 그래프의 개념과 2가지 구현법에 대해 설명하세요.
  - 각 방법에 대해, 두 정점이 연결되었는지 확인하는 시간 복잡도와 한 정점에 연결된 모든 정점을 찾는 시간 복잡도를 비교하세요. 추가로, 공간 복잡도를 비교하세요.
  - 정점의 개수가 n개, 간선의 개수가 n^3개인 그래프는 어떤 방식으로 구현하는 것이 효율적일까요?
  - 탐색
    - 그래프에서 최단거리를 구하는 방법에 대해 설명해 주세요.
    - 정점의 개수가 n개, 간선의 개수가 n^3 개라면, 어떤 알고리즘으로 그래프를 탐색하는 것이 효율적일까요?
- 트리(Tree)
  - 그래프와 트리의 차이를 설명하세요.
  - 사이클이 없는 그래프는 모두 트리인가요? 그렇지 않다면, 예시를 들어주세요.
  - 이진탐색트리 (Binary Search Tree, BST)
    - BST에서 중위 탐색을 하게 되면, 그 결과는 어떤 의미를 가지나요?
    - BST의 주요 연산에 대한 시간 복잡도를 설명하고, 왜 그런 시간복잡도가 도출되는지 설명하세요.
    - BST의 한계점에 대해 설명하세요.
    - BST의 값 삽입, 삭제 방법에 대해 설명하고, 어떤 식으로 값을 삽입하면 편향이 발생하는지 설명하세요.
    - BST와 동일한 로직을 사용하여 삼진 탐색 트리도 정의할 수 있을까요? 그리고 그 이유에 대해 설명하세요.
  - B-Tree와 B+Tree에 대해 설명하세요.
  - 레드-블랙 트리 (Red-Black Tree)
    - 레드-블랙 트리의 균형 유지 방법에 대해 설명하세요.
    - 레드-블랙 트리의 주요 성질 4가지에 대해 설명하세요.
    - 2-3-4 트리, AVL 트리 등의 다른 BBST가 있음에도, 왜 레드-블랙 트리가 많이 사용될까요?
- 힙(Heap)
  - 힙을 배열로 구현한다고 가정하면, 어떻게 값을 저장할 수 있을까요?
  - 힙의 삽입, 삭제 방식에 대해 설명하고, 왜 이진 탐색 트리와 달리 편향이 발생하지 않는지 설명하세요.
  - 힙 정렬의 시간 복잡도는 어떻게 되나요? Stable한가요?
- 해시(Hash)
  - 값이 주어졌을 때, 어떻게 하면 충돌이 최대한 적은 해시 함수를 설계할 수 있을까요?
  - 해시 값이 충돌했을 때, 어떤 방식으로 처리할 수 있을까요?
  - 본인이 사용하는 언어에서는, 어떤 방식으로 해시 충돌을 처리하나요?
  - Double hashing 의 장점과 단점에 대해서 설명하고, 단점을 어떻게 해결할 수 있을지 설명하세요.
  - Load factor에 대해 설명하세요. 본인이 사용하는 언어에서의 해시 자료구조는 load factor에 관련한 정책이 어떻게 구성되어 있나요?
  - 다른 자료구조와 비교하여, 해시 테이블은 멀티스레드 환경에서 심각한 수준의 race condition 문제에 빠질 위험이 있습니다. 성능 감소를 최소화 한 채로 해당 문제를 해결할 수 있는 방법을 설명하세요.
- 트라이(Trie)
- Thread-safety
  - Thread-safe한 자료구조가 있을까요? 없다면, 어떻게 thread-safe한 자료구조를 만들 수 있을까요? 
  - 배열의 길이를 알고 있다면, 조금 더 빠른 Thread Safe 한 연산을 만들 순 없을까요?
  - 사용하고 있는 언어의 자료구조는 Thread Safe 한가요? 그렇지 않다면, Thread Safe 한 Wrapped Data Structure 를 제공하고 있나요?
 
<br>

# 알고리즘
- DFS와 BFS
- 재귀(Recursion)
  - 재귀 함수의 동작 과정을 콜 스택과 함께 설명하세요.
  - 언어의 스펙에 따라, 재귀 함수의 최적화를 진행해주는 경우가 있습니다. 어떤 경우에 재귀함수의 최적화가 가능하며, 그 원리를 설명해주세요.
- 정렬(Sort)
  - 거품 정렬(Bubble sort), 선택 정렬(Selection sort), 삽입 정렬(Insertion sort)
    - Bubble, selection, insertion sort의 속도를 비교하세요.
    - 값이 거의 정렬되어 있거나 완전히 정렬되어 있다면, 위 세 알고리즘의 속도 비교 결과는 달라질까요?
  - 퀵 정렬(Quick sort), 병합 정렬(Merge sort)
    - 퀵 정렬과 병합 정렬을 비교하세요.
    - 퀵 정렬에서 O(n^2)이 걸리는 경우의 예시를 들고, 이를 개선할 수 있는 방법에 대해 설명하세요.
    - 병합 정렬을 재귀를 사용하지 않고 구현할 수 있을까요?
  - 힙 정렬(Heap sort)에 대해 설명하세요.
  - 기수 정렬(Radix sort)과 계수 정렬(Counting sort)에 대해 설명하세요.
  - Stable sort가 무엇이고, 위 모든 정렬 알고리즘 중 어떤 것이 stable 한지 설명하세요.
  - 본인이 사용하고 있는 언어에서 제공하는 정렬 함수의 정렬 알고리즘을 설명하세요.
  - 정렬해야 하는 데이터는 50G 인데, 메모리가 4G뿐이라면, 어떤 방식을 사용해 정렬할 수 있을까요?
- 동적 계획법(Dynamic Programming)
  - 그리디 알고리즘과 동적 계획법을 비교하고, 어떤 경우에 각각의 기법을 사용하는지 설명하세요.
  - 동적 계획법으로 풀 수 있는 모든 문제는 재귀로 변환하여 풀 수 있나요?
- 이진 탐색(Binary Search)
  - Lower bound와 Upper bound 는 무엇이고, 이를 어떻게 구현할 수 있을까요?
  - 이진 탐색의 논리를 적용하여 삼진 탐색을 작성한다고 가정한다면, 시간 복잡도는 어떻게 달라질까요? (실제 존재하는 삼진탐색 알고리즘 무시하세요)
  - 기존 이진 탐색 로직에서 부등호의 범위가 바뀐다면, (e.g. <=를 <로) 결과가 달라질까요? 달라진다면 어떻게 달라질까요?
- 비트마스크(BitMask)

<br>

# 운영체제
- 시스템 콜
- 프로세스 vs 쓰레드
- 프로세스 주소 공간
- 단기, 중기, 장기 스케줄러
- CPU 스케줄링 알고리즘
- [동기화](https://velog.io/@stemmmm/series/동기화)
  - [Critical Section과 Race Condition](https://velog.io/@stemmmm/Critical-Section과-Race-Condition)
  - [Mutex Lock과 Semaphore](https://velog.io/@stemmmm/Mutex-Lock과-Semaphore)
  - [Monitor와 Java의 synchronized 키워드](https://velog.io/@stemmmm/Monitor와-Java의-synchronized-키워드)
  - [Deadlock](https://velog.io/@stemmmm/Deadlock)
- 메모리 관리 전략
- 가상 메모리
- 파일 시스템
- 캐시

<br>

# 네트워크
- www.google.com 을 브라우저에 입력했을 때 일어나는 일
- 웹 서버와 웹 애플리케이션 서버의 차이
- URL, URI, URN의 차이
- OSI 7 계층
  - Transport layer와, Network layer의 차이에 대해 설명하세요.
  - L3 Switch와 Router의 차이에 대해 설명하세요.
  - 각 layer는 패킷을 어떻게 명칭하나요? (e.g. Transport layer의 경우 segment)
  - 각 헤더의 packing order에 대해 설명하세요.
  - ARP에 대해 설명하세요.
- TCP
  - TCP의 특징에 대해 설명하세요.
  - TCP가 신뢰성을 보장하는 방법에 대해 설명하세요.
  - TCP의 혼잡 제어 처리 방법에 대해 설명하세요.
  - TCP의 흐름 제어 방법에 대해 설명하세요.
  - 3-way handshake
    - ACK나 SYN 같은 정보는 어떻게 전달할까요?
    - 2-way handshaking 를 하지않는 이유에 대해 설명하세요.
    - 두 호스트가 동시에 연결을 시도하면, 연결이 가능한가요? 가능하다면 어떻게 통신 연결을 수행하나요?
    - SYN flooding 에 대해 설명하세요.
    - 위 질문과 모순될 수 있지만, 3-way handshake의 속도 문제 때문에 이동 수를 줄이는 0-RTT 기법을 많이 적용하고 있습니다. 어떤 방식으로 가능한 걸까요?
  - 4-way handshake
    - 패킷이 4-way handshake 목적인지 어떻게 파악할 수 있을까요?
    - 4-way handshake를 할 여유가 없어 연결을 빨리 끊어야 하는 경우엔 어떻게 할까요?
    - 4-way handshake 과정에서 중간에 한쪽 네트워크가 강제로 종료된다면, 반대쪽은 이를 어떻게 인식할 수 있을까요?
    - 왜 종료 후에 바로 끝나지 않고, TIME_WAIT 상태로 대기하고 있을까요?
- UDP
  - UDP의 특징과 사용 사례를 설명하세요.
  - TCP와 UDP의 차이점
    - Checksum이 무엇인가요?
    - TCP와 UDP 중 어느 프로토콜이 Checksum을 수행할까요?
    - 그렇다면, checksum을 통해 오류를 정정할 수 있나요?
  - 그런데, 브라우저는 특정 서버가 TCP를 쓰는지 UDP를 쓰는지 어떻게 알 수 있나요?
  - 본인이 새로운 통신 프로토콜을 TCP나 UDP를 사용해서 구현한다고 하면, 어떤 기준으로 프로토콜을 선택할건가요?
- 멀티플렉싱과 디멀티플렉싱
  - 멀티플렉싱과 디멀티플렉싱에 대해 설명하세요.
  - 디멀티플렉싱의 과정에 대해 설명하세요.
- IP
  - IP 주소는 무엇이며, 어떤 기능을 하고 있나요?
  - IPv4와 IPv6의 차이에 대해 설명해 주세요.
  - IPv6는 IPv4의 주소 고갈 문제를 해결하기 위해 만들어졌지만, 아직도 수많은 기기가 IPv4를 사용하고 있습니다. 그렇다면 IP 고갈 문제를 어떻게 해결할 수 있을까요?
  - 수많은 사람들이 유동 IP를 사용하고 있지만, 수많은 공유기에서는 고정 주소를 제공하는 기능이 이미 존재합니다. 어떻게 가능한 걸까요?
  - IPv4를 사용하는 장비와 IPv6를 사용하는 같은 네트워크 내에서 통신이 가능한가요? 가능하다면 어떤 방법을 사용하나요?
  - IP는 송신자와 수신자간 정확한 전송을 보장해 주나요?
  - IPv4에서 수행하는 checksum과 TCP에서 수행하는 checksum은 어떤 차이가 있나요?
  - TTL(Hop limit)이란 무엇인가요?
  - IP 주소와 MAC 주소의 차이에 대해 설명하세요.
- 서브넷 마스크와 게이트웨이
  - 서브넷 마스크와, 게이트웨이에 대해 설명하세요.
  - NAT에 대해 설명하세요.
  - 서브넷 마스크의 표현 방식에 대해 설명하세요.
  - 그렇다면, 255.0.255.0 같은 꼴의 서브넷 마스크도 가능한가요?
- DHCP
  - DHCP는 어떤 계층에 속한 프로토콜인가요?
  - DHCP는 어떻게 동작하나요?
  - DHCP에서 UDP를 사용하는 이유는 무엇인가요?
  - DHCP에서, IP 주소 말고 추가로 제공해주는 정보가 있나요?
  - DHCP의 유효기간은 얼마나 되나요?
- 라우터
  - 라우터 내의 포워딩 과정에 대해 설명하세요. 
  - 라우팅과 포워딩의 차이는 무엇인가요?
  - 라우팅 알고리즘에 대해 설명하세요.
  - 포워딩 테이블의 구조에 대해 설명하세요.
- HTTP
  - HTTP는 왜 TCP를 사용하나요?
  - HTTP/1.1과 HTTP/2의 차이점은 무엇인가요?
    - HOL blocking에 대해 설명해 주세요.
  - HTTP/3.0의 주요 특징에 대해 설명해 주세요.
    - 왜 HTTP/3 에서는 UDP를 사용하나요? 위에서 언급한 UDP의 문제가 해결되었나요?  
  - 상태 코드(Status Code)
    - 401 Unauthorized vs 403 Forbidden
    - 200 OK vs 201 Created
    - 필요하다면 우리가 응답코드를 직접 정의해서 사용할 수 있을까요?
  - 메서드(Method)
    - HTTP 메서드의 멱등성에 대해 설명하세요.
    - GET과 POST의 차이에 대해 설명하세요.
    - POST와 PUT, PATCH의 차이에 대해 설명하세요.
    - HTTP 1.1 이후로, GET에도 body에 데이터를 실을 수 있게 되었지만, 왜 아직도 이런 방식을 지양하는 것일까요?
  - Stateless와 connectionless에 대해 설명하세요.
    - 왜 HTTP는 stateless 구조를 채택하고 있을까요?
    - Connectionless의 논리대로면 성능이 좋지 않을 것으로 보이는데, 해결 방법이 있을까요?
    - TCP의 keep-alive와 HTTP의 keep-alive의 차이를 설명하세요.
- HTTPS
  - 공개키와 대칭키의 차이에 대해 설명하세요.
  - HTTP와 HTTPS의 차이점과 HTTP의 문제점들에 대해 설명하세요.
  - 왜 HTTPS handshake 과정에서는 인증서를 사용할까요?
  - SSL과 TLS의 차이에 대해 설명하세요.
  - TLS/SSL handshake에 대해 설명하세요.
- DNS
  - DNS는 어떤 계층에 속한 프로토콜인가요?
  - DNS는 TCP와 UDP 중 어떤 것을 사용하나요?
  - DNS 레코드 타입 중 A, CNAME, AAAA의 차이에 대해서 설명하세요.
  - DNS round robin 방식에 대해 설명하세요.
  - DNS Recursive query, Iterative query가 무엇인가요?
  - DNS 쿼리를 통해 얻어진 IP는 어디를 가리키고 있나요?
  - DNS 쿼리 과정에서 손실이 발생한다면, 어떻게 처리하나요?
  - 캐싱된 DNS 쿼리가 잘못될 수 도 있습니다. 이 경우, 어떻게 에러를 보정할 수 있나요?
  - hosts 파일은 어떤 역할을 하나요? DNS와 비교하였을 때 어떤 것이 우선순위가 더 높나요?
- 쿠키(Cookie)와 세션(Session)
  - 쿠키와 세션의 차이에 대해 설명하세요.
  - 세션 방식의 로그인 과정에 대해 설명하세요.
  - HTTP stateless의 의미를 생각해보면, 세션은 적절하지 않은 인증 방법 아닌가요?
  - 규모가 커져 서버가 여러 개가 된다면, 세션을 어떻게 관리할 수 있을까요?
- 웹소켓과 소켓 통신
  - 웹소켓과 소켓 통신의 차이를 설명하세요.
  - 소켓과 포트의 차이를 설명하세요.
  - 여러 소켓이 있다고 할 때, 그 소켓의 포트 번호는 모두 다른가요?
  - 사용자의 요청이 무수히 많아지면, 소켓도 그에 비례하요 무수히 많이 생성되나요?
- SOP
  - SOP 정책에 대해 설명하세요.
  - CORS 정책이 무엇인가요?
  - Preflight에 대해 설명하세요.
- 로드 밸런싱(Load Balancing)
  - 로드밸런서는 무엇인가요?
  - 로드 밸런싱의 개념과 기술, 그리고 그 구현 방법에 대해 설명하세요.
  - L4 로드밸런서와, L7 로드밸런서의 차이에 대해 설명해 주세요.
  - 로드밸런서 알고리즘에 대해 설명해 주세요.
  - 로드밸런싱 대상이 되는 장치중 일부 장치가 문제가 생겨 접속이 불가능하다고 가정해 봅시다. 이 경우, 로드밸런서가 해당 장비로 요청을 보내지 않도록 하려면 어떻게 해야 할까요?
  - 로드밸런서 장치를 사용하지 않고, DNS를 활용해서 유사하게 로드밸런싱을 하는 방법에 대해 설명하세요.
- XSS와 CSRF
  - XSS에 대해서 설명하세요.
  - CSRF랑 XSS는 어떤 차이가 있나요?
  - XSS는 프론트엔드에서만 막을 수 있나요?

<br>

# 데이터베이스
- 스키마(Schema)
  - 스키마에 대해 설명하세요.
  - 스키마의 3계층에 대해 설명하세요.
- 키(Key)
  - 키(기본키, 후보키, 슈퍼키 등)에 대해 설명하세요.
  - 기본키는 수정이 가능한가요?
  - MySQL의 경우, 기본키를 설정하지 않아도 테이블이 만들어집니다. 어떻게 이게 가능한 걸까요?
  - 외래키 값은 null이 들어올 수 있나요?
  - 어떤 컬럼의 정의에 UNIQUE 키워드가 붙는다고 가정해봅시다. 이 컬럼을 활용한 쿼리의 성능은 그렇지 않은 것과 비교해서 어떻게 다를까요?
- SQL Join
  - DB JOIN이 무엇인지 설명하고, 각 종류에 대해 설명하세요.
  - 사실, JOIN은 상당한 시간이 걸릴 수 있기에 내부적으로 다양한 구현 방식을 사용하고 있습니다. 그 예시에 대해 설명하세요.
  - 그렇다면 입력한 쿼리에서 어떤 구현 방식을 사용하는지는 어떻게 알 수 있나요?
  - 앞 질문들을 통해 인덱스의 중요성을 알 수 있었는데, 그렇다면 JOIN의 성능도 인덱스의 유무의 영향을 받나요?
  - 3중 조인 부터는 동작 방식이 약간 바뀝니다. 어떻게 동작하는지, 그리고 그 방식이 성능에 어떠한 영향을 주는지 설명하세요.
- [정규화(Normalization)](https://velog.io/@stemmmm/%EB%8D%B0%EC%9D%B4%ED%84%B0%EB%B2%A0%EC%9D%B4%EC%8A%A4-%EC%A0%95%EA%B7%9C%ED%99%94)
- 인덱스(Index)
  - 인덱스가 무엇이고, 언제 사용하는지 설명하세요.
  - 인덱스가 사용하는 자료구조에 대해 설명하세요.
    - DB에서 RBT를 사용하지 않고, B-Tree/B+Tree를 사용하는 이유를 설명하세요.
    - B+Tree가 B-Tree에 비해 반드시 좋다고 할 수 있을까요? 그렇지 않다면 어떤 단점이 있을까요?
    - 오름차순으로 정렬된 인덱스에서 내림차순 정렬을 시도할 경우 성능이 어떻게 될까요? B-Tree/B+Tree의 구조를 기반으로 설명하세요.
  - Primary index와 secondary index에 대해 설명하세요.
  - Composite index에 대해 설명하세요.
  - 일반적으로 인덱스는 수정이 잦은 테이블에선 사용하지 않기를 권합니다. 왜 그럴까요?
  - ORDER BY/GROUP BY 연산의 동작 과정을 인덱스의 존재여부와 연관지어서 설명하세요.
  - 기본키는 인덱스라고 할 수 있을까요? 그렇지 않다면, 인덱스와 기본키는 어떤 차이가 있나요?
  - 그렇다면 외래키는 인덱스라고 할 수 있을까요? 그렇지 않다면, 인덱스와 외래키는 어떤 차이가 있나요?
  - 인덱스가 데이터의 물리적 저장에도 영향을 미치나요? 그렇지 않다면, 데이터는 물리적으로 어떤 순서로 저장되나요?
  - NoSQL도 인덱스를 갖고 있나요? 만약 있다면, RDB의 인덱스와는 어떤 차이가 있을까요?
  - (A, B) 와 같은 방식으로 인덱스를 설정한 테이블에서, A 조건 없이 B 조건만 사용하여 쿼리를 요청했습니다. 해당 쿼리는 인덱스를 탈까요?
  - Table full scan, index range ccan에 대해 설명하세요.
    - 가끔은 인덱스를 타는 쿼리임에도 table full scan 방식으로 동작하는 경우가 있습니다. 왜 그럴까요?
  - 개수를 세는 쿼리인 COUNT는 어떻게 동작하나요? COUNT(1), COUNT(*), COUNT(column)의 동작 과정에는 차이가 있나요?
- [트랜잭션(Transaction)](https://easy-code-yo.tistory.com/26)
  - 트랜잭션의 개념과 ACID 원칙에 대해 설명하세요.
  - ACID 원칙 중, DBMS는 durability를 어떻게 보장하나요?
  - 트랜잭션과 lock에 대해 설명하세요.
  - 트랜잭션은 어떤 경우에 사용할 수 있으며, 어떤 점을 주의해야할까요?
  - 읽기에는 트랜잭션을 걸지 않아도 될까요?
  - 트랜잭션 격리 레벨 (Transaction Isolation Level)
    - 트랜잭션 격리 레벨에 대해 설명하세요.
    - 모든 DBMS가 4개의 레벨을 모두 구현하고 있나요? 그렇지 않다면 그 이유는 무엇일까요?
    - 스토리지 엔진은 정확히 무엇을 하는 건가요?
- 뷰(View)
  - 뷰가 무엇이고, 어떤 경우에 사용하나요?
  - 그렇다면, 뷰의 값을 수정해도 실제 테이블에는 반영되지 않나요?
- 저장 프로시저(Stored procedure)
- 동적 SQL
- DB Locking
  - Optimistic lock과 Pessimistic lock에 대해 설명하세요.
  - 물리적으로 lock을 건다면, 만약 이를 수행중인 요청에 문제가 생겨 비정상 종료되면 lock이 절대 해제되지 않는 문제가 생길 수도 있을 것 같습니다. DB는 이를 위한 해결책이 있나요? 없다면, 우리가 이 문제를 해결할 수 없을까요?
- [DB의 Connection Pool](https://youtu.be/zowzVqx3MQ4?si=OyVzd2S22944A_Ix)
  - DB와 클라이언트가 connection을 어떻게 구성하는지 설명하세요.
- NoSQL
  - RDB와 NoSQL의 차이에 대해 설명하세요.
  - NoSQL의 장점과 단점을 설명하세요.
  - NoSQL은 왜 일반적으로 RDB보다 빠를까요?
  - NoSQL을 활용한 경험이 있나요? 있다면, 왜 RDB를 선택하지 않고 해당 DB를 선택했는지 설명하세요.
  - RDBMS, NoSQL에서의 클러스터링/레플리케이션 방식에 대해 설명하세요.
    - 이러한 분산 환경에선, 트랜잭션을 어떻게 관리할 수 있을까요?
    - 마스터, 슬레이브 데이터 동기화 전 까지의 데이터 정합성을 지키는 방법은 무엇이 있을까요?
    - 다중 트랜잭션 상황에서의 deadlock 상황과, 이를 해결하기 위한 방법에 대해 설명하세요.
    - 샤딩 방식은 무엇인가요? 만약 본인이 DB를 분산해서 관리해야 한다면, 레플리케이션 방식과 샤딩 방식 중 어떤 것을 사용할 것 같나요?
- 트래픽이 높아질 때의 DB 관리
  - DB 서버를 분산하지 않고, 트래픽을 감당할 수 있는 방법은 없을까요?
- SQL Injection
  - SQL injection에 대해 설명하세요.
  - 그렇다면, 우리가 서버 개발 과정에서 사용하는 수많은 DB 라이브러리들은 이 문제를 어떻게 해결할까요?

<br>

# 디자인 패턴
- 디자인 패턴의 개념
- 싱글톤 패턴
  - 싱글톤의 장단점에 대해 설명해 주세요.
  - 싱글톤이 하나의 객체만 생성한다는 것을 어떻게 보장할 수 있을까요?
  - Lazy loading과 Holder
- 어댑터 패턴
- 탬플릿 메소드 패턴
- 팩토리 메소드 패턴
- 옵저버 패턴
- 스트레티지 패턴
- 컴포지트 패턴

<br>

# Spring
- [IoC와 DI](https://velog.io/@stemmmm/IoC와-DI)
- Servlet과 JSP
  - 내부 동작 원리를 설명하세요. 
- 빈(Bean)
  - Spring Bean 주입 방법
  - Spring Bean scope
- MVC
  - MVC1 vs MVC2 vs Spring MVC
  - MVC 패턴을 다른 아키텍처 패턴과 비교하며 설명하세요.
- DispatcherServlet
  - DispatcherServlet의 역할에 대해 설명하세요.
  - 여러 요청이 들어온다고 가정할 때, DispatcherServlet은 한번에 여러 요청을 모두 받을 수 있나요?
  - 수많은 @Controller 를 DispatcherServlet은 어떻게 구분할까요?
- Servlet filter vs Interceptor
  - Interceptor와 Servlet filter에 대해 설명하세요.
  - 설명만 들어보면 인터셉터만 쓰는게 나아보이는데, 아닌가요? 필터는 어떤 상황에 사용해야 하나요?
- AOP
  - AOP에 대해 설명하세요. 
  - @Aspect는 어떻게 동작하나요?
- @Transactional
  - @Transactional 은 어떤 기능을 하나요? 
  - @Transactional(readonly=true)는 어떤 기능인가요? 이게 도움이 되나요?
  - 그런데, 읽기에 트랜잭션을 걸 필요가 있나요? @Transactional을 안 붙이면 되는거 아닐까요?
- JPA
  - JPA와 같은 ORM을 사용하는 이유가 무엇인가요?
  - 영속성은 어떤 기능을 하나요? 이게 진짜 성능 향상에 큰 도움이 되나요?
  - N + 1 문제에 대해 설명하세요.
- Tomcat
  - Tomcat은 정확히 어떤 역할을 하는 도구인가요? 
  - 혹시 Netty에 대해 들어보셨나요? 왜 이런 것을 사용할까요?
 
<br>

# 출처
- https://github.com/JaeYeopHan/Interview_Question_for_Beginner
- https://github.com/gyoogle/tech-interview-for-developer
- https://github.com/VSFe/Tech-Interview
