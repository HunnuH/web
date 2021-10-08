### Web

- web server : web에서 클라이언트의 요청을 받고 처리해서 클라이언트에게 요청처리 결과를 보내주는 프로그램이 설치 되어 있어야한다.

- 구조
  - web applocation 폴더 : `html`,`css`,`javascript`,`이미지`,`jsp` 파일 
    - Web Inf 
      - lib : 외부에서 가져다 사용하는 라이브러리파일
      - classes : 자바클래스, 서블릿클래스,db연동.....
      - `web.xml` : 하나의 사이트를 운영하기 위해 필요한 설정정보를 정의하는 설정파일

- 요청
  - 서버구축 후 `Context`를 만들어 놓은 후에 요청하는 방법
    - servlet & jsp가서 변경
    - `http://ip:port/context명/폴더명/web applicattion파일명`

-  웹환경 구축

  - dynamic web project구축

    - 폴더구조를 확인

  - 서버등록

    - 톰캣서버를 등록
    - 톰캣이 이클립스 밖에서 실행되고 있으면 이클립스는 실행할수없다
    - 이클립스 외부에서 실행되던 서버를 이클립스 내에서 실행되도록 등록
    - context를 서버로 배포 (*server.xml에 <contxet>가 추가된다)
      - 실제위치 : C:\bigdata_iot\work\webwork\.metadata\.plugins\org.eclipse.wst.server.core\tmp0\wtpwebapps\clientweb

  - 문자셋설정

    - utf-8
    - dynamic web project
    - html문서
    - jsp문서

  - 실행

- 태그

  - `<!--  -->` : 주석
  
  - `<h1~h6></h1~h6>` : 제목

  - `<font size=" " face=" " color=" "> </font>` :글씨 

  - `<ing src="이미지경로" width="가로사이즈" height="세로사이즈"` :이미지

    - 이미지의 경로  

      - 파일탐색기에서 확인가능한 파일의 경로를 사용해서는 안된다

      - 웹에서 요청하는 방식을 이용

      - 상대경로 :   <img src="./clientweb/images/viewa.png"/>

        ​                    `.` 현재위치    `..`상위디렉토리    

      - 절대경로 : 경로를 모두 명시 >  <img src="http://192.168.0.63:8088/clientweb/viewa.png"/>
  
        ​                                                     <img src="/clientweb/images/viewa.png"/>
    
  - 목록태그
  
    - 사이트제작시 메뉴로 많이 활용
    - 순서가 없는 목록,  순서가 있는 목록
  
  - 테이블태그
  
  - 양식태그
  
    - 서버와 통신하기 위해 사용(서버로 클라이언트가 입력,선택한 내용을 전송)
    - 무조건 `<form></form>`사이에 정의해야 서버로 데이터가 전송된다
    - 양식태그 종류
      - 텍스트관련 양식태그
      - 버튼
        - `submit`버튼을 누르면 `<form></form>`사이의 모든 양식 태그를 통해 클라이언트가 입력,선택한 값이 서버로 전송
        - 전송되는 데이터의 형식은 `name=value`
      - 선택기능
      - 서버로 데이터를 전송하기 위해서 값을 구분할 수 있도록 반드시 name속성을 정의해야 한다
    - 
  
  - html5요소

-----

### CSS

- css의 기본

  - css의 사용방법

    - 선택자 { 속성명1: 속성값1; .............}
    - 문서의 `<head>`태그 내부에 정의하기
      - 문서의 `<head>`태그 내부에 `<style>`태그로 정의하여 사용
      - 웹페이지 하나에만 속성을 정의하여 사용
    - 외부문서로 정의하고 사용하는 방법
    - 태그내부에 `<style>`속성을 정의해서 `inline`으로 사용하는 방법
- 선택자의 종류
  
  - 태그 : 정의된 모든 태그에 css속성을 적용
    - class속성 : 동일하게 정의된 컨텐츠에만 css속성을 적용
      - 태그와 상관없이 원하는 곳에 중복으로 사용이 가능
      - `.클래스명`{ 속성명1: 속성값1..........}
    - id속성 :  식별하기위한 목적, 컨텐츠 한곳에만 정의 (중복x)
      - 주로 자바스크립트, jquery에서 문서의 컨텐츠 식별
      - `<id = id명>``</태그명>`   정의방법
      - #아이뒤명 { 속성1: 속성값1......} 적용방법
    - 여러 선택자를 복수개 선택
      - 태그명, 태그명....{   }
  
  - 태그와 선택자를 활용
      - 동일한 태그를 이용해서  작업하는 경우 class속성이나 id속성이 정의된 태그에만 속성을 적용
    - 태그내부에 정의된 하위 태그
      - div태그 내부에 정의되어 있는 `<a>`태그에 속성을 적용하고 싶은 경우
  - 기본속성
