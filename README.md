
네트워크(NetWork)
----
```
Network 는 무엇이며 무엇을 목적으로 하는가?
net = 망 work = 일하다  - > 컴퓨터와 컴퓨터사이를 연결하는 것
네트워크를 통해 우리는 데이터를 송수신 한다.
```
*네트워크 연결형태*
![3](https://github.com/user-attachments/assets/b158b4e1-6389-4ae1-83e4-2267c6e5385a)
```
RING형 : 각 링크가 단방향이어서 데이터는 한뱡으로만 전송
         각 노드는 데이터의 송수신을 제어하는 액세스 제어논리를 보유

STAR형 : 중앙집중식 구조
         중앙의 교환장비가 데이터 경로를 개설하고 유도
         이용자의 스테이션은 중앙의 교환장비에 point - to - point 링크로 연결

TREE형 : 지역과 거리에 따라 연결하므로 통신선로의 총경로가 가장 짧음
         접속되는 단말기의 숫자에 맞는 통신장비 이용이 가능

MESH형 : 네트워크상의 모든 노드를 상호 연결
         통신선로의 총길이가 가장 긴 네트워크 구조
         초기 데이타 통신 네트워크의 전형적인 형태
         공중통신망에 많이 사용

BUS형 : 어떠한 통신망에서 선을 따 통신선으로 끌어다가 쓰는 방식이다. 멀티탭의 원리와 동일하다고 보면 된다.
        필요할때마다 선을 끌어쓰면 되기 때문에 기기가 추가될때마다
        추가적인 회선을 깔 필요가 없어져 구축비용을 아낄 수 있다.
         하지만 한 선에 데이터가 몰리게 된다면, 병목 현상이 일어나게 된다
```

*Network 의 종류*
```
근거리 통신망 LAN : 건물범위
광역 통신망 : WAN 지역-지역,국가-국가 연결
++)도시 통신망 : MAN :건물,도시 범위
LAN
비교적 근거리에 위치한 통신망을 연결하는 것
WAN
도시,국가,국제적으로 통신망을 연결하는 것(광역 통신망)
```
*InterNet 이란?*
```
인터넷은 전 세계적으로 연결된 컴퓨터 네트워크의 집합으로, 다양한 공공 및 개인 네트워크들이 상호 연결되어 있습니다
```
*프로토콜은 무엇인가?*
```
프로토콜은 서로간의 통신의 규칙이 있는데 한사람이 다른 한국어를 쓰고 다른 한명이 영어롤 쓰면 프로토콜이 다르다고 말할수 있다.
통신을 위해 사전에 약속한 규칙/규약
문법/의미/순서
TCP/IP: 인터넷에서 가장 중요한 프로토콜로 사용되며,인터넷의 기본적인 원리를 구성합니다. TCP는 신뢰성 있는 데이터
전송을 위한 프로토콜이고,IP는 데이터의 송수신을 위한 주소 지정 및 라우팅을 담당합니다.
HTTP:웹 브라우저와 웹 서버 간의 통신을 위한 프로토콜로,웹 페이지의 요청과 응답을 처리합니다.
FTP: 파일 전송을 위한 프로토콜로, 파일의 업로드와 다운로드를 지원합니다.
SMTP: 이메일전송을 위한 프로토콜로, 이메일의 발송과 수신에 사용됩니다.
```
*네트워킹 모델의 목적은 무엇인가?*
```
호환성(제조사/국가가 다른 통신장치간의 통신목적)
네트워크망 제작시 사용되는 지침서
네트워크망 이상발생시 문제해결에 사용되는 용도
```
*OSI 7계층 TCP/IP 프로토콜 스택*
|OSI 7 LAYER|PHYSICAL LAYER|
|:---:|:---:|
|![1](https://github.com/user-attachments/assets/f6fa51ba-402f-42c4-8640-c84162b8578e)|![2](https://github.com/user-attachments/assets/178bcf0b-b093-495b-9d65-781caef8bb62)|

---
물리 계층(1계층)
---
```
물리적 연결과 관련된 정보를 정의!
√ 주로 전기 신호 전달하는데 초점이 맞춰져있음
√ 물리계층 장치는 케이블,리피터,허브 등이 있다
√ 허브, 리피터: 네트워크 통신을 중재하는 네트워크 장비
√ 케이블은 전기를 이용해서 신호를 전달
√ 케이블 종류는 이더넷 케이블 (UTP,STP)
√ 부호는 의미를 가지는 약속된 기호
√ 리피터:신호 증폭 장치
√ 허브:여러 대의 컴퓨터 간 통신이 가능(리피터의 기능도 가지고 있음)
```










데이터 링크 계층(2계층)
---
```
전기 신호를 모아 우리가 알아볼수 있는 데이터 형태로 처리!
전기 신호를 모아 데이터 형태로 처리하므로 데이터에
대한 에러를 탐지하거나 고치는 역할을 수행할수 있음.
√ 포인트 투 포인트(Point to Point) 간 운송방식 결정
√ 포인트 투 포인트(Point to Point) 간 신뢰성 있는 전송을 보장하기 위한 계층
√ 필요 요소: 식별주소.오류 제어,흐름 제어
√ 사용되는 프로토콜:LAN/WAN
√ 이더넷 통신문제점: 충돌 도메인 발생
√ 이더넷 통신 방법: CSMA/CD 다중접속 하는 방식
√ 이더넷 문제 해결 장치 :CSMA/CD 사용 안함, 이더넷 스위치화 및 고속화 지향(L2 Switch)
```



네트워크 계층(3계층)
---
```
IP 주소와 같은 논리적인 주소가 정의됨
데이터 통신을 할 때 사용되는 두 가지 주소
  * 2계층의 MAC 주소
  * 3계층의 논리적인 IP 주소
√ 역할:경로 탐색
√ 전달하려 하는 데이터를 목적지로 빠르고 안전한 경로로 안내하기 위한 최적경로 탐색
√ 장치:라우터, 레이어 3 스위치
√ 프로토콜 종류:Ip, ICMP, ARP, Routing Protocol(RIP,EIGRP,OSPF)
√ 라우터는 3계층에서 동작하는 장비로 IP 주소를 이해할수 있음
라우터는 IP 주소를 이용해 최적의 경로를 찾아주고 해당 경로로 패킷을 전송하는 역할
√ IP의 용도는 인터넷 환경에서 사용되는 구조
√ Routing 프로토콜은 최적 경로탐색에 사용됨
```





전송계층(4계층)
---
```
여기까지가 하위 계층입니다.
1, 2, 3계층은 신호와 데이터를 올바른 위치로 보내고 실제 신호를 잘 만들어 보내는데 집중함
4계층은 실제로 해당 데이터들이 정상적으로 잘 보내지도록 확인하는 역할
(종단간 데이터의 신뢰성을 보장)
OSI 모델중 4계층 모델이 하는 역할에 대해서 서술하세요 
  종단간의 데이터의 신뢰성을 보장
√전송계층 장치는 L4 SWITCH
√전송계층 프로토콜 : TCP,UDP
√TCP(종단 호스트 내 프로세스 상호 간에 신뢰적인 연결지향성 서비스를 제공)
1 신뢰성 : 종단간 데이터 이상유무 확인
2 연결지향 : 계속적인 데이터 교환을 위한 연결통로 설정
√UDP(TCP 프로토콜에 비해 구조가 단순한 전송계층 프로토콜
데이터의 빠른 전송에 적합)
실시간 응용 및 멀티캐스팅 가능
  - 빠른 요청과 응답이 필요한 실시간 응용에 적합
  - 여러 다수 지점에 전송
```
* IPv4*
```
Bit(Binary Digit)
아라비아숫자를 2진수로 변활 할때 표현되는 한자리
Byte = 8bit의 한묶음
```
*IP주소 표현*

|8bit|8bit|8bit|8bit|
|:---:|:---:|:---:|:---:|
|00000000|00000000|00000000|00000000|
>한개당 1byte로 4개의 8bit가 모이면 4byte 된다

*SUBNET MASK*
```
서브넷마스크란?
 네트워크IP/호스트IP를 지정하기 위해 사용되는 마스크
 32bit로 구성
 1 : 네트워크 IP
 0 : 호스트 자리

서브넷 마스크를 IP에 적용
 IP 192 168 10  1
 SM 255 255 255 0
```
```
클래스풀
 인터넷 상의 IP 주소를 규격화된 크기별로 구분시키는 방식
클래스리스
 Class 라는 규격화된 구분없이 비트 단위별로 IP 주소 범위를 가변적으로 구현
```
 
![333760864-4ae95582-a2aa-43d6-973a-b2c65a7e4556](https://github.com/user-attachments/assets/5a390e99-b649-430e-a5b0-b85e061c7a15)

![333760936-9c4b1ae1-041e-4472-bd40-669ce4cb4ba5](https://github.com/user-attachments/assets/cee0633d-1fa8-4349-b154-f3c299d585e8)

![333760981-9a95d296-c0c3-411b-bec6-3e3569118c59](https://github.com/user-attachments/assets/905de0e1-3586-4f5d-8f09-b426b9dccdf4)

*라우팅(STATIC ROUTING)*
 ```
라우팅 프로토콜
 라우터 간에 라우팅 정보의 교환 및 라우팅테이블의 유지관리를 동적으로 수행하는 프로토콜

필요 기능 및 요소
 1. 라우팅 수행 프로세스
  > 라우팅 정보를 주고받기 위한 프로세스
  > 최적 경로 계산 및 이를 라우팅 테이블에 기록하는 프로세스
  > 토폴로지 변화를 감지하고 이를 자동으로 학습 반영하는 프로세스
 2. 라우팅 테이블의 갱신관리
  > 최적 경로 결정을 위한 알고리즘 및 프로세스들 적용
 3. 라우팅 알고리즘
  > 최적 경로 산출을 하여가며 라우팅 테이블의 갱신,유지관리
 4. 라우팅 프로토콜 메세지
  > 라우팅 정보를 라우터들 간에 운반,전달,교환 등

라우터 메트릭
 RIP,OSPF,IGRP,EIGRP,BGP
```
*정적인 라우팅*
```
정의
 네트워크 관리자가 패킷의 경로를 수동으로 구성하는 라우팅 방식
  > 네트워크 환경 변화와는 무관하게 항상 같은 경로로 만 라우팅 경로의 설정 및 유지
    . 고정적이므로, 만약 토폴로지 변화 때, 수동으로 직접 작업해야 함

특징
 관리자가 라우팅 테이블을 직접 구축
 멀리에 있는 라우터까지의 경로를 일일이 수작업으로 경로를 구성
 유연성이 없어, 혼잡에 즉각적인 대응에 취약함
```

*라우팅(DYNAMIC ROUTING)*
```
AS란?
 자치시스템
동일한 라우팅 정책으로 하나의 관리자에 의하여 운영되는 네트워크, 즉 한 회사나 단체에서 관리하는 라우터 집단
각각 AS영역은 고유식별번호를 가진다(0-65535)
```

![335833554-0df3f790-538c-484b-8467-024467e2108b](https://github.com/user-attachments/assets/34473c12-29ab-480c-ba57-1dcc2a965cfd)

```
AS 번호 장점
 인터넷상에서 독립적인 네트워크를 식별
 외부 네트워크와의 경로를 교환
 고유한 라우팅 정책을 구현

ASBR이란
 AS Boundary Router
 AS 가장자리에서 다른 AS를 연결할 때 사용되는 라우터<br>
 자신의 AS와 인접한 다른 AS에 대한 정보를 가지며 자신을 경유하는 라우터에 외부 AS에 대한 정보를 제공

IGP
 IGP (Interior Gateway Protocol 또는 Intra-domain Routing Protocol)
 자치시스템 내부에서 만 이루어지는 라우팅 프로토콜 (Routing Protocol)

BGP
  BGP (Border Gateway Protocol)
  자치시스템 (AS) 상호 간에 적용되는 라우팅 프로토콜 (Inter-Domain Routing Protocol)
  즉, 독립 운용되는 대규모 네트워크 (AS) 간에, 네트워크 정보를 교환하기 위해 주로 사용됨
```











ROUTING PROTOCOL     
ROUTE : 길/경로
ROUTER : 경로안내장치
ROUTING : 길 안내작업

AS(Autonomous System) : 자치 시스템, 관리자가 관리하는 라우터의 집합(집단)
IGP(Interior Gateway Protocol)
EGP(Exterior Gateway Protocol)

DISTANCE VERTOR :
전체경로학습 -> 최적경로계산

LINK STATE                               대역폭(BandWidth),부하(Load),지연(Delay),신뢰도(Reliability),최대전송단위(Maximum Transmission Unit)0
1.전체경로 학습 -> 2 최적경로 산출           Serial : 10^8






경로를 안내해주기위해서 사용되는 프로토콜

DNS SERVICE/ SYSTEM / SERVER

Domain Name Service/System/Server
Domain : 영역
Name : 이름
Service : - 제공하다

WEB SERVICE
하이퍼텍스트 형식의 문서파일을 제공해주는 서비스

ProGram
Pro: 앞으로.미리
Gram : 쓰다, 적다

HardWar :

SofrWare : System SoftWare : WindowOS,Linux OS,,,
           Application

미들웨어
---
|-|
|:---|
|[OPEN JDK 다운로드](https://jdk.java.net/archive/)|
|[이클립스 다운로드](https://www.eclipse.org/downloads/)|
|[톰캣 다운로드](https://tomcat.apache.org/download-90.cgi)|

데이터베이스(Database)
---
```
데이터베이스란? -> 데이터의 저장소

DBMS(Database Management System,데이터베이스 관리시스템)란? -> 데이터 베이스를 운영하고 관리하는 소프트 웨어
계층형,망형,관계형 DBMS 중 대부분의 DBMS가 테이블로 구성된 관계형 DBMS(RDMBS)형태로 사용됨.

SQL(Strucyured Query Language)란? -> 구조화된 질의 언어라는 뜻으로 관계형 데이터베이스에서 사용되는 언어.
표준 SQL을 배우면 대부분의 DBMS를 사용할 수 있음.
```
|다운로드 경로|
|:---|
|[MySQL COMMUNITY 설치](https://hongong.hanbit.co.kr/mysql-%EB%8B%A4%EC%9A%B4%EB%A1%9C%EB%93%9C-%EB%B0%8F-%EC%84%A4%EC%B9%98%ED%95%98%EA%B8%B0mysql-community-8-0/)|


|SQL 기본 CRUD|
|:---|
|[기본 CRUD](DOC/README.md)|



mkdir /final

cd /final
touch 12 34 56

touch -t 199901011200 34
mkdir /back
ls -ld /final /back
cp /final/12 /final/56 /back
ls -l /back

cp -p /final/34 /back

ls -l /etc/login.defs /etc/passwd /boot/grub/grub.cfg
```
1번
mkdir /backup
cp /etc/login.defs /etc/passwd /boot/grub/grub.cfg /backup
ls -l /backup

2번
mkdir test
cp ./grub.cfg test/grub
cp ./login.defs test/login
cp ./passwd test/pass

3번
touch /backup/test1 /backup/test/test2
ls -l /backup
ls -l test
4번
mkdir -p /home/test/c/d
cp -rp /backup/test /home/test/c/d/linux

5번
cd /home
cp /backup/gurb.cfg /backup/login.defs /backup/passwd /backup/test1 /home/test/c/d/linux
```

passwd
ifconfig
pwd
cd위치변경
ls 디렉토리 목록확인 
mkdir 폴더 만들기
touch 빈 파일만들기
cp 파일복사
mv 파일이동
rm 삭제
---
cat.head.tail.more
>
vi



