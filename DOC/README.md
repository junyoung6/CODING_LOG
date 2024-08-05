>DDL/DML
```
-h:서버 주소, 일반적으로 ip를
입력하거나 네트워크 상 서버 이름으로 등록할수 있음.
localhost일 경우 생략할수 있음.

-u: 사용자 이름, User ID

-p: 비밀번호, User password
port번호를 적어준다
기본 포트인 3306일 떄는 생략가능.

DB 조회
 show databases;

DB위치 지정
 use mysql;

테이블 확인
 show tables;
 select * from user;

DB 생성
 db생성(TUI)
 create database testdb;
 show databases;

Table 생성
 table 생성(GUI) - 생략

table 생성(TUI)
 use testdb;
 show tables;
 mysql> create table tbl_user(
     -> user_id varchar(10) primary key,
     -> user_password varchar(100) not null,
     -> user_name varchar(45) not null);
--> 테이블 생성 보는법
      desc tbl_user;

컬럼 추가 alter
   mysql> alter table tbl_user add column user_tel varchar(30) null after user_name;
   mysql> desc tbl_user;(테이블 생성 확인)

컬럼 삭제 alter
   mysql> alter table tbl_user drop user_password;
    (user_password 가 삭제됨)

컬럼 수정 alter
   mysql> alter table tbl_user change column user_tel user_phone varchar(100) not null;
     (user_tel을 user_phone 으로 수정)

alter 명령어
 Column 추가 : amount int not null 
 Column 수정 : product_price -> product_price varchar(100) null
 Column 삭제 : product_details

 column 추가 : alter table 테이블명 add column 컬럼명 자료형 제약조건
 column 수정 : alter table 테이블명 change column 기존컬럼명 변경컬럼명 변경자료형 제약조건
 column 삭제 : alter table 테이블명 drop 컬럼명

   





