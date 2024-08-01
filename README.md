```
<h3>네트워크(NetWork)</h3>
Network 는 무엇이며 무엇을 목적으로 하는가?<br>
net = 망 work = 일하다  - > 컴퓨터와 컴퓨터사이를 연결하는 것
네트워크를 통해 우리는 데이터를 송수신 한다.

네트워크 구조
망사형 : 모든 컴퓨터 장치 연결
스타형 : 모든 컴퓨터가 중앙 허브에 1:1로 연결
트리형(계층형) : 계층적으로 연결
링형(루프형) : 인접한 컴퓨터 끼리 연결
버스형 : 하나의 통신회선에 여러대의 컴퓨터 연결


Network 의 종류는 크게 ooo/ooo 로 나눌 수 있다
근거리 통신망 LAN : 건물범위
광역 통신망 : WAN 지역-지역,국가-국가 연결
++)도시 통신망 : MAN :건물,도시 범위
LAN
비교적 근거리에 위치한 통신망을 연결하는 것
WAN
도시,국가,국제적으로 통신망을 연결하는 것(광역 통신망)
ISP업체 보유한 망(KT)
안정성에 중점

InterNet 이란?
인터넷의 인터라는 의미는 연결을 의미하는데 여러개의 네트워크를 묶다라고 의미를 가지고 있다

프로토콜은 무엇인가?
프로토콜은 서로간의 통신의 규칙이 있는데 한사람이 다른 한국어를 쓰고 다른 한명이 영어롤 쓰면 프로토콜이 다르다고 말할수 있다.
통신을 위해 사전에 약속한 규칙/규약
문법/의미/순서
TCP/IP: 인터넷에서 가장 중요한 프로토콜로 사용되며,인터넷의 기본적인 원리를 구성합니다. TCP는 신뢰성 있는 데이터
전송을 위한 프로토콜이고,IP는 데이터의 송수신을 위한 주소 지정 및 라우팅을 담당합니다.
HTTP:웹 브라우저와 웹 서버 간의 통신을 위한 프로토콜로,웹 페이지의 요청과 응답을 처리합니다.
FTP: 파일 전송을 위한 프로토콜로, 파일의 업로드와 다운로드를 지원합니다.
SMTP: 이메일전송을 위한 프로토콜로, 이메일의 발송과 수신에 사용됩니다.

네트워킹 모델의 목적은 무엇인가?
호환성(제조사/국가가 다른 통신장치간의 통신목적)
네트워크망 제작시 사용되는 지침서
네트워크망 이상발생시 문제해결에 사용되는 용도

TCP/IP 모델과 OSI 7 모델의 계층을 적고 각 계층별 역할을 적으세요
4 전송               : 송수신지간(End to End)의 데이터의 신뢰성 확보 
3 네트워크          경로탐새
2 데이터링크      : 장치간의(Point to Point) 데이터의 운송방식 결정
1 물리               : 장치의 물지거 연결/ 디지털 신호 전달

--------------------------------------------------------------------------
<h3>Layer 물리계층</h4>
물리계층 하는일/역할/관련 장치는?
네트워크의 가장 기초적인 계층인 물리계층은 OSI 모델에서 첫 번째 계층으로, 
데이터 통신의 물리적 전송을 담당합니다. 
관련장치는 케이블,허브,리피터
하는일 : 물리적 연결
역할 : 전기적 신호(디지털 신호)
정치 : 허브,리피터,케이블

Cable 이란
전기를 이용해서 신호를 보내는 것.

LAN Cable 종류
UTP FTP STP

부호(Code) 란?
의미를 가지는 약속된 기호

신호(Signal)이란?
  부호가 특정 매개체를 이용해서 전달되어지는 상태

신호전달에 필요한 요소?
전기에너지
통신망

리피터란?
신호증폭기

허브란
집선장치

----------------------------------------------------------------------

<h3>Layer 데이터링크</h3>
OSI 모델중 2계층 모델이 하는 역할에 대해서 설명하세요
  하는일 : 장치간 운송방식 지정
  역할 : 장시간 데이터의 신뢰성 확보(Ethernet / Hdic)
   장치 : L2 Switch

데이터 링크의 목적달성을 위한 필요 요소 3가지는 무엇인가요
   장치 식별 , 오류제어, 흐름제어

LAN/WAN 의 대표 2계층 프로토콜의 명칭은 무엇인가요l
   LAN : Ethernet
   WAN : Hdlc , ppp ,Frame - relay, Atm
  

초기 이더넷 프로토콜의 문제점은 무엇인가요
통신량이 많아지면 충돌영역이 발생

초기 이더넷 프로토콜이 사용하는 통신방법은 어떤것인가요
CSMA/CD 방식 사용

초기 이더넷 프로토콜의 문제점을 해결하기 위한 장치는
L2 Switch

-------------------------------------------------------------------
<h3>Layer 네트워크 계층</h3>
OSI 모델중 3계층 모델이 하는 역할은 무엇인가요 
  경로 탐색

3계층 관련 장치는 무엇인가요
  라우터

3계층 관련 프로토콜 종류는 어떤게 있나요
   Ip, ICMP, ARP, Routing Protocol(RIP,EIGRP,OSPF)

 ICMP 의 용도는?
 ip에 필요한 기타 기능을 수행하가위해 사용
  통신가능여부 확인

IP 의 용도는?
  인터넷에서 사용되는 기본 주소 체계
   인터넷 환경에서 사용되는 구조

Routing 프로토콜의 용도는
최적 경로탐색에 사용


-----------------------------------------------------------------
<h3>Layer 전송계층</h3>
OSI 모델중 4계층 모델이 하는 역할에 대해서 서술하세요 
  종단간의 데이터의 신뢰성을 보장

4 계층 관련 프로토콜은 어떤게 있고 각각 특징을 서술하세요
  TCP  : 연결지향성         신뢰도 높음      속도 느림
  UDP :  비연결지향성      신뢰도 낲음      속도 빠름 



```
-------------------------------------------------------------------------------

```
ROUTING PROTOCOL      정적 Routing - > Static

                                                           Default
                      동적 Routing

                                    IGP --> Distance Vector   RIPv2
                                         |
                               AS       --> Link-State OSPF            

                                    EGP
ROUTE : 길/경로
ROUTER : 경로안내장치
ROUTING : 길 안내작업

AS(Autonomous System) : 자치 시스템, 관리자가 관리하는 라우터의 집합(집단)
IGP(Interior Gateway Protocol)
EGP(Exterior Gateway Protocol)

DISTANCE VERTOR :
전체경로학스 -> 최적경로계산










경로를 안내해주기위해서 사용되는 프로토콜

DNS SERVICE/ SYSTEM / SERVER

Domain Name Service/System/Server
Domain : 영역
Name : 이름
Service : - 제공하다


WEB SERVICE
하이퍼텍스트 형식의 문서파일을 제공해주는 서비스
```