- 박스모델
  - 포지셔닝
- 플로팅

------

### 자바스크립트

- 자바스크립트 기본
  - 사용방법
  - 문법
  - 함수
  - 내장객체
  - 이벤트처리
- 브라우저객체 모델
- DOM
- J-Query
- Ajax
- web socket
- 프레임워크
  - react JS
  - Angular
- 내부 자바스크립트 프로그램
  - node JS
  - Express
  - Mongo db
  - Angular

------

### 브라우저 객체(BOM)

- 웹페이지를 구성하는 모든 컨텐츠를 접근하는 방법

  - window

  - document

  - form

    - 객체 제어 : html태그에 정의되어 document에 출력되는 모든 구성요소를 객체로 정의하고 사용하기 위해서 name속성을 정의해야 한다.

    - 모든 브라우저 객체는 계층구조를 갖고 있다. 

      - ```html
        <body>
            <form name="myform">
               <input type="text" name="id"> 
               
            </form>    
        </body>
        <!-- 위처럼 정의된 text를 접근하는 방법-->
        window.document.myform.id
        ```

      - html로 웹페이지를  구성하는 컨텐츠를 저으이

      - css를 이용해서 레이아웃과 스타일 적용

        

  - image

  - history

-----

### window 객체

- 대화상자 관련
  - `alert` :안내창
  - `prompt`: 사용자로부터 입력을 받기 위한 창
  - `confirm`: 상호작용을 위한 선택창
- popup 관련
  - `open()`: 새창을 실행
  - `close()` :창을 닫기
  - `opener객체`:popup창을 실행해 준 부모창
- 데이터처리
  - `pareInt`: 숫자모양을 한 문자열을 숫자로 변환
  - `isNaN`:입력한 문자열이 숫자인지 문자인지 판단
  - `eval`: 매개변수로 전달된 문자들을 실제로 실행
  - `trim`: 공백을 제거
- 자동실행
  - 자바스크립트 함수 명령문을 일정 시간이 지난 후에 자동으로 실행할 수 있도록 지원
  - `setTimeout`: 자바스크립트 함수 명령문을 일정 시간이 지난 후에 한 번만 자동으로 실행
    - 작업id = setTimeout("실행할 자바스크립트 명령문 or 함수명");

-----

### DOM(document object model)

- 문서를 접근하는 방법을 표준으로 정의해 놓은 것
- 플랫폼이나 언어에 상관없이 컨텐츠의  구조를 통적으로 업데이트하고 엑세스 할 수 있도록 w3c에서 표준으로 정의해 놓은 문서 접근 방법
- `word wide web consortium` : 브라우저 내부에 포함된 html이나 css명세에 따라서 html문서를 해석하는데 이것을 w3c에서 정한다
- Dom구성요소
  - `document` : dom객체에서 가장 상위 객체
  - `element `:  html문서를 구성하는 모든 컨텐츠
  - `attribute` : 태그내부에 정의되어 있는 속성
  - `text` : 태그와 태그사이에 입력한 문자열 혹은  공백도 문자열 객체로 인식
  - Dom에서 사용할수 있는 속성
    - `nodeValue` : 노드의 값
    - `nodeName`: 노드의 이름
    - `chlidNode`:하나의 노드밑에 형성된 모든 자식노드를  반환
    - `firstchild` : 첫 번째 자식 노드 
    - `lastchild` : 마지막 자식 노드
  - Dom에서 사용할수 있는 메소드
    -  노드를 탐색하고 정보를 파악 				
      - `getElementsByTagName("태그명")` : 태그에 해당하는 모든 객체를 노드의 list형태로 반환 
      - `getAttribute("속성명")` : 해당 속성에 정의되어 있는 값이 리턴
      - `setAttribute("속성명,"값")` : 특정객체의 속성의 값을 변경하거나 설정
      - `getElementsById("id명")` : id로 정의된 dom객체를 반환		
    - 노드를 추가하고 변경 및 삭제
      - `createTextNode` : 텍스트노드 생성
      - `new imgNode`: 태그엘리먼트 생성
      - `appendchild("노드명")` :노드를 추가
        - 삽입될 노드를 생성 - createElement or createTextNode
        - 삽입될 노드의 위치를 구하기
        - 노드추가
      - `insertBefore` :노드를 추가
  - `callback함수` 
    - 해당 명령문이 실행될때 바로 호출되어 실행되는 함수가 아니라 어떤 이벤트가 발생하거나 특정 상태값이 변경되거나 ..할때 함수가 실행되도록 하는것
    - 브라우저 화면에서 발생하는 이벤트는 예측이 불가능 하므로 화면에 이벤트가 발생했을때 처리를 담당하는 브라우저 내부의 프로그램에게 어떤 함수를 실행할지 알려 주는일

