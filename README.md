# Spring_Intro

### 프로젝트 작성 중 새로 알게된 내용 과 팁을 작성한 문서

+ 프로젝트 생성할때 starter-web & thymeleaf 두 라이브 러리 추가
 web은 톰캣,mvc thymeleaf는 템플릿엔진

+ 프로젝트 첫 생성시 Setting - gradle - build and run using & run test using 둘다 intellij로 변경시 빌드 빨라짐

+ Logging library로 logback & slf4j 주로 사용한다.
  
+ 객체의 return값이 Null일 경우가 있을때 Optional<> 로 감싼다.


-----
< Annotation>
+ @Controller : Controller 임을 명시

+ @GetMapping("hello") : get으 로 "" 안에 들어오는 URL 매핑해준다

+ @PostMapping" : post 방식 매핑

+ @RequestParam("name") : 웹에서 'name'이라는 parameter 받음

+ @ResponseBody :Http의 Body부분에 return값을 직접 넣어주겠다는 의미

+ @AfterEach : 각 테스트 코드가 동작후 실행되는 코드로 테스트 후 데이터 초기화 할때 쓴다

+ @SpringBootTest : 스프링 컨테이너와 테스트를 함께 실행한다.

+ @Transactional : '테스트 케이스'에 이 애노테이션이 있으면, 테스트 시작 전에 트랜잭션을 시작하고, 
  테스트 완료 후에 항상 롤백한다. 
  이렇게 하면 DB에 데이터가 남지 않으므로 다음 테스트에 영향을 주지 않는다.