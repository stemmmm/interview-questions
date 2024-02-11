# 목차
- [Java](#Java)
- [프로그래밍 일반](#프로그래밍-일반)
- [컴퓨터구조](#컴퓨터구조)
- [자료구조](#자료구조)
- [알고리즘](#자료구조)
- [네트워크](#네트워크)
- [데이터베이스](#데이터베이스)
- [디자인패턴](#디자인패턴)
- [Spring](#Spring)

<br>

# Java
- 자바의 컴파일 과정에 대해 설명하세요.
- 자바 가상 머신 (Java Virtual Machine, JVM)
  - 자바 가상 머신(JVM)의 역할과 기능에 대해 설명하세요.  
  - 자바 말고 다른 언어는 JVM 위에 올릴 수 없나요?
  - 반대로 JVM 계열 언어를 일반적으로 컴파일해서 사용할 순 없나요?
  - VM을 사용함으로써 얻을 수 있는 장점과 단점
  - JVM과 내부에서 실행되고 있는 프로세스는 부모 - 자식 관계를 갖고 있다고 봐도 무방한가요?
- 가비지 콜렉션 (Garbage Collection, GC)
  - GC의 원리와 장단점에 대해 설명하세요.  
  - 자바에서는 GC를 어떤 방식으로 구현했나요?
  - GC는 어떤 데이터 영역을 관리하나요?
  - `finalize()`를 수동으로 호출하는 것은 왜 문제가 될 수 있을까요?
  - 어떤 변수의 값이 `null`이 되었다면, 이 변수는 GC가 될 가능성이 있을까요?
  - Reference counting 방식과 이 알고리즘에서 발생할 수 있는 순환 참조(retain cycle)에 대해 설명하세요.
- 기본 타입(Primitive type)과 참조 타입(Reference type)에 대해 설명하세요.
- Call by value vs Call by reference
  - 각각의 개념과 그 차이에 대해 설명하세요.
  - 과연 모든 언어에 이 개념이 존재할까요?
- `equals()`와 `hashcode()`
  - 각각의 메서드가 어떤 역할을 하는지, 그리고 두 메서드의 관계에 대해 설명하세요.
  - `hashcode()`를 직접 정의해야 한다면, 어떤 점을 염두에 두고 구현 하실건가요?
  - `equals()`를 재정의 해야 할 때, 어떤 점을 염두에 두어야 하는지 설명해 주세요.
- `String` vs `StringBuffer` vs `StringBuilder`
  - 각각의 개념과 그 차이에 대해 설명하세요.
  - Interend String에 대해 설명하세요.
- 업캐스팅과 다운캐스팅에 대해 설명하세요.
- 오토박싱과 오토언박싱에 대해 설명하세요.
- `static`
  - 컴파일 과정에서 `static` 키워드가 붙은 변수나 함수는 어떻게 처리되나요?
  - `static`을 사용하면 어떤 이점이 있고, 어떤 제약이 있나요?
  - `static`과 `static final`은 어떤 차이가 있나요?
  - `final`과 `static final`은 어떤 차이가 있나요?
  - static 클래스와 static 메서드를 비교하세요.
- `final`
  - `final` 키워드를 사용하면, 어떤 이점이 있나요?
  - 그렇다면 컴파일 과정에서, `final` 키워드는 다르게 취급되나요?
- 래퍼(Wrapper) 클래스의 역할과 사용법에 대해 설명하세요.
- 접근 제어자(Access modifier)에 대해 설명하세요.
- 예외 처리
  - `Exception`에 대해 설명해 주세요.
  - 예외를 처리하는 세 가지 방법에 대해 설명해 주세요.
  - `CheckedException`, `UncheckedException`의 차이에 대해 설명해 주세요.
  - 예외 처리가 성능에 큰 영향을 미치나요? 만약 그렇다면, 어떻게 하면 부하를 줄일 수 있을까요?
- Collection 프레임워크에 속한 자료구조들의 종류와 사용법에 대해 설명하세요.
- 쓰레드 (Thread)
  - `Thread`의 활용 방법과 주의점에 대해 설명하세요. 
  - `ThreadLocal`에 대해 설명해 주세요. 
- `synchronized`
  - `synchronized` 키워드의 역할과 사용법에 대해 설명하세요.
  - `synchronized` 키워드가 어디에 붙는지에 따라 의미가 약간씩 변화하는데, 각각 어떤 의미를 갖게 되는지 설명하세요.
  - 효율적인 코드 작성 측면에서, `synchronized`는 좋은 키워드일까요?
  - `synchronized`를 대체할 수 있는 자바의 다른 동기화 기법에 대해 설명하세요.
- Stream API와 람다식
  - Stream API의 개념과 활용법에 대해 설명하세요.
  - 람다식의 개념과 사용법에 대해 설명하세요.
  - Stream과 for문의 성능을 비교하세요.
  - Stream을 병렬처리 할 수 있나요?
  - Stream에서 사용할 수 있는 함수형 인터페이스에 대해 설명해 주세요.
  - 가끔 외부 변수를 사용할 때, `final` 키워드를 붙여서 사용하는데 왜 그럴까요? 꼭 그래야 할까요?
- 직렬화(Serialization)란 무엇인가요?
- 리플렉션 (Reflection)
    - 리플렉션의 개념과 사용법에 대해 설명하세요.
    - 의미만 들어보면 리플렉션은 보안적인 문제가 있을 가능성이 있어보이는데, 실제로 그렇게 생각하시나요? 만약 그렇다면, 어떻게 방지할 수 있을까요?
    - 리플렉션을 언제 활용할 수 있을까요?
- 어노테이션 (Annotation)
  - 자바에서 어노테이션은 어떤 기능을 하나요?
  - 별 기능이 없는 것 같은데, 어떻게 Spring에서는 어노테이션이 그렇게 많은 기능을 하는 걸까요?
  - Lombok의 @Data를 잘 사용하지 않는 이유는 무엇일까요?
- 제네릭(Generic)의 개념과 사용법에 대해 설명하세요.
- 레코드(Record)란 무엇인가요?

<br>

# 프로그래밍 일반
- 객체 지향 프로그래밍 (Object-Oriented Programming, OOP)
  - SOLID에 대해 설명하세요.
  - Composition의 개념과 활용 방법에 대해 설명하세요.
  - 인터페이스와 추상 클래스의 차이에 대해 설명하세요.
    - 왜 클래스는 단일 상속만 가능한데, 인터페이스는 2개 이상 구현이 가능할까요?
- 함수형 프로그래밍 (Functional Programming)
  - 순수 함수와 함수형 프로그래밍 매커니즘의 연관성에 대해 설명하세요.
  - Side-effect가 무엇인가요? 이를 모두 없애는 프로그래밍이 이상적이라고 할 수 있을까요?
  - 왜 함수형 프로그래밍 매커니즘을 사용할까요?
  - 순수 함수는 thread-safe 한가요? 그렇다면 왜 그럴까요?
  - 고차 함수에 대해 설명하세요.
- 프레임워크와 라이브러리의 차이에 대해 설명하세요.
- RESTful API에 대해 설명하세요.
- TDD(Test Driven Development)는 무엇이며, 어떤 장점이 있나요?
- 애자일(Agile) 개발에 대해 설명하세요.
- 데브옵스(DevOps)란 무엇인가요?
- Git과 GitHub에 대해 설명하세요.
- 가상화와 가상 머신
  - 가상화와 가상 머신의 차이를 설명하세요.
  - 그렇다면 도커(Docker)는 둘 중 어디에 속하나요? 왜 사람들이 도커를 많이 채택할까요?
  - 하나의 Host OS에서 돌아간다면, 한 컨테이너가 다른 컨테이너에 간섭할 수 있는 위험이 있지 않을까요? 이를 어떻게 방어할 수 있을까요?
  - 도커 위에 도커를 올릴 순 없을까요?
- 인증과 인가의 차이에 대해 설명하세요.
  - OAuth에 대해 설명하세요.
- JWT (JSON Web Token)
  - JWT 인증 방식에 대해 설명하세요.
  - Signature는 어떻게 만들어지나요?
  - 만약 access token이 탈취되면, 어떻게 대응해야 할까요?
  - 반대로 Refresh Token이 탈취되면, 어떻게 대응해야 할까요?
- 문자열 인코딩인 base64 인코딩과, 이를 사용하는 이유에 대해 설명하세요.

<br>

# 컴퓨터구조
- 폰 노이만 구조에 대해 설명하세요.
- 컴퓨터의 구성 요소에 대해 설명하세요.
- 중앙 처리 장치 (CPU)
  - 32비트와 64비트 컴퓨터의 차이는 무엇인가요?
  - 32비트와 64비트 컴퓨터에서 사용할 수 있는 메모리의 최대 크기는 얼마인가요? 왜 그런건가요?
  - CPU의 작동 원리에 대해 설명하세요.
- 캐시 메모리에 대해 설명하세요.
- 고정 소수점 표현 방식과 부동 소수점 표현 방식에 대해 설명하세요.
- 패리티 비트와 해밍 코드에 대해 설명하세요.

<br>


# 자료구조
- 시간 복잡도와 공간 복잡도
  - Big-O, Big-Theta, Big-Omega 표기법에 대해 설명하세요.
  - 다른 표기법 사용하지 않고, Big-O를 사용하는 이유가 있을까요?
  - O(1)은 O(n^2)보다 무조건 빠른가요?
- 배열(Array)에 대해 설명하세요.
- ArrayList에 대해 설명하고, 배열과 비교하세요.
- 연결 리스트 (Linked List)
  - 연결 리스트를 배열과 비교하며 설명하세요.
  - 연결 리스트를 사용해서 구현할 수 있는 다른 자료구조에 대해 설명하세요.
- 스택(Stack)과 큐(Queue)
  - 스택과 큐의 개념과 주요 연산에 대해 설명하세요.
  - 스택 2개로 큐를 만드는 방법과 그 시간 복잡도를 설명하세요.
  - 큐 2개로을 스택을 만드는 방법과 그 시간 복잡도를 설명하세요.
  - 시간 복잡도를 유지하면서, 배열로 스택과 큐를 구현할 수 있을까요?
  - Prefix, infix, postfix 표기법에 대해 설명하고, 이를 스택을 활용하여 계산하는 방법에 대해 설명하세요.
  - 덱(Deque)은 어떻게 구현할 수 있을까요?
- 그래프 (Graph)
  - 그래프의 개념과 2가지 구현법에 대해 설명하세요.
  - 각 방법에 대해, 두 정점이 연결되었는지 확인하는 시간 복잡도와 한 정점에 연결된 모든 정점을 찾는 시간 복잡도를 비교하세요. 추가로, 공간 복잡도를 비교하세요.
  - 정점의 개수가 n개, 간선의 개수가 n^3개인 그래프는 어떤 방식으로 구현하는 것이 효율적일까요?
  - 탐색
    - 그래프에서 최단거리를 구하는 방법에 대해 설명해 주세요.
    - 정점의 개수가 n개, 간선의 개수가 n^3 개라면, 어떤 알고리즘으로 그래프를 탐색하는 것이 효율적일까요?
- 트리 (Tree)
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
- Heap
  - 힙을 배열로 구현한다고 가정하면, 어떻게 값을 저장할 수 있을까요?
  - 힙의 삽입, 삭제 방식에 대해 설명하고, 왜 이진 탐색 트리와 달리 편향이 발생하지 않는지 설명하세요.
  - 힙 정렬의 시간 복잡도는 어떻게 되나요? Stable한가요?
- Hash
  - 값이 주어졌을 때, 어떻게 하면 충돌이 최대한 적은 해시 함수를 설계할 수 있을까요?
  - 해시 값이 충돌했을 때, 어떤 방식으로 처리할 수 있을까요?
  - 본인이 사용하는 언어에서는, 어떤 방식으로 해시 충돌을 처리하나요?
  - Double hashing 의 장점과 단점에 대해서 설명하고, 단점을 어떻게 해결할 수 있을지 설명하세요.
  - Load factor에 대해 설명하세요. 본인이 사용하는 언어에서의 해시 자료구조는 load factor에 관련한 정책이 어떻게 구성되어 있나요?
  - 다른 자료구조와 비교하여, 해시 테이블은 멀티스레드 환경에서 심각한 수준의 race condition 문제에 빠질 위험이 있습니다. 성능 감소를 최소화 한 채로 해당 문제를 해결할 수 있는 방법을 설명하세요.
- Trie
  - 문자열을 저장하고, 처리하는 주요 자료구조 및 알고리즘 (Trie, KMP, Rabin Karp 등) 에 대해 설명하세요.
- Thread-safe한 자료구조가 있을까요? 없다면, 어떻게 thread-safe한 자료구조를 만들 수 있을까요?
  - 배열의 길이를 알고 있다면, 조금 더 빠른 Thread Safe 한 연산을 만들 순 없을까요?
  - 사용하고 있는 언어의 자료구조는 Thread Safe 한가요? 그렇지 않다면, Thread Safe 한 Wrapped Data Structure 를 제공하고 있나요?
 
<br>

# 알고리즘
- DFS와 BFS에 대해 설명하세요.
- 재귀 (Recursion)
  - 재귀 함수의 동작 과정을 콜 스택과 함께 설명하세요.
  - 언어의 스펙에 따라, 재귀 함수의 최적화를 진행해주는 경우가 있습니다. 어떤 경우에 재귀함수의 최적화가 가능하며, 그 원리를 설명해주세요.
- 정렬 (Sort)
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
- 동적 계획법 (Dynamic Programming)
  - 그리디 알고리즘과 동적 계획법을 비교하고, 어떤 경우에 각각의 기법을 사용하는지 설명하세요.
  - 동적 계획법으로 풀 수 있는 모든 문제는 재귀로 변환하여 풀 수 있나요?
- 이진 탐색 (Binary Search)
  - Lower bound와 Upper bound 는 무엇이고, 이를 어떻게 구현할 수 있을까요?
  - 이진 탐색의 논리를 적용하여 삼진 탐색을 작성한다고 가정한다면, 시간 복잡도는 어떻게 달라질까요? (실제 존재하는 삼진탐색 알고리즘 무시하세요)
  - 기존 이진 탐색 로직에서 부등호의 범위가 바뀐다면, (e.g. <=를 <로) 결과가 달라질까요? 달라진다면 어떻게 달라질까요?
- 비트마스크(BitMask)에 대해 설명하세요.

<br>

# 출처
- https://github.com/JaeYeopHan/Interview_Question_for_Beginner
- https://github.com/gyoogle/tech-interview-for-developer
- https://github.com/VSFe/Tech-Interview
