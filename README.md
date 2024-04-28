# CS-Technical-Interview
CS 지식 저장소


(공통)

  <details>
    <summary>1. 동기와 비동기의 차이를 설명 해 주세요.</summary> 
    <br>
    <p>동기는 하나의 작업이 끝날 때까지 다른 작업을 시작하지 않고, 먼저 시작한 작업이 끝나면 새로운 작업을 시작하는 방식입니다. 작업이 직렬로 배치되어 실행되고, 작업 실행의 순서가 정해져 있는 것이 동기 방식입니다.</p>
    <p>비동기는 먼저 시작된 작업의 완료 여부와는 상관없이 새로운 작업을 시작하는 방식입니다. 작업이 병렬로 배치되어 실행되고, 작업의 순서가 확실하지 않아서 나중에 시작된 작업이 먼저 끝나는 경우도 발생합니다. 이와 같은 방식이 비동기 방식입니다.</p>
  </details>

  <details>
    <summary>2. 프레임워크와 라이브러리의 차이를 설명 해 주세요.</summary>
    <br>
    <p>프레임워크와 라이브러리의 주요 차이점은 제어의 흐름에 있습니다.</p>
    <p>프레임워크는 전체적인 프로그램의 흐름을 제어하는 구조나 틀입니다. 프레임워크가 정한 규칙과 구조 안에서 개발자는 필요한 부분을 채워 넣습니다. 예를 들어, 식당에서 메뉴를 선택할 수 있지만, 그 과정은 식당이 정한 흐름에 따릅니다.</p>
    <p>라이브러리는 일련의 함수나 메서드 모음이며, 개발자가 필요할 때 가져와서 사용합니다. 다시 말해, 개발자가 직접 제어합니다. 예를 들어, 책을 읽을 때 원하는 책을 직접 골라서 읽는 것과 같습니다.</p>
    <p>따라서, 라이브러리는 개발자가 선택하여 사용하는 도구이고, 프레임워크는 전체적인 틀과 규칙에 따라 개발을 진행하는 환경입니다.</p>
  </details>

  <details>
    <summary>3. DDD (Domain-Driven Design)에 대해 설명 해 주세요.</summary>
    <br>
    <p>Domain-Driven Design (DDD)은 복잡한 소프트웨어 프로젝트를 처리하기 위한 접근 방식으로, 비즈니스 도메인의 복잡성을 관리하고 반영하는 데 중점을 둡니다. DDD의 핵심은 소프트웨어의 구조와 언어가 그 비즈니스 도메인의 전문 용어와 밀접하게 일치해야 한다는 것입니다. 이 접근 방식을 통해 개발자와 비즈니스 전문가 간의 커뮤니케이션이 개선되고, 소프트웨어의 품질과 유지 보수성이 향상됩니다.

DDD는 크게 네 가지 기본 요소로 구성됩니다:

도메인 모델: 비즈니스 문제를 추상화한 모델로, 도메인의 핵심 개념과 관계를 표현합니다. 이 모델은 개발 과정 전반에 걸쳐 비즈니스 로직의 기반이 됩니다.

유비쿼터스 언어(Ubiquitous Language): 개발자와 비즈니스 전문가가 공유하는, 도메인 모델을 기반으로 한 언어입니다. 이 언어는 커뮤니케이션의 모호함을 줄이고, 모든 이해당사자가 동일한 용어를 사용하도록 보장합니다.

경계 컨텍스트(Bounded Context): 도메인이 서로 다른 모델을 가질 수 있는 명확한 경계를 정의합니다. 각 경계 컨텍스트 내에서는 유니크한 모델과 유비쿼터스 언어가 사용됩니다. 이를 통해 복잡성을 관리하고, 모델 간의 간섭을 최소화합니다.

도메인 로직의 패턴: DDD에서는 엔티티, 값 객체, 서비스, 리포지토리, 애그리게잇 등의 패턴을 사용하여 도메인 로직을 구조화하고 구현합니다. 이 패턴들은 도메인 모델을 효과적으로 설계하고 구현하는 데 도움을 줍니다.

