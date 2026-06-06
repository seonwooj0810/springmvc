# 스프링 MVC 1편

인프런 김영한 강의 **[스프링 MVC 1편 - 백엔드 웹 개발 핵심 기술](https://www.inflearn.com/course/스프링-mvc-1)** 을 따라하며 학습한 코드입니다.

> 진행 범위: 현재 코드는 강의 도입부의 **로깅**과 **요청 매핑(@RequestMapping)** 구간까지 다룹니다. 이후 섹션(요청/응답 파라미터, 메시지 컨버터, 뷰 등)은 아직 코드로 구현되지 않았습니다.

## 사용 기술

- Java 11
- Spring Boot 2.7.15 (`spring-boot-starter-web`, `spring-boot-starter-thymeleaf`)
- Lombok
- JUnit 5
- Gradle

## 학습한 내용

코드로 확인되는 주제입니다.

### 로깅
- `@Slf4j` 로거와 로그 레벨(trace/debug/info/warn/error) 출력 (`basic/LogTestController`)

### 요청 매핑
- `@RequestMapping`의 `method`로 HTTP 메서드 제한, 다중 경로 매핑 (`basic/requestmapping/MappingController`)
- `@PathVariable` 경로 변수 매핑 (단일/다중)
- 클래스 레벨 `@RequestMapping` + `@GetMapping`/`@PostMapping`/`@PatchMapping`으로 회원 관리 API 형태 매핑 (`basic/requestmapping/MappingClassController`)

## 프로젝트 구조

```
src/main/java/hello/springmvc
├── SpringmvcApplication.java
└── basic/
    ├── LogTestController.java          # 로깅
    └── requestmapping/
        ├── MappingController.java      # 요청 매핑, @PathVariable
        └── MappingClassController.java # 클래스 레벨 매핑
src/main/resources/static               # 정적 리소스 (index, hello-form)
```