-----

### J-Query

- 자바스크립트로 만들어진 라이브리이며 프레임워크 처럼 사용

- DOM을 쉽게 사용할 수 있도록 지원

- 크로스브라우징을 구현
  - 모든 브라우저에서 동일한 뷰를 볼수있도록 구성
  
- 기능
  - `DOM` : 객체의 필수속성, 메소드, 노드제어, 스타일 제어
  - Ajax
  - 플러그인 : 필요한 기능을 만들어서 제공하는 것 (JQuery로 만들어진 완제품) 
  - Effect : 애니메이션 효과
  
- 사용방법
  - 라이브러리 파일을 직접 다운 받아 프로젝트에 추가후 사용
    - `compress.ver` :압축 버전 로딩속도 빠름 (jquery-3.6.0.js)
    - `un compress.ver` : 개발자 버전 수정해서 작업이 빠름(jquery-3.6.0.min.js)
  - cdn방식
    - 외부사이트에서 공유한 jquery라이브러리 경로 추가하여 작업
  
- 형식
  - `ready handle` 이용 
    - 자바스크립트 이므로` <script></script>`태그내에서 작업
    - `ready handler`는 브라우저 내부에서 dom객체가 생성이 완료되면 jquery작업을 시작하겠다는 의미
      - $(document).ready(function(){        })
  - 일반적인 jquery문법
    - `$("선택자").동작(  )`
  
- 선택자
  - `$(객체)` : 선택자로 지정한 객체에 적용
  - `$("*") `: dom객체의 모든 요소
  - `$("id명")` : 작성한 id속성으로 정의된 요소에 적용
  - `$(".class명")`  : 작성한 class속성으로 정의된 모든 요소에 이용
  - `$(this)` : 현재 작업중인 엘리먼트에 적용
  - `$("태그명1 태그명2")` :태그1의 하위로 정의되어 있는 태그2를 선택자로 사용
  - `$("태그명. 클래스명")` : class속성으로 정의된 특정 태그를 선택자로 사용
  - `$("태그명:first") ` : 태그들 중 첫번째 엘리먼트를 선택자로 사용 
  - `$("태그명1 태그명2: first-child")` : 모든 태그명1의 하위 엘리먼트 중 첫번쨰 엘리먼트들을 선택자로 사용
  - `$("[속성명]")` : 작성한 속성을 갖고 있는 모든 엘리먼트를 선택자로 사용
  - `$("태그명[속성명=속성값]")` : 특정태그의 속성과 속성값을 비교해서 일치하는 엘리먼트를 선택자로 사용 
  - `$(":input태그의 type")` : 해당 type속성으로 정의된 form태그의 요소가 선택(HTML의 요소에도 적용)
  - `$("태그명:even")`: 짝수
  - `$("태그명:odd")` : 홀수
  
- DOM제어 메소드
  - `append()` :선택된 요소의 lastchild 컨텐츠 추가
  - `prepend() `:선택된 요소의 firstchild 컨텐츠 추가
  - `after()` :선택된 요소의 뒤에 새로운 컨텐츠 추가
  - `before() `:선택된 요소의 앞에 새로운 컨텐츠 추가
  - `remove()` : 선택된 요소와 그 자식 요소를 삭제
  - `empty() `:선택된 요소의 자식요소 삭제
  
- setter/getter 메소드
  - `text()` : 원하는 위치에 텍스트 추가 > set/get둘다 가능(html태그 적용불가)
  - `val() `:  입력필드의 값을 반환하거나 설정 > set/get둘다 가능
  - `html()` : 원하는 위치에 html태그를 추가
  - `css()` : css속성을 설정
  - `attr() `: 태그의 속성을 셋팅 dom의 표중 api메소드에서 setattribure와 동일
  
- 이벤트
  - `on()`를 이용  - 정식
    - bind의 성능을 개선
  - `bind()`를 이용 
  - 이벤트에 대한 약식 표현
    - `객체.click()`  
  
