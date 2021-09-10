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



### DOM(document object model)

- 문서를 접근하는 방법을 표준으로 정의해 놓은 것
- 플랫폼이나 언어에 상관없이 컨텐츠의  구조를 통적으로 업데이트하고 엑세스 할 수 있도록 w3c에서 표준으로 정의해 놓은 문서 접근 방법
- `word wide web consortium` : 브라우저 내부에 포함된 html이나 css명세에 따라서 html문서를 해석하는데 이것을 w3c에서 정한다
- Dom구성요소
  - document : dom객체에서 가장 상위 객체
  - element :  html문서를 구성하는 모든 컨텐츠
  - attribute : 태그내부에 정의되어 있는 속성
  - text : 태그와 태그사이에 입력한 문자열 혹은  공백도 문자열 객체로 인식
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

