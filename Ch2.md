## DB ch2 📃

## 01. 데이터베이스 관리 시스템의 등장 배경

### 파일 시스템
- 파일을 생성, 삭제, 수정, 검색하는 기능 제공

1. 같은 내용의 데이터가 여러 파일에 중복 저장됨
   - 저장 공간을 낭비, 데이터 일관성 데이터 무결성 유지 어려움
2. 응용 프로그램이 데이터 파일에 종속됨
   - 사용하는 파일의 구조를 변경하면 응용 프로그램의 구조도 변경해야 함
3. 데이터 파일에 대한 동시 공유, 보안, 회복 기능이 부족함
4. 응용 프로그램을 개발하기 쉽지 않음

## 02. 데이터베이스 관리 시스템의 정의
데이터베이스 관리 시스템 (DBMS: DataBase Management System)

- 파일 시스템의 데이터 중복과 데이터 종속 문제를 해결하기 위해 제시된 소프트웨어

DBMS이 제공하는 주요기능 3가지
- 정의 기능 : 데이터베이스 구조를 정의하거나 수정할 수 있음
- 조작 기능 : 데이터를 삽입, 삭제, 수정, 검색하는 연산을 할 수 있음
- 제어 기능 : 데이터를 항상 정확하고 안전하게 유지할 수 있음

## 03. 데이터베이스 관리 시스템의 장단점

### 장점
- 데이터 중복을 통제 가능
- 데이터 독립성 확보
- 데이터 동시 공유 가능
- 데이터 보안 향상
- 데이터 무결성 유지 가능
- 표준화 가능
- 장애 발생 시 회복 가능
- 응용 프로그램 개발 비용 감소

### 단점
- 비용이 많이 듦
- 백업과 회복 방법 복잡
- 중앙 집중 관리로 인한 취약점 존재

## 데이터베이스 관리 시스템의 발전 과정
데이터 모델에 따라 네트워크 DBMS, 계층 DBMS, 관계 DBMS, 객체지향 DBMS, 객체 관계 DBMS로 구분할 수 있음

데이터 모델 : 데이터를 데이터베이스에 저장하는 구조

### 1. 1세대 데이터베이스 관리 시스템 : 네트워크 DBMS, 계층 DBMS

(1) 네트워크 DBMS 
![image](https://github.com/leeseoyoung16/DB/assets/101916673/4e667ee8-8e73-42e6-a98a-f6789c677815)

- 노드와 간선을 이용한 그래프 형태로 구성하는 네트워크 데이터 모델 사용
- 데이터베이스 구조가 복잡하고 변경하기 어려움

(2) 계층 DBMS
![image](https://github.com/leeseoyoung16/DB/assets/101916673/b2d85b9f-f2c2-48fd-a18d-a7697d540a1a)

- 데이터베이스를 트리 형태로 구성하는 계층 데이터 모델을 사용
- 복잡한 현실 세계의 모습을 부모 자식 관계가 명확한 트리 형태로 표현하기 힘듦
- 구조 변경이 어려움\

ex> IMS

### 2. 2세대 데이터베이스 관리 시스템 : 관계 DBMS

(1) 관계 DBMS

![image](https://github.com/leeseoyoung16/DB/assets/101916673/9f4db7aa-2729-493b-a58a-00764621e430)
- 데이터베이스를 테이블 형태로 구성하는 관계 데이터 모델을 사용
- 단순하고 이해하기 쉬운 구조로 구성

ex> 오라클, MS SQL 서버, 액세스, 인포믹스, MYSQL, 마리아DB

### 3. 3세대 데이터베이스 관리 시스템 : 객체지향 DBMS, 객체관계 DBMS

(1) 객체지향 DBMS
- 객체를 이용해 데이터베이스를 구성
- 새로운 유현의 데이터를 저장하고, 데이터에 대한 복잡한 분석 및 처리 지원

ex> 오투, 온투스, 젬스톤

(2) 객체관계 DBMS
- 관계 데이터모델 + 객체지향 개념

ex> 오라클

### 4. 4세대 이후 데이터베이스 관리 시스템 : NoSQL DBMS, NewSQL DBMS

비정형 데이터가 대량으로 생성되며 등장

(1) NoSQL DBMS
- 안정성과 일관성 유지를 위한 복잡한 기능 포기
- 데이터 구조를 미리 정해두지 않아 비정형 데이터 처리에 적합
- 확장성이 뛰어나 여러 대의 서버 컴퓨터에 데이터를 분산하여 저장하고, 처리하는 환경에서 주로 사용

⚡ NOTE. SQL은 관계 DBMS를 의미 

ex> 몽고디비, H베이스, 카산드라, 레디스, 네오포제이, 오리엔트DB

(2) NewSQL DBMS
- 관계 DBMS가 제공하는 안정성과 일관성을 여전히 중요하게 평가, 정형 데이터 차지하는 비율 높음
- 기존의 관계 DBMS + NoSQL

ex> 구글 스패너, 볼트 DB, 누오 DB

![image](https://github.com/leeseoyoung16/DB/assets/101916673/155a35a4-6404-4468-947a-6039fa3a84a2)




   