DDD를 통해 개발팀은 비즈니스 요구 사항을 더 잘 이해하고, 유연하며 유지 보수가 용이한 소프트웨어를 개발할 수 있습니다.</p>
  </details>

  <details>
    <summary>4. OSI 7계층에 대해 설명 해 주세요.</summary>
    <br>
    <p>OSI 7계층 모델은 네트워크 통신에서 데이터가 전송되는 과정을 7개의 계층으로 나눈 것입니다. 각 계층은 특정 기능을 담당하며, 데이터가 상위 계층에서 하위 계층으로 내려가면서 필요한 헤더 정보가 추가되고, 받는 쪽에서는 이 과정이 역순으로 이루어지며 헤더를 해석합니다. 이 모델은 네트워크 문제를 진단하고 설계하는 데 유용합니다.

물리 계층(Physical Layer): 실제 전기적, 물리적 신호를 전송하는 계층입니다. 케이블, RJ45, 광섬유 등의 하드웨어가 여기에 해당합니다.

데이터 링크 계층(Data Link Layer): 네트워크에서 두 장치 간의 데이터 전송을 가능하게 하는 계층입니다. 이 계층은 MAC 주소를 사용하여 데이터의 오류 검출 및 재전송을 담당합니다. 이더넷, Wi-Fi가 여기에 속합니다.

네트워크 계층(Network Layer): 다른 네트워크로 데이터를 전송하는 기능을 담당합니다. 이 계층에서는 IP 주소를 사용하여 데이터를 목적지까지 라우팅합니다. 대표적으로 IP가 이에 해당합니다.

전송 계층(Transport Layer): 데이터의 전송을 관리하며, 통신을 위한 포트 번호를 사용합니다. TCP(신뢰성 있는 데이터 전송을 보장)와 UDP(더 빠르지만 신뢰성이 낮은 전송)가 이 계층에 속합니다.

세션 계층(Session Layer): 통신 세션을 관리하며, 데이터 교환의 시작과 끝을 담당합니다. 애플리케이션 간의 세션을 설정, 관리, 종료하는 역할을 합니다.

표현 계층(Presentation Layer): 데이터의 표현 형식(인코딩)을 담당합니다. 데이터 압축, 암호화, 변환 등을 처리하여 애플리케이션이 이해할 수 있는 형태로 변환합니다.

응용 계층(Application Layer): 최종 사용자와 직접적으로 상호작용하는 계층입니다. 웹 브라우저, 이메일 클라이언트 등 사용자가 사용하는 응용 프로그램이 여기에 속합니다.

이 계층적 접근 방식은 문제를 효율적으로 진단하고, 네트워크 기능을 분할하여 관리하기 용이하게 만듭니다.</p>
  </details>

  <details>
    <summary>5. TCP/IP 프로토콜에 대해 설명 해 주세요.</summary>
    <br>
    <p>TCP/IP(Transmission Control Protocol/Internet Protocol)는 인터넷상에서 데이터를 안전하게 전송하기 위한 표준 규약(프로토콜) 집합입니다. 이는 네트워크 통신의 주요 두 가지 기능을 담당합니다.

TCP(Transmission Control Protocol)는 데이터가 목적지에 안정적으로, 순서대로, 에러 없이 도달하도록 보장합니다. 데이터를 여러 패킷으로 나누어 전송하고, 수신측에서는 이를 다시 조립합니다. 전송 중 손실이나 오류가 발견되면, 해당 패킷은 재전송됩니다.

IP(Internet Protocol)는 데이터 패킷을 송신지에서 수신지로 올바르게 전달하기 위한 주소 지정과 라우팅(경로 결정)을 담당합니다. 각 기기는 고유한 IP 주소를 가지고 있어 인터넷 상에서 서로를 식별할 수 있습니다.

