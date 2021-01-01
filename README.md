# Spring_Intro

###프로젝트 작성 중 새로 알게된 내용 과 팁을 작성한 문서

+ 프로젝트 생성할때 starter-web & thymeleaf 두 라이브 러리 추가
 web은 톰캣,mvc thymeleaf는 템플릿엔진

+ 프로젝트 첫 생성시 Setting - gradle - build and run using & run test using 둘다 intellij로 변경시 빌드 빨라짐


+ Logging library로 logback & slf4j 주로 사용한다.


-----
< Annotation>
+ @Controller : Controller 임을 명시

+ @GetMapping("hello") : get으 로 "" 안에 들어오는 URL 매핑해준다

+ @RequestParam("name") : 웹에서 'name'이라는 parameter 받음

+ @ResponseBody :Http의 Body부분에 return값을 직접 넣어주겠다는 의미