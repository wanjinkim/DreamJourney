## 여행 플랫폼 서비스 DreamJourney
### 주제
Spring을 활용한 웹 프로젝트 구현

### 목적
- 교통, 숙소, 액티비티 예약 및 예매 서비스 제공, 사용자가 원하는 조건에 따라<br>해당하는 교통, 숙소, 액티비티 결과 조회 등 여러 서비스를 제공한다.
  
### 사용언어 & 사용기술
<img src="https://img.shields.io/badge/Java-007396?style=flat&logo=Java&logoColor=white" />  <img src="https://img.shields.io/badge/HTML5-E34F26?style=flat&logo=HTML5&logoColor=white" />  <img src="https://img.shields.io/badge/CSS3-1572B6?style=flat&logo=CSS3&logoColor=white" />  <img src="https://img.shields.io/badge/JavaScript-F7DF1E?style=flat&logo=JavaScript&logoColor=black"/>
<img src="https://img.shields.io/badge/Oracle-F80000?style=flat&logo=oracle&logoColor=white"/>  <img src="https://img.shields.io/badge/jQuery-0769AD?style=flat&logo=jquery&logoColor=white"/><br>
<img src="https://img.shields.io/badge/Bootstrap-7952B3?style=flat&logo=bootstrap&logoColor=white"/>   <img src="https://img.shields.io/badge/Chart.js-FF6384?style=flat&logo=chart.js&logoColor=white"/> <img src="https://img.shields.io/badge/Ajax-green?style=flat&logo=jquery&logoColor=white"/>  <img src="https://img.shields.io/badge/FlatPickr-blue?style=flat&logo=flatpickr&logoColor=white"/> <img src="https://img.shields.io/badge/RESTfulApi-yellow?style=flat&logo=restfulapi&logoColor=white"/> <img src="https://img.shields.io/badge/spring-green?style=flat&logo=spring&logoColor=white"/> <img src="https://img.shields.io/badge/Mybatis-black?style=flat&logo=mybatis&logoColor=white"/>

### 개발도구
<img src="https://img.shields.io/badge/Eclipse IDE-2C2255?style=flat&logo=eclipseide&logoColor=white"/>  <img src="https://img.shields.io/badge/Visual Studio Code-007ACC?style=flat&logo=visualstudiocode&logoColor=white"/>  <img src="https://img.shields.io/badge/Apache Tomcat-F8DC75?style=flat&logo=apachetomcat&logoColor=white"/>  <img src="https://img.shields.io/badge/Sourcetree-0052CC?style=flat&logo=sourcetree&logoColor=white"/> <img src="https://img.shields.io/badge/Git-orange?style=flat&logo=git&logoColor=white"/> <img src="https://img.shields.io/badge/Github-navy?style=flat&logo=github&logoColor=white"/> <img src="https://img.shields.io/badge/Exerd-red?style=flat&logo=exerd&logoColor=white"/> 

### 개발환경
<table>
  <tr>
    <td>OS version (platform)</td>
    <td>Windows(10, 11), Mac OS</td>
  </tr>
  <tr>
    <td>Language</td>
    <td>Java(OracleJDK 11.0.18), Oracle, HTML/CSS, JavaScript</td>
  </tr>
  <tr>
    <td>IDE</td>
    <td>SQL Developer, Exerd, STS 3.9.18, Visual Studio Code, Source Tree</td>
  </tr>
  <tr>
    <td>DB</td>
    <td>Oracle Database 11g</td>
  </tr>
  <tr>
    <td>Server</td>
    <td>Apache Tomcat 9</td>
  </tr>
  <tr>
    <td>API, Library</td>
    <td> REST API(Kakao Map API, Daum Postcode API, Iamport API, Kakao Login API), JavaMail API, jQuery, Chart.js, Flatpickr, Datetimepicker</td>
  </tr>
  <tr>
    <td>FrameWork</td>
    <td>Spring, Mybatis 3.5.2</td>
  </tr>
  <tr>
    <td>ETC</td>
    <td>BootStrap, Ajax, Git</td>
  </tr>
</table>

### 개요
여행과 관련된 기능을 제공하는 웹사이트로, 교통수단, 숙소, 액티비티 결제가 가능합니다.<Br>
또한, 소셜 기능을 통해 여행 공유가 가능하여 사용자들이 서로 정보를 공유하고<br>
계획을 세우는 기능을 제공함으로써 이용자에게 다양한 경험을 주는 것을 목표로 하였습니다.<br>