- effect
  - `hide()` : 선택된 요소를 화면에서 감춘다
  - `animate` : 커스텀 애니메이션을 만들때 사용
    - 형식 :` .animate( properties [,duration] [,easing] [,complete] )`
    - `properties `: {  }로 표현이 가능하며 필수로 지정해야 하는 매개변수(css속성)
    - `duration (speed) `: 효과가 나타나는 속도를 의미
    - `easing` : 포인트 이동할때 애니메이션 속도를 지정
    - `complete` : callback으로 함수명을 명시
  
- jquery ui

- bootstrap

----

### JDBC( Java DataBase Cconnectivity)

- 자바로` DBMS`연동을 하기위한 기술
- 오라클에 접속해서` JDBC`를 사용하기전 설정
  - 오라클 드라이버를 다운
  - 오라클드라이버를` JVM`이 인식할수있도록 설정
    - 이클립스가 아닌경우 
      - `jdk`의` lib`폴더나` tomcat`의 `lib`에 복사에서 사용해도 되지만 가급적 자제 (충돌할 경우가 생김)
    - 이클립스 사용하는 경우
      - 작업프로젝트 선택
      - 프로젝트 선택 후 단축 메뉴를 `[buid path] > [cinfigure build path..]` 선택
      - 대화상자에서 `[libraries]`탭 선택
      - `Modulepath`선택
      - `[add external jars..]`선택후 라이브러리 파일의 경로를 찾아서 등록

- JAVA API를 이용해서 JDBC연동

  - 오라클 드라이버 로딩

    - 오라클 드라이버를 `jvm`이 인식할 수 있도록 핵심클래스를 메모리에 로딩

    - `Java.lang`패키지에 `class`라는 클래스를 이용해서 오라클 드라이버의 핵심클래스를 메모리에 로딩

    - `[MySQL] `: 핵심클래스명 - com.mysql.jdbc.Driver

      ​                   `Class.forName("com.mysql.jdbc.Driver")`

- DB서버에 연결

  - `driverManager`의 `getConnection`이라는 메소드를 이용해서 DB서버에 연결

    - `static`메소드이므로 클래스이름으로 엑세스

    - `throws`하고 있는 `SQLexception`은  `Exception`하위이르모 문법적으로 `Exception`에 대한 처리를 해야한다

    - 매개변수

      - `url` : 연결문자열(어떤 `DBMS`를 쓰느냐에 따라서 다른 형식의 문자열을 작성해야 한다)
      - `user` : 사용자계정
      - `password` : 패스워드

    - 리턴타입

      - java.sql.Connection을 리턴

      -   DriverManager클래스의 getConnection메소드는 DB서버에 연결하고 연결정보를 객체로 만들어서 리턴한다. 

      - 리턴하는 연결정보를 표현해놓은 객체가  java.sql.Connection 표준API는  java.sql.Connection이지만
        연결정보를 노출시키면 안되므로 실제로는 Connection을 상속받은 오라클사에서 만든 Connection의 하위객체가 리턴된다.

      -  Connection은 스펙만 제시하는 인터페이스이고 이를 상속받아서 DBMS제조사에서 작성한 객체를 실제로 사용하는 것
           다형성이 적용되어 있다.

      - SQL실행

        - `statement`사용

          - `executeupdate `: `insert`, `update`, `delete`명령문을 실행

            ​								매개변수로 sql문을 전달하면 실행결과로 몇개의 row가 실행 반영되었는지 리턴
          
        -  PreparedStatement를 사용
                ① executeUpdate : insert, update, delete명령문을 실행
                ② executeQuery : select명령문을 실행
                => 리턴타입이나 실행 모두 Statement와 동일하나 매개변수로 sql을 전달하지 않는다.
        
      - 결과처리

        - nsert, delete , update
                - 모두 int를 리턴하기 때문에 동일한 방법으로 처리
                      int result = stmt.executeUpodate(sql)
           -  select
                      sqlplus프로그램을 이용해서 select sql문을 실행하면 결과로 테이블(2차원표의 형태)이 리턴
                      이 테이블을 자바로 만든 application에서 사용할 수 있도록 모델링해 놓은 클래스가 ResultSet

         - 자원반납

                 - 클라이언트가 점유해서 사용하던 자원을 반납해야 한다.
                 - close메소드를 이용해서 반납하고 객체가 만들어진 순서가 아니라 가장 마지막에 만들어진 객체부터 해제한다.                                         

------

### 서블릿

