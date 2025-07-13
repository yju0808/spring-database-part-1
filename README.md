# 🗄️ 스프링 DB 1편 - 데이터 접근 핵심 원리 정리

김영한님의 인프런 강의를 따라가며 실습한 코드와 내용을 정리한 레포입니다.
데이터 접근 기술의 근본 개념과 스프링 기반 해결책들을 학습했습니다.

---

## 📘 학습한 주요 개념

### 1️⃣ JDBC 이해

* JDBC 기본 동작 원리 이해
* `DriverManager`, `Connection`, `PreparedStatement` 사용법
* SQL 직접 작성 방식의 한계와 최신 기술 비교
* CRUD 로직을 직접 작성하며 JDBC의 불편함 체험

### 2️⃣ 커넥션 풀과 DataSource

* 커넥션 풀의 필요성과 개념
* `DataSource` 인터페이스 기반 구성
* `DriverManagerDataSource` vs `HikariDataSource`
* 커넥션 풀 라이브러리 적용 및 설정

### 3️⃣ 트랜잭션 처리

* 트랜잭션 기본 개념 및 동작 흐름
* JDBC의 수동 커밋, 롤백 처리 실습
* 동시성 문제와 DB 락 이해
* 트랜잭션이 필요한 실무 케이스 (계좌 이체 등)

### 4️⃣ 스프링과 트랜잭션 문제 해결

* 스프링의 트랜잭션 추상화 (`PlatformTransactionManager`)
* `TransactionTemplate`, AOP 기반 선언적 트랜잭션 처리
* 트랜잭션 동기화와 커넥션 재사용 원리
* 스프링 부트 기반 자동 설정 확인

### 5️⃣ 자바 예외 이해

* 자바 예외 계층 구조 (`Exception`, `RuntimeException`)
* 체크 예외 vs 언체크 예외
* 스택 트레이스와 예외 포함 원리
* 예외 활용 전략과 실무 판단 기준

### 6️⃣ 스프링과 예외 처리, 반복 문제 해결

* 스프링의 데이터 접근 예외 추상화 (`DataAccessException`)
* 예외 변환 전략 구현 및 적용
* JDBC 반복 코드 제거: `JdbcTemplate` 활용
* JdbcTemplate 기반 CRUD 구현 실습

---

## 🔗 참고

* 강의 링크: [스프링 DB 1편 - 데이터 접근 핵심 원리](https://www.inflearn.com/course/%EC%8A%A4%ED%94%84%EB%A7%81-db-1)
* 강사: 김영한