TCP/IP 모델은 데이터의 효율적이고 신뢰할 수 있는 전송을 보장하여, 인터넷의 기반이 되는 기술입니다.</p>
  </details>

  <details>
    <summary>6. HTTPS가 동작하는 방식에 대해서 설명 해 주세요.</summary>
    <br>
    <p>HTTPS는 웹 통신의 보안을 강화하기 위해 HTTP에 SSL/TLS 프로토콜을 결합한 것입니다. 이 프로토콜은 데이터의 안전한 전송을 보장하기 위해 데이터 암호화, 서버 인증, 데이터 무결성 보호 기능을 제공합니다. HTTPS의 주요 동작 방식은 다음과 같습니다:

연결 설정: 클라이언트(브라우저)와 서버 간의 연결 초기에 'SSL Handshake' 과정이 진행됩니다. 이 단계에서 클라이언트와 서버는 서로 통신에 사용할 암호화 방식을 협상합니다. 

서버 인증: 클라이언트는 서버로부터 받은 디지털 인증서를 검증하여 서버의 신뢰성을 확인합니다. 인증서에는 서버의 공개 키, 인증서 발급 기관(CA), 유효 기간 등이 포함되어 있습니다. 

키 교환: 서버와 클라이언트는 공개키 암호화를 사용하여 세션 키를 안전하게 교환합니다. 이 세션 키는 이후 세션 동안 데이터를 암호화하는 데 사용됩니다. 

데이터 전송: 세션 키를 사용하여 클라이언트와 서버 간에 전송되는 데이터는 모두 암호화됩니다. 이로써 데이터를 엿보거나 수정하는 중간자 공격으로부터 보호됩니다. 

연결 종료: 통신이 끝나면 세션 키는 폐기되며, 양측은 연결을 안전하게 종료합니다.

HTTPS는 웹 통신에서 중요한 보안 메커니즘을 제공하여 개인정보 보호와 데이터 보안을 강화합니다.


또는