### 데이터 구조
![데이터구조](https://github.com/wanjinkim/DreamJourney/assets/45139754/50e01824-1769-47f0-9bd4-c393f65b8238)


### 담당업무
- 메인화면 설계
- 회원가입
- 커뮤니티 게시판(등록, 수정, 삭제)
- 커뮤니티 게시판 댓글(댓글 등록, 수정, 삭제)
---
### 화면구성
### 1. 메인화면 ⬇️
- header, 갤러리, footer로 이루어져있다.
- 메인 화면의 '로그인' 버튼을 클릭하여 로그인 페이지로 이동한다.
- 베스트 숙소, 베스트 액티비티, 드림저니 인기여행기 등은 모두 동적으로 처리된다.
- **예약/예매** : 교통, 숙소, 액티비티
- **추천여행지** : 지역
- **커뮤니티** : 베스트 여행기, 소통해요
- **Contact** : 고객센터
- **마이페이지** : 여행후기, 회원정보 수정, 탈퇴<br>
![메인회면](https://github.com/wanjinkim/DreamJourney/assets/45139754/13c5b08a-f72e-4af0-a6af-1ab807687c98)

### 2. 회원가입 ⬇️
- 닉네임, 전화번호, 이메일 등 중복검사를 포함한 인증번호 유효성 검사를 통과해야만 가입된다.
- 미성년자는 가입할 수 없다.
- 가입시 입력한 이름과, 전화번호 인증하는 사람의 이름이 같아야 가입을 할 수 있다.<br><br>
![회원가입_폼](https://github.com/wanjinkim/DreamJourney/assets/45139754/6c8ecfe2-cd08-4955-97a4-1d56e2a092c6)



### 3. 게시판 ⬇️
- 회원은 커뮤니티 게시판에 글을 등록, 조회, 수정, 삭제할 수 있다.
- 댓글 작성자만이 본인의 댓글을 수정, 삭제 할 수 있다.
- 동행 카테고리의 게시글에서는 채팅을 이용할 수 있다.<br><br>
![커뮤니티_게시판](https://github.com/wanjinkim/DreamJourney/assets/45139754/f6f57e24-76b5-4fdf-8c71-7afc27022701)
![댓글수정](https://github.com/wanjinkim/DreamJourney/assets/45139754/8d9cfdb6-3abc-4a5d-bb61-7beb81b7233d)
![커뮤니티_동행채팅_회원1](https://github.com/wanjinkim/DreamJourney/assets/45139754/1c8001c1-40d9-4469-afbc-d124440ccc4e)



### 4. 결제 ⬇️
- 원하는 액티비티를 선택한 후, 결제할 수 있다.<br><br>
![액티비티](https://github.com/wanjinkim/DreamJourney/assets/45139754/c3bddab5-b903-40d1-9c53-3172d1a61c34)
![액티비티_상세보기1](https://github.com/wanjinkim/DreamJourney/assets/45139754/b9db9f67-1066-4132-8845-d5eaf0f19cac)
![액티비티_상세보기2](https://github.com/wanjinkim/DreamJourney/assets/45139754/c4da2d93-f013-436e-a714-d4870ec0f1e9)
![결제](https://github.com/wanjinkim/DreamJourney/assets/45139754/afdbdeb3-fe84-4eb0-9daa-67b76feb8520)
![결제 전체화면](https://github.com/wanjinkim/DreamJourney/assets/45139754/3e6b5941-f3d9-4bf8-9f29-dd8f5e20baae)
![이니시스](https://github.com/wanjinkim/DreamJourney/assets/45139754/d997e1ea-5bd1-4769-a1f4-01a1754d137d)
![결제완료](https://github.com/wanjinkim/DreamJourney/assets/45139754/e5de6b14-5d0d-4e40-9763-78d57c5259ce)

### 5. 여행후기 작성
- 위치와 코멘트를 추가해야만 작성을 완료할 수 있다.
![마이페이지_내 여행_여행 등록 (4)](https://github.com/wanjinkim/DreamJourney/assets/45139754/ec6cd049-e426-4fc2-bbd0-f7e4acc393e6)
![마이페이지_내 여행](https://github.com/wanjinkim/DreamJourney/assets/45139754/b33fc846-1c2e-4dd6-b55f-ac364562b51e)



---
## 개발 스토리
### 회고
<table>
    <tr>
        <td>💡 프레임워크, API의 적극적인 사용 전과 후의 결과물의 퀄리티 차이는 뚜렷하다.
</td>
    </tr>
</table>
DI, IoC, AOP 등 처음 접하는 개념과 dependency 관리, 데이터베이스 설정 등 설정해야 하는 것들이 많아 
환경설정부터 쉽지 않았으나, 스프링의 특징에 점점 익숙해지면서 어노테이션을 활용한 URL 매핑(@GetMapping, @PostMapping)을 
사용하여 간단하게 컨트롤러의 메서드를 매핑하고 요청을 처리할 수 있었습니다.

또한, JDBC가 아닌 Mybatis를 사용함으로써 SQL과 자바 코드를 분리할 수 있어 가독성이 높아지고, 쿼리를 변경하기도 용이했습니다. 
'#{}' 형태로 파라미터를 쉽게 바인딩 할 수 있다는 것도 큰 장점이었습니다. 이를 통해 DB와의 연동이 더욱 효율적이고 쉬워졌습니다.

마지막으로, 의존성 주입 기능을 활용하면서 객체 생성과 관리의 편리함을 느꼈습니다.  @Autowired 어노테이션을 활용하여
객체를 생성하고 관리해 주기 때문에, 복잡한 객체 생성 로직을 사용하지 않아도 되었습니다. 

프레임워크를 활용함으로써 더욱 효율적이고 편리한 개발이 가능해졌으며, 기능을 구현하는 데에만 집중할 수 있어 조원들의 
업무 생산성이 Servlet/JSP 프로젝트에 비해 크게 향상되었습니다. 또한 API의 적극적인 활용으로 이미 구현된 고퀄리티의 기능을
활용함으로써 개발 시간을 줄여주었고, 이용자 입장에서도 좋은 질의 서비스를 제공받는 것을 경험하고 나서
모든 서비스를 개발자가 직접 구현하는 것이 좋은 것만은 아니라는 것을 느꼈습니다.
