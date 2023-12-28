# java-boiler-plate

## 스프링부트로 새 프로젝트를 시작할때 필요한 것들 정리

---

### Version: Spring Boot 3.2.1
### Java: 17
<br>

1. [spring initializr](https://start.spring.io/)에서 초기 프로젝트 생성할때 포함시키면 좋은것들
   * Spring Boot DevTools
     * 이유 ~~그냥 넣자~~
       1. 코드변경시 자동재시작
       2. 디버깅
       3. 테스트
   * Lombok (**필수!!**)
     * Class에 getter, setter, toString, equals 등등 패턴 메소드까지 어노테이션으로 간단하게 지정
   * Spring Web(**필수!!**)
     * REST API서버를 만든다면 필수
   * Spring Data JPA (**필수!!**)
     * 자바 ORM 기술의 토대. 현재는 거의 querydsl과 함께 표준으로 자리잡은듯
   * H2 Database(**중요**)
     * 개발할때 DB (MySQL, Oracle ...)를 따로 연결하기 싫다면 의존성추가만으로도 사용할수 있는 간편함
   * MySQL, MariaDB, PostgreSQL Drive (택 1)
     * 데이터베이스들의 연결 드라이버. 사용할 것만 추가
   * Spring for RabbitMQ (선택)
     * 아직까지는 대기열, 동시성제어로만 사용해봤다 ㅠ ㅠ
   * Spring Security (**필수 !!**)
     * 어플리케이션의 보안과 관련된 것들이 모여있는 모듈.
   * OAuth2 Client / OAuth2 Resource Server (**필수 !!**)
     * OAuth2 프로토콜을 사용하여 인증하는 클라이언트를 구현하는데 필요한 기능제공
     * 간단하게 구축하려는 프로젝트에 N****, K****, G****, A***** 의 간편로그인이 들어간다면 사용하면 좋다
     
