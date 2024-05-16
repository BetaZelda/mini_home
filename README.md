
# Cyworld Mini Homepage Project 

![SPRING](https://img.shields.io/badge/Spring-6DB33F?style=for-the-badge&logo=spring&logoColor=white)
![JAVA](https://img.shields.io/badge/Java-ED8B00?style=for-the-badge&logo=openjdk&logoColor=white)

![ORACLE](https://img.shields.io/badge/Oracle-F80000?style=for-the-badge&logo=Oracle&logoColor=white)

![HTML5](https://img.shields.io/badge/HTML5-E34F26?style=for-the-badge&logo=html5&logoColor=white)
<img src="https://img.shields.io/badge/css-1572B6?style=for-the-badge&logo=css3&logoColor=white"> 
![js](https://img.shields.io/badge/JavaScript-F7DF1E?style=for-the-badge&logo=JavaScript&logoColor=white)


## Intro

과거 인기 소셜 미디어였던 싸이월드를 재현한 미니 프로젝트.

로그인을 통해 각 회원별 미니홈피를 띄우고 해당 홈피에서의 게시물, 댓글 달기 기능 등을 구현함.


## 개발 환경
+ Spring Tool Suite 3 (v3.9.18)
+ Java 11
+ Oracle Database 11g Express Edition (v11.2.0.2.0) 
+ Tomcat v9.0


## 개발 기간
2024.05.07. ~ 2024.05.13.


## 팀원
+ 김종민(조장)
+ 한다솔
+ 박서경
+ 오승빈(moi)


## 하이라이트
### 싸이월드 레이아웃 재현
- 실제 싸이월드 미니홈피와 유사하게 스타일 지정.
- Controller에서의 mapping을 통해 문서간 링크 연결.

### 회원가입 및 로그인 
- 로그인을 통한 세션값 유지. 로그인한 해당 회원에 따라 싸이월드 홈피 내용이 다르게 출력.

### 싸이월드 게시물 업로드 기능/페이징
- SQL문 작성을 통해 미니홈피에서 작성한 게시물을 출력(Oracle DB). 한 페이지에서 일정 갯수 초과시 하단에 페이징.

### 각 게시물에 댓글 달기 추가
- 게시물과 별개로 각 게시물의 댓글도 DB에 저장 및 출력.



## Project Structure

```markdown
src
├── main
│   ├── java
│   │    ├── mini.interceptor
│   │    ├── miniDiary
│   │    ├── miniGuest
│   │    ├── miniHome
│   │    ├── miniLogin
│   │    ├── miniPhoto
│   │    └── miniProfile
│   └── resources
│   │    ├── config.mybatis
│   │    │    ├── dao-context.xml
│   │    │    ├── SqlMapConfig.xml
│   │    │    ├── login.xml
│   │    │    └── ...
│   │    └── db.properties
│   │ 
│   └── webapp
│        ├── resources
│        ├── WEB-INF
│        │     ├── spring
│        │     │    └── appServlet
│        │     │          └── servlet-context.xml
│        │     └── views
│        │          ├── homeL.jsp
│        │          ├── homeR.jsp
│        │          └── ...
│        │
│        ├── index.jsp
│        └── main.jsp
│
└── ...
```






