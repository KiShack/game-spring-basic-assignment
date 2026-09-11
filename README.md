# [필수 과제]

### Lv 1. 설정 파일 작성: Docker MySQL 연결

Spring Boot에 게임 데이터를 저장하기 위한 데이터베이스(MySQL)를 연결하는 작업.

Spring Boot ----> ( Docker ) ----> MySQL

* Docker : 소프트웨어 개발과 배포를 도와주는 컨테이너.

* 컨테이너(Container) : 애플리케이션과 그 실행 환경을 함께 패키징하여 **'어디서든 동일하게 실행될 수 있도록'** 해주는 기술.

application.properties : 'Spring Boot'에서 'MySQL'에 접속할 때 필요한 설정을 정하는 파일. (주소, 포트, DB 명, 사용자 명, 비밀번호 등)

---

### Lv 2. 의존성 주입(DI)

* IoC(Inversion of Control, 제어의 역전) : 객체를 직접 관리하지 않고 'Spring'에게 맡기는 것.

* @Service : 해당 클래스를 'Spring'이 관리하는 Bean 객체로 등록하도록 알려주는 이노테이션.

* Bean : 'Spring'이 관리하는 객체

* DI(Dependency Injection, 의존성 주입) : 'Spring'이 관리하는 Bean 객체를 필요한 곳에 넣어주는 것.

---

### Lv 3. RESTful API: 게임 목록 조회

* API(Application Programming Interface) : 서로 다른 프로그램이 기능이나 데이터를 주고받을 수 있도록 정해놓은 인터페이스(규칙).

* REST(ful) API : 클라이언트와 서버가 HTTP를 통해 데이터를 주고받을 때, REST 원칙을 기반으로 설계한 API. REST 원칙을 잘 따르도록 설계한 API를 RESTful API라고 한다.

* RESTful API 디자인 원칙
  1. 동사보단 명사, 단수보단 복수
  2. 마지막에 / 넣지 않기
  3. _ 대신 - 사용, 대문자 사용하지 않기
  4. 확장자 포함하지 않기
  5. 계층화 하기

---

### Lv 4. @Transactional

* 트랜잭션(Transactional) : 여러 개의 데이터베이스 작업을 하나의 작업 단위로 묶어 처리하는 것. **작업 중 문제가 발생하면 전체 작업을 되돌릴 수 있다.**
   -> 데이터 중 일부만 저장되는 식의 불완전한 상태를 방지하기 위함.

* @Transactional : 해당 메서드를 하나의 트랜잭션으로 처리하도록 'Spring'에게 알려주는 어노테이션.

* readOnly : 트랜잭션을 읽기 전용으로 설정하는 옵션. 데이터를 조회할 때 사용하며, 데이터를 저장하거나 수정하는 작업에는 사용하지 않는다.

---

### Lv 5. Bean Validation: 게임 생성

* DTO(Data Transfer Object) : 계층이나 프로그램 사이에서 데이터를 전달하기 위한 객체.

* Validation(검증) : 클라이언트가 보낸 데이터가 정해진 조건에 맞는지 확인하는 것.

* Bean Validation : @NotBlank, @NotNull, @Size, @Min, @Max 등의 어노테이션을 사용하여 데이터의 조건을 선언적으로 검증하는 방법.

---

### Lv 6. 보상 카드 선택과 진행 저장

---

### Lv 7. 저장된 여정 이어하기

---

### Lv 8.  더티 체킹: 이름 수정, 자식부터 삭제

---