HTTPS의 동작 방식은 크게 세 단계로 설명할 수 있습니다. 첫째, 클라이언트와 서버 사이의 보안 연결을 설정하기 위해 SSL 핸드셰이크 과정이 진행됩니다. 이 과정에서 서버는 자신의 인증서를 클라이언트에게 제공하고, 클라이언트는 이를 검증하여 서버의 신뢰성을 확인합니다. 둘째, 핸드셰이크를 통해 클라이언트와 서버는 데이터 암호화에 사용할 세션 키를 안전하게 교환합니다. 마지막으로, 이 세션 키를 사용하여 데이터를 암호화하고 전송함으로써 중간자 공격으로부터 정보를 보호합니다.</p>
  </details>

  <details>
    <summary>7. CORS란 무엇인가요?</summary>
    <br>
    <p></p>
  </details>

  <details>
    <summary>8. REST API란 무엇인지 설명 해 주세요.</summary>
    <br>
    <p></p>
  </details>

  <details>
    <summary>9. 프로세스와 스레드의 차이는 무엇인가요?</summary>
    <br>
    <p></p>
  </details>

  <details>
    <summary>10. 멀티 스레드는 무엇인가요?</summary>
    <br>
    <p></p>
  </details>

  <details>
    <summary>11. 관계형 DB와 비관계형 DB의 차이는 무엇인가요?</summary>
    <br>
    <p></p>
  </details>

  <details>
    <summary>12. 대용량 트래픽 발생 시 어떻게 대응해야 하나요?</summary>
    <br>
    <p></p>
  </details>

  <details>
    <summary>13. ORM을 사용하면서 쿼리가 복잡해지는 경우에는 어떻게 해결하는게 좋을까요?</summary>
    <br>
    <p></p>
  </details>

  <details>
    <summary>14. JWT, Refresh, Access Token에 대해서 설명해주세요.?</summary>
    <br>
    <p></p>
  </details>

  <details>
    <summary>15. OAuth에 대해서 설명해주세요.</summary>
    <br>
    <p></p>
  </details>

  <details>
    <summary>16. CI/CD에 대해서 설명해주세요.</summary>
    <br>
    <p></p>
  </details>

  <details>
    <summary>17. 프로세스와 쓰레드에 대해서 설명하고 그 차이에 대해서 설명해주세요.</summary>
    <br>
    <p></p>
  </details>

  <details>
    <summary>18. 쿼리 최적화에 대해 설명해주시고 방법에 대해 설명해주세요.</summary>
    <br>
    <p></p>
  </details>

  <details>
    <summary>19. DB 로직 최소화를 하려면 어떻게 해야 할까요?</summary>
    <br>
    <p></p>
  </details>

  <details>
    <summary>20. 테스트코드에 대해서 아는대로 설명해주시고 활용 경험에 대해서 답변해주세요.</summary>
    <br>
    <p></p>
  </details>

  <details>
    <summary>21. AWS S3, EC2를 사용하는 이유와 사용 경험에 대해서 답변해주세요.</summary>
    <br>
    <p></p>
  </details>

  <details>
    <summary>22. Array, LinkedList에 대해 설명해주시고 각각 어떻게 사용하는지 말씀해주세요.</summary>
    <br>
    <p></p>
  </details>

  <details>
    <summary>23. 정렬 알고리즘에 대해서 아는대로 설명해주세요.</summary>
    <br>
    <p></p>
  </details>

  <details>
    <summary>24. CI/CD를 적용해 본 적이 있나요? 있다면 경험을 공유 해 주세요.</summary>
    <br>
    <p></p>
  </details>

  <details>
    <summary>25. 도커를 활용한 경험이 있나요? 도커가 무엇인지, 경험이 있다면 공유 해 주세요.</summary>
    <br>
    <p></p>
  </details>

  <details>
    <summary>26. 인덱스란 무엇이고 일반적인 원리는 어떤지 설명해주세요.</summary>
    <br>
    <p></p>
  </details>

  <details>
    <summary>27. 모든 요소에 인덱스를 걸지 않는 이유는 무엇일까요?</summary>
    <br>
    <p></p>
  </details>

  <details>
    <summary>28. Call by reference란 무엇이고 보통 어떻게 쓰이나요?</summary>
    <br>
    <p></p>
  </details>

  <details>
    <summary>29. 정규화란 무엇이고 대표적인 장점과 단점은 무엇이 있을까요?</summary>
    <br>
    <p></p>
  </details>

  <details>
    <summary>30. 동시성과 병렬성을 비교하여 설명해주세요.</summary>
    <br>
    <p></p>
  </details>

  <details>
    <summary>31. 리팩토링에 대해 아는만큼 설명해주세요.</summary>
    <br>
    <p></p>
  </details>

  <details>
    <summary>32. 절차지향 프로그래밍과 객체지향 프로그래밍을 비교하여 각각의 특징에 대해 설명해주세요.</summary>
    <br>
    <p></p>
  </details>

  <details>
    <summary>33. 메모리 구조에 대해 설명해주세요.</summary>
    <br>
    <p></p>
  </details>

  <details>
    <summary>34. 아스키코드와 유니코드, 그리고 EUC-KR과 UTF-8의 차이점에 대해 설명해주세요.</summary>
    <br>
    <p></p>
  </details>

  <details>
    <summary>35. 메세지 큐(Message Queue)에 대해 설명해주세요.</summary>
    <br>
    <p></p>
  </details>

  <details>
    <summary>36. TDD(Test Driven Development)에 대해 설명해주세요.</summary>
    <br>
    <p></p>
  </details>

  <details>
    <summary>37. OOP의 5가지 설계 원칙에 대해 설명해주세요.</summary>
    <br>
    <p></p>
  </details>

  <details>
    <summary>38. 함수형 프로그래밍에 대해 설명해주세요.</summary>
    <br>
    <p></p>
  </details>

  <details>
    <summary>39. SQL Injection에 대해 설명해주세요.</summary>
    <br>
    <p></p>
  </details>

  <details>
    <summary>40. Docker(도커)의 장점과 단점을 설명해주세요.</summary>
    <br>
    <p></p>
  </details>

  <details>
    <summary>41. MSA에 대해 설명해주세요.</summary>
    <br>
    <p></p>
  </details>

  <details>
    <summary>42. OOP에 대해 설명해주세요.</summary>
    <br>
    <p></p>
  </details>

  <details>
    <summary>43. RESTful API에 대해 설명해주세요.</summary>
    <br>
    <p></p>
  </details>

  <details>
    <summary>44. Call By Value와 Call By Reference 차이를 설명해주세요.</summary>
    <br>
    <p></p>
  </details>

  <details>
    <summary>45. Docker(도커)와 Kubernates(쿠버네티스)에 대해 설명해주세요.</summary>
    <br>
    <p></p>
  </details>

  <details>
    <summary>46. 자료구조와 알고리즘에 대해 설명해주세요.</summary>
    <br>
    <p></p>
  </details>

  <details>
    <summary>47. 해시 테이블과 해시 테이블의 시간 복잡도에 대해 설명해주세요.</summary>
    <br>
    <p></p>
  </details>

  <details>
    <summary>48. AVL 트리에 대해 설명해주세요.</summary>
    <br>
    <p></p>
  </details>

  <details>
    <summary>49. 스택, 큐, 트리, 힙 구조에 대해 설명해주세요.</summary>
    <br>
    <p></p>
  </details>

  <details>
    <summary>50. LinkedList와 ArrayList의 차이점을 설명해주세요.</summary>
    <br>
    <p></p>
  </details>

  <details>
    <summary>51. 레드블랙 트리에 대해 설명해주세요.</summary>
    <br>
    <p></p>
  </details>

  <details>
    <summary>52. 우선순위 큐와 내부 구조 및 시간복잡도에 대해 설명해주세요.</summary>
    <br>
    <p></p>
  </details>

  <details>
    <summary>53. 큐와 스택의 구현에 대해 설명해주세요.</summary>
    <br>
    <p></p>
  </details>

  <details>
    <summary>54. 버블소트에 대해 설명해주세요.</summary>
    <br>
    <p></p>
  </details>

  <details>
    <summary>55. 힙소트에 대해 설명해주세요.</summary>
    <br>
    <p></p>
  </details>

  <details>
    <summary>56. 머지소트에 대해 설명해주세요.</summary>
    <br>
    <p></p>
  </details>

  <details>
    <summary>57. 퀵소트에 대해 설명해주세요.</summary>
    <br>
    <p></p>
  </details>

  <details>
    <summary>58. 삽입소트에 대해 설명해주세요.</summary>
    <br>
    <p></p>
  </details>

  <details>
    <summary>59. 동적 프로그래밍(Dynamic Programming)의 두 가지 조건을 설명해주세요.</summary>
    <br>
    <p></p>
  </details>

  <details>
    <summary>60. 재귀 알고리즘과 재귀의 시간 복잡도를 설명해주세요.</summary>
    <br>
    <p></p>
  </details>

  <details>
    <summary>61. 동적 프로그래밍(Dynamic Programming)에 대해 설명해주세요.</summary>
    <br>
    <p></p>
  </details>

  <details>
    <summary>62. TCP와 UDP의 차이에 대해 설명해주세요.</summary>
    <br>
    <p></p>
  </details>

  <details>
    <summary>63. 웹 접근성의 국제표준에 대해 설명해주세요.</summary>
    <br>
    <p></p>
  </details>

  <details>
    <summary>64. HTTP와 HTTPS를 비교하여 설명해주세요.</summary>
    <br>
    <p></p>
  </details>

  <details>
    <summary>65. TCP와 HTTP의 차이점을 설명해주세요.</summary>
    <br>
    <p></p>
  </details>

  <details>
    <summary>66. 공인 IP와 사설 IP의 차이점을 설명해주세요.</summary>
    <br>
    <p></p>
  </details>

  <details>
    <summary>67. HTTP 프로토콜에 대해 설명해주세요.</summary>
    <br>
    <p></p>
  </details>

  <details>
    <summary>68. HTTP1과 HTTP2를 비교하여 설명해주세요.</summary>
    <br>
    <p></p>
  </details>

  <details>
    <summary>69. 웹 동작 방식에 대해 설명해주세요.</summary>
    <br>
    <p></p>
  </details>

  <details>
    <summary>70. GET과 POST의 차이를 설명해주세요.</summary>
    <br>
    <p></p>
  </details>

  <details>
    <summary>71. 3 Way-Handshake에 대해 설명해주세요.</summary>
    <br>
    <p></p>
  </details>

  <details>
    <summary>72. 컨텍스트 스위칭(Context Switching)에 대해 설명해주세요.</summary>
    <br>
    <p></p>
  </details>

  <details>
    <summary>73. 레이스 컨디션과 그것으로 인해 발생할 수 있는 문제들은 뭐가 있나요?</summary>
    <br>
    <p></p>
  </details>

  <details>
    <summary>74. 세마포어(Semaphore)와 뮤텍스(Mutex)의 차이점을 설명해주세요.</summary>
    <br>
    <p></p>
  </details>

  <details>
    <summary>75. 페이지 폴트에 대해 설명해주세요.</summary>
    <br>
    <p></p>
  </details>

  <details>
    <summary>76. 멀티 프로세스와 멀티 쓰레드를 비교하여 설명해주세요.</summary>
    <br>
    <p></p>
  </details>

  <details>
    <summary>77. 멀티 쓰레드 프로그래밍 작성 시 유의점을 설명해주세요.</summary>
    <br>
    <p></p>
  </details>

  <details>
    <summary>78. 가상메모리에 대해 설명해주세요.</summary>
    <br>
    <p></p>
  </details>

  <details>
    <summary>79. 운영체제의 스케쥴러에 대해 설명해주세요.</summary>
    <br>
    <p></p>
  </details>

  <details>
    <summary>80. Byte Ordering에 대해 설명해주세요.</summary>
    <br>
    <p></p>
  </details>

  <details>
    <summary>81. 데드락(DeadLock)과 임계 영역(Critical Section)에 대해 설명해주세요.</summary>
    <br>
    <p></p>
  </details>

  <details>
    <summary>82. CPU의 메모리 I/O 도중 생기는 병목 현상 해결 방법에 대해 설명해주세요.</summary>
    <br>
    <p></p>
  </details>

  <details>
    <summary>83. 페이지 교체 알고리즘과 LRU(Least Recently Used)에 대해 설명해주세요.</summary>
    <br>
    <p></p>
  </details>

  <details>
    <summary>84. DB 정규화에 대해 설명해주세요.</summary>
    <br>
    <p></p>
  </details>

  <details>
    <summary>85. 커넥션 풀을 사용하는 이유와 장점 그리고 주의점을 설명해주세요.</summary>
    <br>
    <p></p>
  </details>

  <details>
    <summary>86. 클러스터링과 리플리케이션에 대해 설명해주세요.</summary>
    <br>
    <p></p>
  </details>

  <details>
    <summary>87. 인덱스의 자료구조에 대해 설명해주세요.</summary>
    <br>
    <p></p>
  </details>

  <details>
    <summary>88. 트랜잭션의 ACID에 대해 설명해주세요.</summary>
    <br>
    <p></p>
  </details>

  <details>
    <summary>89. DB 락의 종류에 대해 설명해주세요.</summary>
    <br>
    <p></p>
  </details>

  <details>
    <summary>90. 힌트(Hint)에 대해 설명해주세요.</summary>
    <br>
    <p></p>
  </details>

  <details>
    <summary>91. 트랜잭션(Transaction)에 대해 설명해주세요.</summary>
    <br>
    <p></p>
  </details>

  <details>
    <summary>92. 낙관적 동시성 제어와 비관적 동시성 제어에 대해 비교하여 설명해주세요.</summary>
    <br>
    <p></p>
  </details>