- 개요

  - 클라이언트의 용청을 처리하기 위한 기술
  - 클라이언트가 요청하면 서버에서 실행되면 DB에 대한 처리등 리소스를 사용하여 만들어진 결과를 응답
  - 서버에 의해서 호출되기 때문에 서버가 인식하는 위치에 저장되어 있어야 한다.
  - 개발자가 서블릿을 호출하는 명령문을 직접 정의하는 것이 아니라 서버에 의해서 호출되어야 하므로 정해진 규칙대로 만들어야한다

- 작성방법

  - 표준화된 폴더 구조안에 서블릿 클래스가 작성되어야 한다

    - 서블릿이 저장되는 폴더 - classes폴더
    - 이클립스에서는 자동으로 classes폴더가 복사된다

  - 서버에 의해서 호출되어야 하므로 반드시 public클래스로 작성해야 한다

    - 어떤 패키지에 작성하더라도 서버가 찾아서 실행할 수 있어야 하므로

  - 서블릿클래스가 되기 위해서는 무조건 서블릿클래스를 상속받아야 한다.

    - 서블릿클래스에는 내부적으로 네트워크로 요청되는 데이터를 받아서 처리하거나 분석하는 등의 기능이 미리 작성되어 있다.

  - 서버가 호출할 메소드(콜백메소드)를 오버라이딩

    - 서버가 클라이언트의 요청을 분석해서 서블릿 디렉토리에 존재하는지 찾는다.
    - 서블릿의 적절한 시점에 호출되는 메소드를 실행한다.
    - 서버가 서블릿객체를 생성하고 관리한다.(life cycle관리)

  - 오버라이딩 메소드

    - init : 서블릿 객체가 초기화될때 호출되는 메소드

    - destroy : 서블랫 객체가 소멸될때 호출되는 메소드

    - service : 클라이언트가 요청시 호출되는 메소드

      ​               클라이언트의 요청을 처리하는 메소드로 요청을 받고 처리할 내용을 구현

    - doGet : 클라이언트가 get방식으로 요청할떄 호출되는 메소드

    - doPost  : 클라이언트가 post방식으로 요청할때 호출되는 메소드

  - 서버가 서블릿을 찾을수 있도록 등록(web.xml)

    - 서버가 요청을 분석해서 실행할 서블릿을 서블릿 디렉토리에서 찾아서 실행한다.
    - 서버가 요청을 확인하고 어떤 서블릿클래스를 실행해야 하는지 알수있도록 설정파일에 등록
    - web.xml에 등록(태그로 작성)

- 요청방법

  - get방식 요청
    - 주소표시줄에 입력해서 요청
      - 주로 테스트용도
      - http://서버ip:port/context명/서블릿맵핑명
    - 하이퍼링크로 요청
      - 텍스트나 이미지를 클릭해서 서블릿을 요청
        - `<a href = "/context명/서블릿맵핑명">서블릿요청</a>`
    - `<from>`태그의 method속성을 get으로 정의 하고 submit버튼을 눌러서 요청
    - 사용자가 양식태그를 통해 입력한 모든내용이 요청 hrader에 추가되어 서버로 전송되는 방식
    - 사용자가 입력한 모든 내용이 그대로 노출되므로 보안에 적합하지 않다
    - 서버에 저장된 데이터를 가져오는 경우 사용되는 방식
    - 클라이언트가 입력한 내용을 제한적으로 전송
  - post방식 요청
    - 사용자가 입력한 데이터가 요청메시지 body에 추가되어 서버로 전송되는 방식
    - 사용자가 입력한 모든내용이 요청된 body에 추가되므로 노출되지 않는다
    - 클라이언트가 입력한 모든 내용의 데이터를 전송 가능
    - 파일업로는 무조건 post방식으로 처리

-----

### JSP 

- 지시자

- 스크립트요소 : `<%` 로 시작하는 것을 스크립트 요소라고 한다

  - 주석문  : `<%-- -- %>`

  - 스크립트릿  
    - 자바코드를 쓸수있는 스크립트요소
    - `<% %>`
    - html태그와 같이 사용가능
    - `<% %>`안에 작성하는 모든 코드는 _jspservice메소드 내부에 자동으로 추가된다
    - java처럼 java.lang패키지 뺴고 모든 패키지는 import해야 한다.
    - 스크립트릿 안에서는 _jspservice메소드 내부에 선언된 모든 지역변수를 사용할 수있다.
  - 표현식
    - 문자열이나 메소드 호출 결과, 연산식 등을 웹 페이지에 출력하기 위한 목적으로 사용
    - `<%= 변수, 메소드호출(리턴타입), 연산식...%>`
    - 표현식 내부에서 사용하는 값들이 out.print메소드 내부에 생성
    - ;을 추가하지 않는다
    - 표현식은 자바에서 만들어진 값을 웹 페이지에 출력할 목적으로 제공되는 스크립트요소이며 스크립트릿과 html태과 같이 사용 할수 있다.
  - 선언문
    - `<%! %>`
    - jsp문서에서는 거의 사용하지 않는다
    - 멤버변수나 멤버메소드를 정의하기 위해 사용

- 내장객체

- 액션태그

- EL& JSTL

-----

### 요청재지정

- 클라이언트로 부터 최초로 받은 요청을 실행하고 새로운 요청을 하는방법
- 화면을 분리하고 분리된 화면으로 응답하기 위해 필요한 기술
- MVC패턴을 이해하고 개발하기 위해 반드시 필요한 개념
- 데이터 공유
  - 서블릿에서 발생한 데이터를 요청재지정 하는 뷰로 넘겨주기 위해서 데이터를 서블릿에서 공유해야 한다.
    - page(this - 현재jsp페이지에서만 공유)  >> javax.servlet.jsp.pagecontext
    - request(요청객체 - 한번의 request가 응답되는 동안 실행되는 객체들이 공유)  >> HttpservletRequest
    - session(세션객체 - 세션이 생성된 순간 브라우저에서 보여지는 모든 웹 페이지에서 데이터를 공유) >> Httpsession
    - application(context 객체 - 톰캣메모리에 공유해서 톰캣에서 실행되는 모든 웹 페이지에 공유 )  >> servletcontext
- 데이터 저장
  - 객체.setAttribute("저장할 attribute의 이름", 저장할 객체)

- 데이터 가져오기
  - object 변수 = 객체.getAttribute("공유된 attribute의 이름") 
- 요청재지정
  - redirect
    - HttpservletResponse의 sendRedirect메소드를 이용해서 처리
    - response.sendRedirect("요청재지정될 wev application의 path")
    - 최초요청된 서블릿이 response된 후 재요청하는 방법이므로 데이터를 공유 할수없다.
  - forward
    - RequestDispatcher rd = request.getRequestDispatcher("요청재지정으로 실행할 application의 path")
    - rd.forward(request객체, response객체)
    - 최초 요청된 서블릿이 실행된 후 응답하지 않은 상태에서 요청재지정으로 명시된 application이 응답
    - 한번 요청으로 모든 application을 실행 따라서 데이터 공유가 가능
  - include

-----

### Spring

- 프레임워크 개요

- 스프링의 특징

  - 경량의 시스템

  - pojo(Plain Old Java Object)기반 시스템을 개발

    - 기존에 사용하던 자바 클래스를 그대로 사용해서 만들어진  클래스를 이용해서 개발

  - Ioc(Inversion of Control) 컨테이너를 제공

    - 객체를 lifecycle을 관리하는 컴포넌트

    - 의존성 주입 : 시스템내부에서 사용하는 객체를 생성하고 소멸하고  사용하는 곳에 전달해주는 역활을 담당하는 컴포넌트가     

      ​                       프레임워크 내부에 있으며 이를 스프링 컨테이너라고 한다.

    - 스프링내부에서 지원하는 Ioc컨테이너를 이용해서 커플링을 낮게 만들수있다

    - 스프링 결합도를 낮추기 위해서 객체에 대한 모든 생성을 코드에서 직접 new하지 않고 프레임 워크 내부에서 컨테이너가 관리하도록 한다

    - IOC컨테이너의 유형

      - BeanFactory - Application
        - getbean이 호출되면 객체를 생성해서 넘긴다
        - getbean호출되면 전달한 id에 해당하는 객체만 생성
      - ApplicationContext - Application
        - 컨테이너객체가 생성될때 등록된 xml문서에 정의된 모든 bean을 생성해서 컨테이너 내부에 존재하는 map형태의 자료구조에 저장한다.
        - bean과 bean사이에 관계가 설정되어 있다면 이 관계도 모두 셋팅한 후 객체를 저장
        - 사용하지 않는 bean에 오류가 있으면 오류를 발생시킨다.
      - WebApplicationContext - web

    - 객체사용하기

      - DL(Dependency Lookup)
        - 컨테이너가 제공하는 메소드를 통해서 객체를 스프링컨테이너로 부터 가져오는 작업
      - DI(Dependency Injection)
        - 개발자가 직접코드를 구현을 통해서 스프링 컨테이너로 부터 객체를 받아오는 DL과 다르게 spring내부 클래스에서서 사용하는 객체를 자동으로` mapping`시켜주는것
        - `applicationContext객체`가 생성될때 자동으로 DI가 처리된다
        - 개발자는 설정 파일에 생성할 객체와 어떤 방법으로 어떤 객체를 주입할 것인지 명시
        - 클래스에는 명시한 방법에 따라서 객체를 주입받을 수 있도록 `setter메소드`나 생성자를 미리 정의해야한다.
        - `Contructor Injection `
          - 생성자를 통해서 객체를 주입하는 방법
          - oop특성이 적용되어 있는 상태
          - xml설정 파일에 생성자 방식으로 객체를 전달할 수 있도록 `<construct-arg>`가 `<bean>`내부에 정의 
          - `<construct-arg>`태그의 갯수가 생성자 매개변수 갯수와 동일
        - `setter injection`
          - `setter메소드`를 통해서 객체를 주입받는 방식으로 기본은 무조건 기본생성자를 호출한다
          - 컨테이너에 의해서 만들어질 객체는 기본생성자가 정의되어 있어야 한다
          - `setter메소드`를 호출할 수 있도록 정의해야 한다
          - 설정파일에` property태그`를 이용해서 객체를 전달받을수 있도록 정의

----

### 어노테이션 

- 어노테이션을 사용하는경우
  - 설정파일에 `context`네임스페이스 추가
  - `<context:component-scan >`을 이횽해서 빈을 찾을 패키지를 등록
  - `controller`,` service`, `repository`로 빈을 등록
  - DI설정
    - @Autowide`
      - `<context:component-scan >`에서 선언된 타입과 동일한 객체를 찾아서 injection시켜준다
    - `@Qualifier`
      - 동일한 타입의 빈이 두개이상 있는 경우 정확하게 어떤 빈을 연결할 것인지 @Qualifier어노테이션을 이용해서 빈을 설정한다.

- 빈을 생성하는 경우 사용하는 기호
  - `componen`t :  기본 빈을 등록 하고 사용
  - `service` : 서비스빈의 역활을 하는 경우 등록
  - `repository` : db연동을 위한 빈
  - `controlle`r : 웹에서 사용하는 컨트롤러의 역활응 하는 빈을 등록

----

### front Controller

- 모든 요청을 하나의 서블릿에서 처리하도록 구조를 만드는 패턴
- 보안로깅,트랜잭션처리, 웹에 관련된 모든 기능을 스프링에서 제공하는 기능을 사용할 것이므로 모두 스프링 웹MVC를 통해서 요청이 처리 되도록 한다
- 요청이 하나의 서블릿에서 관리
- 웹에서 주로 사용하는 패턴
- 창구역활을 하는 컴포넌트를 제작하겠다는 의미

---

### spring mvc프로젝트 생성

- `pom.xml`파일의 `<proertises>`엘리먼트에서 자바와 스프링 버젼을 변경

  ```java
  <properties>
  		<java-version>1.8</java-version>
  		<org.springframework-version>4.2.4.RELEASE</org.springframework-version>
  		<org.aspectj-version>1.6.10</org.aspectj-version>
  		<org.slf4j-version>1.6.6</org.slf4j-version>
  	</properties>
  ```

- servlet-api 버젼 변경

  ```java
  <dependency>
  			<groupId>javax.servlet</groupId>
  			<artifactId>javax.servlet-api</artifactId>
  			<version>3.0.1</version>
  			<scope>provided</scope>
  		</dependency>
  ```

- 프로젝트 속성
  - `project facets`버젼 변경
    - java: 1.8  web:3.0
    - compiler :1.8
  - 프로젝트 오류 확인

----

### controller 생성

- spring 설절 파일에 `<context:component-scan>`으로 컨트롤러를 추가할 패키지를 추가
- src에 패키지를 만들고 컨트롤러 추가
  - `@Controller `어노테이션 기호로 선언
- 요청할때 실행될 메소드 정의
  - `@RequestMapping`으로 실행될 요청 path를 등록
  - `return`될 객체를 명시
- `src/main/webapp/WEB-INF`폴더 아래 `view`를 만들기

---

### tiles프레임워크 적용

- 화면구성
  - 라이브러리를 pom.xml에 추가
  - 레이아웃이 적용되어 있는 템플릿파일과 연결환 jsp파일들이 미리 만들어져 있어야 한다.
  - tiles설정 파일 작성(tiles-config.xml)
    - 템플릿 등록 : 템플릿의 각영역을 나누고 영역게 연결해줄 jsp파일을 정의
  - 템플릿 
    - jsp파일에 나눠놓은 각 영역이 tiles설정 파일과 일치하도록 설정
    - tiles프레임워크에서 제공하는 태그를 쓰기위해 등록
    - 스프링내부에서 실행될때 `DispatcherServlet`이 뷰의 정보를 `viewResolver`에 전달하면 기존에는 컨트롤러에서 넘겨주는 뷰정보에 `perfix와 suffix`를 이용해서 뷰를 완성하는 방식
      - 뷰정보 : test/index
      - internalResourceViewResolver를 이용해서 뷰를 완성
    - 기존방식과 다르게 tiles프레임워크를 이용해서 뷰를 만들수있도록 스프링 설정 파일에 등록
      - tiles설정 파일이 어떤 파일인지 등록
      - 만들어야 할 뷰의 정보가 tiles뷰임을 등록
    - 템플릿을 활용해서 어떤 뷰를 만들 것인지 tiles설정 파일에 등록
      - `<definition name="index" extends="mainTemplate">`
      - name 속성 : controller에서 사용할 뷰의 이름
      - extends속성 :  tiles설정파일에 등록한 템플릿의 이름

----

### 작업순서

**1. spring mvc project**

**- po**[**m.xml에서**](http://m.xn--xml-k94n91q/) **버전바꾸기**

**- project facets에서 버전바꾸기**

**2. 에러 없이 실행되는거 확인**

**3. 첨부된 erp.zip파일의 압축을 풀고 폴더 배치**

**- res폴더의 하위 폴더는 resources하위로**

**- view폴더의 하위 폴더들은 WEB-INF의 하위 boardlist.jsp에러 발생!!!!**

**=> tiles라이브러리가 추가되기 전에 사용 하고 있기 때문에 발생**

**4. po**[**m.xml에**](http://m.xn--xml-568n/) **tiles라이브러리 추가하기**

**5. /WEB-INF/spring/appServlet/servlet-context.xml을**

**/WEB-INF/config로 이동하고 파일명 spring-config.xml로변경하기** 

**6. web.xml파일을 열고 스프링설정파일 경로 변경하기**

**7. tiles-config.xml설정파일을 생성하고 블로그에 명시되어 있는대로**

**템플릿등록하기**

**8. /WEB-INF/layout/index.jsp와 /WEB-INF/layout/mainLayout.jsp를**

**열고 템플릿에 등록한 영역의 이름을 <tiles:insertAttribute>로 추가**

**9. spring-config.xml파일을 열고 tiles로 뷰를 만들도록 등록하기**

**10. 이제 설정 작업 완료!!**

**서버를 restart하고 오류가 있는지 확인하기**

**오류가 없으면 이제 컨트롤러 만들고 연결하면 됩니다.**

**11. src/main/java에 컨트롤러 만들기**

**=> /WEB-INF/include/top.jsp를 열고 요청 path확인하고 없으면 등록**

**12. Controller를 작성하고 화면을 세 개 요청 할 것이므로** 

**메소드 3개를 정의하고 뷰를 리턴하도록 설정**

**=> top.jsp에 설정한 요청 path로 requestmapping을 등록**

**13. tiles-config.xml에 뷰를 등록**

**템플릿을 기반으로 등록하며 뷰의 이름은 컨트롤러 각 메소드에 정의한** 

**이름으로 등록하기**

**14. 실행해서 결과 확인하기**

---

### Mybatis

- DAO클래스에서 SQL을 분리 할수있도록 지원하는 프레임워크

- DAO에서 DB작업을 위해서 처리되던 중복된 내용을 모두 MYbatis에서 처리한다

- pom.xml에 의존모듈 추가

- Mybatis에서 사용할 설정 파일을 작성

  - mybatis메인 설정파일 : my batis를 사용하기위해서 필요한 내용을 정의

    ​                                           (`/WEB-INF/config/mybatis-config.xml`)

  - mapper : 자바코드로 부터 sql문을 분리하는 것이 목적

- spring설정파일에 등록

  - spring내부에서 mybatis를 사용하기 위해서 설정
    - connection객체를 관리하기 위한 spring의 클래스를 등록
      - wAS가 관리하는 Conection pool에서 DB연동을 하기위한 Connection을 받아서 관리할 수 있도록 스프링에서 제공되는 빈을 등록한다
    - spring에서 mybatis의 핵심 클래스인 sqlSession을 사용할 수 있도록 factory클래스 등록
      - sqlsession을 만들기 위해서 mybatis설정 파일의 정보를 넘겨준다.
    - mybatis핵심클래스인 sqlsession사용할수있도록 빈으로 등록
      - DB연동을 위한 기능을 제공하는 클래스
