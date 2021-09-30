# web 실습

### 회원가입 

```html
<!DOCTYPE html>
<html>
<head>
<meta charset="UTF-8">
<title>회원가입</title>
</head>
<body>
<table border="1"  width="330"  height="300">
		
				<tr align="center">
				<td colspan="3">회원가입</td>
				</tr>
				
				<tr >
	            <td>이름</td>
	            <td colspan="2"> <input type="text"  size="15"  maxlength="5"  name="name" /></td>
				</tr>
				
				<tr >
	            <td> 사용자ID</td>
	            <td colspan="2"> <input type="text"  size="15"  maxlength="10"  name="id" /></td>
				</tr>
				
				<tr >
	            <td> 암호</td>
	            <td colspan="2"><input type="password"  size="15"  maxlength="15"   name="pass"/></td>
				</tr>
				
				<tr >
	            <td> 암호확인</td>
	            <td colspan="2"> <input type="password"  size="15"  maxlength="15"   name="passreward"/></td>
				</tr>
				
				<tr >
	            <td> 주민등록번호</td>
	            <td colspan="2">  <input type="text"  size="6"  maxlength="6"  name="admis1" />&nbsp;<input type="text"  size="6"  maxlength="6"  name="admin2" /></td>
				</tr>
				
				<tr >
	            <td> 전화번호</td>
	            <td colspan="2"> <input type="text"  size="4"  maxlength="4"  name="num1" />-<input type="text"  size="4"  maxlength="4"  name="num2" />-<input type="text"  size="4"  maxlength="4"  name="num3" /></td>
				</tr>
				
				<tr >
	            <td> 성별</td>
	            <td colspan="2"><input type="radio" name="성별" value="남자">남자 <input type="radio" name="성별" value="여자">여자</td>
				</tr>
				
				<tr >
	            <td>직업</td>
	            <td colspan="2">	
	            <select >
	             <option value="선택하여주십시오">선택하여주십시오</option>
	             <option value="웹디자이너">웹디자이너</option>
	             <option value="개발자">개발자</option>
	             <option value="빅데이터개발자">빅데이터개발자</option>
	             <option value="DBA">DBA</option>
	             <option value="임베디드개발자">임베디드개발자</option> 
	             </select> </td>
				</tr>
				
				<tr >
	            <td> email주소</td>
	            <td colspan="2">  <input type="text"  size="20"  maxlength="20"  name="email" /></td>
				</tr>
				
				<tr align="center">
				<td colspan="3">
				<input type="submit" value="가입신청">
				<input type="reset" value="취소">
				</td>
				</tr>
				
				</table>
</body>
</html>
```

### CSS - table작성

```html
<!--  mytable
@charset "UTF-8";
		table{
			           border-collapse: collapse;
			           text-align: center;
			           border-color: #a8ca40;
			           width: 500px;
			}
		th,td{
	font-size: 9pt;
	border:  solid 1px  #a8ca40;
	height: 20px
}
			tr:hover{
						background-color: skyblue;
			}
			th{
					color: white;
					background-color: #a8ca40;
			}
             .m1{
                      background-color: #eef4d6;
                      
             } -->

<!DOCTYPE html>
<html>
<head>
<meta charset="UTF-8"/>
<title>Insert title here</title>
<link rel="stylesheet"  type="text/css"  href="../common/css/mytable.css"/>
</head>
<body>
	<table border="1">
		<caption>가장 즐겨듣는 15곡 연주 목록</caption>
		<thead>
		<tr >
			<th>순위</th>
			<th>곡명</th>
			<th>가수명</th>
			<th>앨범</th>
		</tr>
		</thead>
		<tbody>
		<tr class="m1">
				<td>1</td>
				<td>소리쳐</td>
				<td>이승철</td>
				<td>Reflection of Sound</td>
			</tr>
			<tr>
				<td>2</td>
				<td>겨울비는내리고</td>
				<td>김범룡</td>
				<td>김범룡1집</td>
			</tr>

			<tr class="m1">
				<td>3</td>
				<td>거리에서</td>
				<td>성시경</td>
				<td>The Ballads</td>
			</tr>

			<tr>
				<td>4</td>
				<td>알 수 없는 인생</td>
				<td>이문세</td>
				<td>발칙한 여자들 OST</td>
			</tr>

			<tr class="m1">
				<td>5</td>
				<td>사랑안해</td>
				<td>백지영</td>
				<td>Thank You I Can Smile Again</td>
			</tr>

			<tr>
				<td>6</td>
				<td>내 사람</td>
				<td>SG워너비</td>
				<td>Global Underground Moscow</td>
			</tr>

			<tr class="m1">
				<td>7</td>
				<td>그녀를 사랑해줘요</td>
				<td>하동균</td>
				<td>Aha Shake Heartbreak</td>
			</tr>

			<tr>
				<td>8</td>
				<td>남자를 몰라</td>
				<td>Buzz(버즈)</td>
				<td>The Precious History</td>
			</tr>

			<tr class="m1">
				<td>9</td>
				<td>겨울비는내리고</td>
				<td>김범룡</td>
				<td>김범룡</td>
			</tr>

			<tr>
				<td>10</td>
				<td>아이스크림</td>
				<td>MC몽</td>
				<td>The way I am</td>
			</tr>

			<tr class="m1">
				<td>11</td>
				<td>원하고 원망하죠</td>
				<td>이승기</td>
				<td>남자가 여자를 사랑할 때</td>
			</tr>

			<tr>
				<td>12</td>
				<td>I'm Coming</td>
				<td>비(Rain)</td>
				<td>4집</td>
			</tr>

			<tr class="m1">
				<td>13</td>
				<td>You and me</td>
				<td>자우림</td>
				<td>ashes to ashes - 6집</td>
			</tr>

			<tr>
				<td>14</td>
				<td>떠나지마</td>
				<td>이승철</td>
				<td>Reflection of Sound</td>
			</tr>

			<tr class="m1">
				<td>15</td>
				<td>하고 싶은 말</td>
				<td>김태우</td>
				<td>솔로 스페셜</td>
			</tr>
			</tbody>
	</table>
</body>
</html>
```

### 포지셔닝 실습

```html
<!DOCTYPE html>
<html>
<head>
<meta charset="UTF-8">
<title>Insert title here</title>
<style type="text/css">
				#m1{
				        position: absolute;
						width: 440px;
          				height: 440px;
          				background-color: none;
          				border-color: blue;
          				border-style: solid;
          				border-width: 15px;
          				top: 5px;
          				left: 500px;
          				z-index: 2;
				}
				#m2{
						 position: absolute;
						width: 250px;
          				height: 250px;
          				background-color: none;
          				border-color: green;
          				border-style: solid;
          				border-width: 15px;
          				top:50px;
          				left: 280px;
          				z-index: 1;
				}
				#m3{
						 position: absolute;
						width: 300px;
          				height: 300px;
          				background-color: none;
          				border-color: red;
          				border-style: solid;
          				border-width: 15px;
          				top:240px;
          				left: 40px;
          				z-index: 3;
				}
				#m4{
						 position: absolute;
						width: 300px;
          				height: 300px;
          				background-color: none;
          				border-color: yellow;
          				border-style: solid;
          				border-width: 15px;
          				top:500px;
          				left: 250px;
          				z-index: 4;
				}
				#m5{
						 position: absolute;
						 font-family: Arial;
						 font-size: 30pt;
						 font-weight: bolder;
          				top:600px;
          				left: 400px;
          				z-index: 5;
				}
				#m6{
						 position: absolute;
						 font-family: Arial Black;
						 font-size: 30pt;
						 font-weight: bolder;
          				top:630px;
          				left: 450px;
          				z-index: 5;
				}

</style>
</head>
<body>
<div id="m1"></div>
<div id="m2"></div>
<div id="m3"></div>
<div id="m4"></div>
<div id="m5">Microsoft</div>
<div id="m6">Internet Explorer</div>
</body>
</html>
```

### 계시판 생성 실습

```html
<!DOCTYPE html>
<html>
<head>
<meta charset="UTF-8"/>
<title>즐겨듣는 음악 계시판</title>
<style type="text/css">
		table{
			           border-collapse: collapse;
			           width: 600px;
			}
			th{
					color: #9fbcd9;
					background-color: white;
					border-top:  2px solid   #9fbcd9;
			}
			tr{
					  border-bottom : 1px solid   #9fbcd9;
					  cursor: pointer;
			}
			.a0{
					text-align: center;
			}
			.a1{
				background-color:   #f0faff;
				color: blue;
			}
			.m1{
					text-align: left;
			}
			.m2{
					text-align: center;
			}
			tr:hover{
						background-color: #f0faff;
			}
			.m1:hover {
							color:blue;
							text-decoration: underline;
			}
</style>
</head>
<body>
	<table border="0" >
		<thead>
		<tr class="a0">
			<th>순위</th>
			<th>곡명</th>
			<th>가수명</th>
			<th>앨범</th>
		</tr>
		</thead>
		<tbody>
		<tr >
				<td class="a1" colspan="4">참고</td>
			</tr>
			<tr class="a1">
				<td>공지</td>
				<td>  &nbsp;재밌게 들으세요</td>
				<td></td>
				<td></td>
			</tr>
		<tr >
				<td>1</td>
				<td class="m1">소리쳐</td>
				<td class="m2">이승철</td>
				<td class="m2">Reflection of Sound</td>
			</tr>
			<tr>
				<td>2</td>
				<td class="m1">겨울비는내리고</td>
				<td class="m2">김범룡</td>
				<td class="m2">김범룡1집</td>
			</tr>

			<tr >
				<td>3</td>
				<td class="m1">거리에서</td>
				<td class="m2">성시경</td>
				<td class="m2">The Ballads</td>
			</tr>

			<tr>
				<td>4</td>
				<td class="m1">알 수 없는 인생</td>
				<td class="m2">이문세</td>
				<td class="m2">발칙한 여자들 OST</td>
			</tr>

			<tr >
				<td>5</td>
				<td class="m1">사랑안해</td>
				<td class="m2">백지영</td>
				<td class="m2">Thank You I Can Smile Again</td>
			</tr>

			<tr>
				<td>6</td>
				<td class="m1">내 사람</td>
				<td class="m2">SG워너비</td>
				<td class="m2">Global Underground Moscow</td>
			</tr>

			<tr >
				<td>7</td>
				<td class="m1">그녀를 사랑해줘요</td>
				<td class="m2">하동균</td>
				<td class="m2">Aha Shake Heartbreak</td>
			</tr>

			<tr>
				<td>8</td>
				<td class="m1">남자를 몰라</td>
				<td class="m2">Buzz(버즈)</td>
				<td class="m2">The Precious History</td>
			</tr>

			<tr >
				<td>9</td>
				<td class="m1">겨울비는내리고</td>
				<td class="m2">김범룡</td>
				<td class="m2">김범룡</td>
			</tr>

			<tr>
				<td>10</td>
				<td class="m1">아이스크림</td>
				<td class="m2">MC몽</td>
				<td class="m2">The way I am</td>
			</tr>

			<tr >
				<td>11</td>
				<td class="m1">원하고 원망하죠</td>
				<td class="m2">이승기</td>
				<td class="m2">남자가 여자를 사랑할 때</td>
			</tr>

			<tr>
				<td>12</td>
				<td class="m1">I'm Coming</td>
				<td class="m2">비(Rain)</td>
				<td class="m2">4집</td>
			</tr>

			<tr >
				<td>13</td>
				<td class="m1">You and me</td>
				<td class="m2">자우림</td>
				<td class="m2">ashes to ashes - 6집</td>
			</tr>

			<tr>
				<td>14</td>
				<td class="m1">떠나지마</td>
				<td class="m2">이승철</td>
				<td class="m2">Reflection of Sound</td>
			</tr>

			<tr >
				<td>15</td>
				<td class="m1">하고 싶은 말</td>
				<td class="m2">김태우</td>
				<td class="m2">솔로 스페셜</td>
			</tr>
			</tbody>
	</table>

</body>
</html>
```

### 레이아웃 실습

```html
<!DOCTYPE html>
<html>
<head>
<meta charset="UTF-8">
  <title> New Document </title>
  <style type="text/css">
  				#header{
  	  				background-color: blue; 
  					}
  				#m0{
  					width: 95%;
  					margin-left: auto;
  					margin-right: auto;
  					text-align: justify;
  				}
  				#m1{
  				   width: 65%;
  				   float: right;
  				}	
  				#m2{
  					width:30%; 
  					float:right;
  					margin-left: 20px;
  					background-color: green; 
  				}	
  				#m3{
  					clear:both;
  					background-color: #cccc99;
  				}
</style>
</head>
 <body>
<div id="header">
			<h1>
			헤더 영역입니다.
			</h1>
</div>
<div id="m0">

<div id="m2"> <p >
			메뉴
			Nothing too complex, but still pretty cool right? Child’s play you say. Ok, well before we get into the part where floats usher in a world of bacon-loving unicorns, let’s back up for a second to talk about what’s actually happening here. In the web world, our HTML is bound by some rules, in particular, the normal flow. In the normal flow, each block element (div, p, h1, etc.) stacks on top of each other vertically, from the top of the viewport down. Floated elements are first laid out according to the normal flow, then taken out of the normal flow and sent as far to the right or left (depending on which value is applied) of the parent element. In other words, they go from stacking on top of each other to sitting next to each other, given that there is enough room in the parent element for each floated element to sit. This behavior is crucial to remember as you build your websites.
     </p> </div>	
     
	<div id="m1">
			<p>
			The float property is a valuable and powerful asset to any web designer/developer working with HTML and CSS. Tragically, it can also cause frustration and confusion if you don’t fully understand how it works. Also, in the past, it’s been linked to some pretty nasty browser bugs so it's normal to get nervous about using the float property in your CSS rule sets. Let’s calm those nerves and ease that frustration. I’ll show you exactly what the float property does to your elements and how incredibly useful it can be once you master it.
			</p>
			<p>
			We see floats in the print world every time we pick up a magazine article with an image on the left or right with text flowing nicely around it. In the world of HTML/CSS, text will wrap around an image with the float property applied to it, much like in a magazine layout. Images are just one of the many use cases for the float property: we can also achieve the popular two-column layout using floats. In fact, you can float just about any element in your HTML. By learning and understanding float property basics, along with position property basics, you will be able to achieve any layout with confidence.
			</p>
			<p>
			The float property has four values that we can apply to it: left, right, inherit, and none. Each value is pretty self explanatory. For example, if you assign float: left to an element, it will move to the left-most boundary of its parent element. The same idea applies if you were to assign float: right; to an element. That element would be sent off to the right-most boundary of its parent element. The inherit value tells an element to inherit the float value of its parent element. The value none is the default value and tells an element not to float at all.
	</p> </div>
</div>    

<div id="m3"> <p >
			푸터 영역입니다.
</p></div>
</body>
</html>

```

### function 연습

```html
<!DOCTYPE html>
<html>
	<head>
		<meta charset="UTF-8">
		<title>Insert title here</title>
		<script type="text/javascript">
			//1. printgugu() -> js_gugu_exam.html의 <body>태그 안에 정의한 내용을 function으로 작성하기
			function printgugu() {
				document.write("<table border='1'>");
				for(dan = 1;dan<=9;dan++) {
					document.write("<tr>")
					for(i = 1;i<=9;i++) {
						if(dan==i){
							document.write("<td bgColor='yellow'>"+dan+"*"+i+"="+(dan*i)+"</td>");
						}else{
							document.write("<td>"+dan+"*"+i+"="+(dan*i)+"</td>");	
						}
						
					}
					document.write("</tr>")
				}
				document.write("</table>");
			}
			//2. print() -> function내부에서 출력할 단을 prompt로 입력받고 구구단을  document.write로 출력하는 함수를 정의
			function printdan() {
				dan = prompt("단을 입력")
					for(i = 1; i<=9; i++) {
						document.write(dan+"*"+i+"="+(dan*i)+"<br/>");
						}		
					}
			//3. calc() -> 숫자2개를 입력받고 연산자를 입력받아서 입력받은 숫자에 대해서 선택한 연산을 적용해서 결과를 alert으로 출력하기
			//    => Calc.java를 참고, promt 를 세 개를 이용해서 값을 입력받기
			function calc() {
				opr = prompt('연산자 입력');
				num1 = parseInt(prompt("숫자1 입력"));
				num2 = parseInt(prompt("숫자2 입력"));
				result = 0;
				switch(opr)  {
					case "+":
						result = num1+num2;
					break;
					case "-":
						result = num1-num2;
						break;
					case "*":
						result = num1*num2;
						break;
					case "/":
						result = num1/num2;
						break;
				}
				alert("계산결과  > " +result);
			}
			//4. hapTest(num) -> 1부터 매개변수로 전달받은 숫자까지의 합을 구해서 리턴하기
			function hapTest(num) {
				result = 0;
				for(i=1;i<=num;i++){
					result = result+i;
				}
				return result;
			}
		</script>
	</head>
	<body>
		<input type="button" value="전체구구단 출력" onclick="printgugu()">
		<input type="button" value="입력받은 단을 구구단으로 출력하기" onclick="printdan()">
		<input type="button" value="연산하기" onclick="calc()">
		<script type="text/javascript">
			//숫자를 입력받아서 1부터 입력받은 수까지의 합을 구하는 함수를 호출하여 매개변수로 숫자를 전달하고
			//리턴받은 값을 alert으로 출력하기
			//-> hapTest함수를 호출해서 결과를 완성하기
			mynum = parseInt(prompt("숫자입력"));
			returnVal  = hapTest(mynum);
			alert("함수결과 > "+returnVal);
		</script>
	</body>
</html>
```

### 로그인 시스템

```html
<!DOCTYPE html>
<html>
<head>
<meta charset="UTF-8">
<title>Insert title here</title>
			<script type="text/javascript">
							function rel(form) {
								data = form.id.value;
								if(data.length<4) {
									myrel = "4글자 이상의 글자를 입려하세요"
									document.getElementById("val").innerHTML = myrel;
								} else {
									if(data=="java"){
										myrel0 ="이미 사용중인 아이디 입니다."
										document.getElementById("val").innerHTML = myrel0;
									}else{
									myrel2 ="사용가능한 아이디 입니다."
									document.getElementById("val").innerHTML = myrel2;
									}
								} 
							}
			</script>
</head>
<body>
	<h1>티몬 회원가입</h1>
		<h2>필수항목</h2>
			<form  name = "myform">
					아이디 : <input type="text" name="id"  onkeyup="rel(this.form)" >
			</form>
					<div id="val" style="color : red"></div>
</body>
</html>
```



### web 제작

```html
<!--메인 페이지-->
<!DOCTYPE html>
<html lang="en">
<head>
  <title>Bootstrap Example</title>
  <meta charset="utf-8">
  <meta name="viewport" content="width=device-width, initial-scale=1">
  <link rel="stylesheet" href="https://maxcdn.bootstrapcdn.com/bootstrap/3.4.1/css/bootstrap.min.css">
  <script src="https://ajax.googleapis.com/ajax/libs/jquery/3.5.1/jquery.min.js"></script>
  <script src="https://maxcdn.bootstrapcdn.com/bootstrap/3.4.1/js/bootstrap.min.js"></script>
  <style>
    .navbar {
      margin-bottom: 0;
      border-radius: 0;
    }
    
    .row.content {height: 450px}
    
    .sidenav {
      padding-top: 20px;
      background-color: #f1f1f1;
      height: 100%;
    }
    
    footer {
      background-color: #555;
      color: white;
      padding: 15px;
    }
    
    @media screen and (max-width: 767px) {
      .sidenav {
        height: auto;
        padding: 15px;
      }
      .row.content {height:auto;} 
    }
  </style>
</head>
<body>

<nav class="navbar navbar-inverse">
  <div class="container-fluid">
    <div class="navbar-header">
      <button type="button" class="navbar-toggle" data-toggle="collapse" data-target="#myNavbar">
        <span class="icon-bar"></span>
        <span class="icon-bar"></span>
        <span class="icon-bar"></span>                        
      </button>
      <a class="navbar-brand" >###</a>
    </div>
    <div class="collapse navbar-collapse" id="myNavbar">
      <ul class="nav navbar-nav">
        <li class="active"><a href="http://localhost:8088/clientweb/bootstrap/task/site_making.html#">Home</a></li>
        <li><a href="#">전체글</a></li>
        <li><a href="http://localhost:8088/clientweb/bootstrap/task/site_making2.html">가입인사</a></li>
        <li><a href="#">자유게시판</a></li>
        <li><a href="#">정보</a></li>
        <li><a href="#">후기</a></li>
        <li><a href="#">Q&A</a></li>
        <li><a href="#">공지사항</a></li>
      </ul>
      <ul class="nav navbar-nav navbar-right">
        <li><a href="#"><span class="glyphicon glyphicon-log-in"></span> Login</a></li>
      </ul>
    </div>
  </div>
</nav>
  
<div class="container-fluid text-center">    
  <div class="row content">
    <div class="col-sm-1 sidenav">
      <p><a href="https://www.musinsa.com/" > 무신사</a></p>
      <p><a href="https://kream.co.kr/">KREAM</a></p>
    </div>
    <div class="col-sm-8 text-left"> 
    <div class="row">
				<div id="myCarousel" class="carousel slide" data-ride="carousel">
					  <ol class="carousel-indicators">
						    <li data-target="#myCarousel" data-slide-to="0" class="active"></li>
						    <li data-target="#myCarousel" data-slide-to="1"></li>
						    <li data-target="#myCarousel" data-slide-to="2"></li>
					  </ol>
					  <div class="carousel-inner">
					    <div class="item active">
					      <img src="../../images/p1.jpg" style="width:100%;  height:300px">
					    </div>
					
					    <div class="item">
					      <img src="../../images/p2.jpg" style="width:100%;  height:300px">
					    </div>
					
					    <div class="item">
					      <img src="../../images/p3.png" style="width:100%;  height:300px">
					    </div>
					  </div>
					
      <h1>comunity</h1>
      <p>패션 관련 커뮤니티입니다.</p>
      <hr>

       <a class="left carousel-control" href="#myCarousel" data-slide="prev">
					    <span class="glyphicon glyphicon-chevron-left"></span>
					    <span class="sr-only">Previous</span>
					  </a>
					  <a class="right carousel-control" href="#myCarousel" data-slide="next">
					    <span class="glyphicon glyphicon-chevron-right"></span>
					    <span class="sr-only">Next</span>
					  </a>
    </div>
    </div>
    </div>
    <div class="col-lg-2 sidenav">
      <div class="well">
         <img src="../../images/u.jpg" width="100%" height="200">
      </div>
      <div class="well">
        <img src="../../images/k.jpg" width="100%" height="200">
        
      </div>
    </div>
  </div>
</div>
</body>
</html>

<!--가입인사 페이지-->
<div class="jumbotron">
  <div class="container text-center">
    <h1>가입인사</h1>      
    <p>처음 방문해주신 분들은 필히 작성부탁드립니다.</p>
  </div>
</div>
  
<div class="container-fluid bg-3 text-center">    
  <h3>새로오신분</h3><br>
  <div class="row">
    <div class="col-sm-3">
      <p>원빈</p>
      <img src="../../images/a1.jpg" class="img-responsive" style="width:100%" alt="Image">
    </div>
    <div class="col-sm-3"> 
      <p>정우성</p>
      <img src="../../images/a2.jpg" class="img-responsive" style="width:100%" alt="Image">
    </div>
    <div class="col-sm-3"> 
      <p>강동원</p>
      <img src="../../images/a3.jpg" class="img-responsive" style="width:100%" alt="Image">
    </div>
    <div class="col-sm-3">
      <p>이나영</p>
      <img src="../../images/a4.jpg" class="img-responsive" style="width:100%" alt="Image">
    </div>
  </div>
</div><br>

</body>
</html>

```

### 오라클 연동

```java
package jdbc;

import java.sql.Connection;
import java.sql.DriverManager;
import java.sql.SQLException;
import java.sql.Statement;

public class updateTest {
	public static void main(String[] args) {
		
		String url = "jdbc:oracle:thin:@ip주소:포트:xe";
		String user = "scott";
		String password = "tiger";
		String sql = "update member set addr ='서울특별시' where addr ='서울'";
		try {
		Class.forName("oracle.jdbc.driver.OracleDriver");
		System.out.println("driver succes");
		Connection con = DriverManager.getConnection(url,user,password);
		System.out.println("Connection succes");
		Statement stmt = con.createStatement();
		System.out.println("statement succes");
		int result = stmt.executeUpdate(sql);
		System.out.println("result succes");
		}catch(ClassNotFoundException e) {
			e.printStackTrace();
		} catch (SQLException e) {
			e.printStackTrace();
		}
	}
}

```

### DBMS연동 

```java
//DButil
import java.sql.Connection;
import java.sql.DriverManager;
import java.sql.ResultSet;
import java.sql.SQLException;
import java.sql.Statement;

public class DBUtil {
	static {
		try {
			Class.forName("oracle.jdbc.driver.OracleDriver");
		} catch (ClassNotFoundException e) {
			e.printStackTrace();
		}
	}
	public static Connection getConnect() {
		String url = "jdbc:oracle:thin:@ip:1521:xe";
		String user = "scott";
		String password = "tiger";
		Connection con = null;
		try {
			con = DriverManager.getConnection(url,user,password);
		} catch (SQLException e) {
			e.printStackTrace();
		}
		return con;
	}
	
	public static void close(ResultSet rs, Statement stmt, Connection con) {
		try {
			if(rs!=null) rs.close();
			if(stmt!=null) stmt.close();
			if(con!=null) con.close();
		} catch (SQLException e) {
			e.printStackTrace();
		}
	}
	public static void close(Connection con) {
		try {
			if(con!=null) con.close();
		} catch (SQLException e) {
			e.printStackTrace();
		}
	}
}

//memberDAO	
import java.sql.Connection;
import java.sql.DriverManager;
import java.sql.PreparedStatement;
import java.sql.ResultSet;
import java.sql.SQLException;
import java.sql.Statement;
import java.util.ArrayList;

public class MemberDAO {
	public int insert(MemberDTO user) {
		System.out.println("웹페이지에 사용자가 입력한 데이터:"+user); 
		String sql = "insert into member values(?,?,?,?,1000,?)";
		Connection con = null;
		PreparedStatement stmt = null;		
		int result = 0;
		try {			
			con = DBUtil.getConnect();
			stmt = con.prepareStatement(sql);			
			stmt.setString(1, user.getId());
			stmt.setString(2, user.getPass());
			stmt.setString(3, user.getName());
			stmt.setString(4, user.getAddr());
			stmt.setString(5, user.getDeptno());
				
			result = stmt.executeUpdate();
			System.out.println(result+"개 행 삽입성공");
		} catch (SQLException e) {
			e.printStackTrace();
		}finally {
			DBUtil.close(null, stmt, con);
		}
		return result;
	}
	public int insert(String id, String pass, String name, String addr, String deptno) {
		String sql = "insert into member values(?,?,?,?,1000,?)";
		Connection con = null;
		PreparedStatement stmt = null;			
		int result = 0;
		try {			
			con = DBUtil.getConnect();
			stmt = con.prepareStatement(sql);			
			stmt.setString(1, id);
			stmt.setString(2, pass);
			stmt.setString(3, name);
			stmt.setString(4, addr);
			stmt.setString(5, deptno);
				
			 result = stmt.executeUpdate();
			System.out.println(result+"개 행 삽입성공");
		} catch (SQLException e) {
			e.printStackTrace();
		}finally {
			DBUtil.close(null, stmt, con);
		}
		return result;
	}

	public void update(String id,  String addr) {
		String sql = "update member ";
		sql = sql+"set addr=? ";
		sql = sql+"where id=?";
		Connection con = null;
		PreparedStatement stmt = null;
		try {
			con = DBUtil.getConnect();
			stmt = con.prepareStatement(sql);	
			stmt.setString(1, addr);
			stmt.setString(2, id);
			System.out.println("Statement객체 생성완료" + stmt);
			int result = stmt.executeUpdate();
			System.out.println(result+"개 행 수정성공");
		} catch (SQLException e) {
			e.printStackTrace();
		}finally {
			DBUtil.close(null,stmt,con);
		}	
	}
	
	public int delete(String id) {
		StringBuffer sql = new StringBuffer();
		sql.append("delete from member ");
		sql.append("where id=? ");
		Connection con = null;
		PreparedStatement stmt = null;
		int result = 0;
		try {
			con = DBUtil.getConnect();
			System.out.println("커넥션성공!"+ con);
			stmt = con.prepareStatement(sql.toString());
			stmt.setString(1, id);
			System.out.println("Statement객체 생성완료" + stmt);
			 result =  stmt.executeUpdate();
			System.out.println(result+"개 행 삭제성공");
		} catch (SQLException e) {
			e.printStackTrace();
		}finally {
			DBUtil.close(null, stmt,con);
		}
		return result;
	}
	
	public ArrayList<MemberDTO> getMemberList() {
		System.out.println("dao요청");
		ArrayList<MemberDTO> userlist = new ArrayList<MemberDTO>();
		MemberDTO user = null;
		StringBuffer sql = new StringBuffer();
		sql.append("select * from member");	
		Connection con = null;
		Statement stmt = null;
		ResultSet rs = null;
		try {
			con = DBUtil.getConnect();
			stmt = con.createStatement();
			rs = stmt.executeQuery(sql.toString());
			while(rs.next()) {
				user = new MemberDTO(rs.getString(1),rs.getString(2),rs.getString(3),rs.getString(4),rs.getInt(5),rs.getString(6));
				userlist.add(user);
			}	
			System.out.println("조회성공");
		} catch (SQLException e) {
			e.printStackTrace();
		}finally {
			DBUtil.close(rs, stmt, con);
		}
		return userlist;
	}
	
	public ArrayList<MemberDTO>search(String search) {
		System.out.println("dao search 요청 : "+search);
		ArrayList<MemberDTO> userlist = new ArrayList<MemberDTO>();
		MemberDTO user = null;
		StringBuffer sql = new StringBuffer();
		sql.append("select * from member where addr like ? ");	
		Connection con = null;
		PreparedStatement stmt = null;
		ResultSet rs = null;
		try {
			con = DBUtil.getConnect();
			stmt = con.prepareStatement(sql.toString());
			stmt.setString(1,  "%"+search+"%");
			rs = stmt.executeQuery();
			while(rs.next()) {
				user = new MemberDTO(rs.getString(1),rs.getString(2),rs.getString(3),rs.getString(4),rs.getInt(5),rs.getString(6));
				userlist.add(user);
			}	
			System.out.println("dao >>>>"+userlist.size());
		} catch (SQLException e) {
			e.printStackTrace();
		}finally {
			DBUtil.close(rs, stmt, con);
		}
		return userlist;
	}
	
	public MemberDTO read(String id) {
		System.out.println("da0 >>>>>" +id);
		MemberDTO user = null;
		StringBuffer sql = new StringBuffer();
		sql.append("select * from member where id like ? ");	
		Connection con = null;
		PreparedStatement stmt = null;
		ResultSet rs = null;
		try {
			con = DBUtil.getConnect();
			stmt = con.prepareStatement(sql.toString());
			stmt.setString(1,  id);
			rs = stmt.executeQuery();
			while(rs.next()) {
				user = new MemberDTO(rs.getString(1),rs.getString(2),rs.getString(3),rs.getString(4),rs.getInt(5),rs.getString(6));
			}	
		} catch (SQLException e) {
			e.printStackTrace();
		}finally {
			DBUtil.close(rs, stmt, con);
		}
		return user ;		
	}
}

//memberDTO
public class MemberDTO {
	private String id; 
	private String pass;
	private String name;
	private String addr;
	private int point;
	private String deptno;
	public MemberDTO() {
		
	}
	public MemberDTO(String id, String addr) {
		super();
		this.id = id;
		this.addr = addr;
	}
	public MemberDTO(String id, String pass, String name, String addr, String deptno) {
		super();
		this.id = id;
		this.pass = pass;
		this.name = name;
		this.addr = addr;
		this.deptno = deptno;
	}
	public MemberDTO(String id, String pass, String name, String addr, int point, String deptno) {
		super();
		this.id = id;
		this.pass = pass;
		this.name = name;
		this.addr = addr;
		this.point = point;
		this.deptno = deptno;
	}	
	public String toString() {
		return "MemberDTO [id=" + id + ", pass=" + pass + ", name=" + name + ", addr=" + addr + ", point=" + point
				+ ", deptno=" + deptno + "]";
	}

	public String getId() {
		return id;
	}
	public void setId(String id) {
		this.id = id;
	}
	public String getPass() {
		return pass;
	}
	public void setPass(String pass) {
		this.pass = pass;
	}
	public String getName() {
		return name;
	}
	public void setName(String name) {
		this.name = name;
	}
	public String getAddr() {
		return addr;
	}
	public void setAddr(String addr) {
		this.addr = addr;
	}
	public int getPoint() {
		return point;
	}
	public void setPoint(int point) {
		this.point = point;
	}
	public String getDeptno() {
		return deptno;
	}
	public void setDeptno(String deptno) {
		this.deptno = deptno;
	}	
}

//regist.html
<!DOCTYPE html>
<html>
<head>

<meta charset="UTF-8">
<title>Insert title here</title>
  <meta name="viewport" content="width=device-width, initial-scale=1">
  <link rel="stylesheet" href="https://maxcdn.bootstrapcdn.com/bootstrap/3.4.1/css/bootstrap.min.css">
  <link href="https://fonts.googleapis.com/css?family=Montserrat" rel="stylesheet">
  <script src="https://ajax.googleapis.com/ajax/libs/jquery/3.5.1/jquery.min.js"></script>
  <script src="https://maxcdn.bootstrapcdn.com/bootstrap/3.4.1/js/bootstrap.min.js"></script>
</head>
<body>
	<div class="container-fluid">
			<form role="form" class="form-horizontal" action="/serverweb/member/insert.do" method="POST"  name="myform">
				<fieldset>
					<div id="legend">
						<legend>아래 양식을 작성해주세요.</legend>
					</div>
					<div class="form-group">
						<!-- 부서코드 -->
						<label class="control-label col-sm-2" for="orgcode">부서코드</label>
						<div class="col-sm-3">
							<input type="text" id="orgcode" name="deptno"
								placeholder="부서코드" class="form-control"
								 required>
						</div>
					</div>
					
					<div class="form-group">
						<!-- 성명-->
						<label class="control-label col-sm-2" for="orgname">성명</label>
						<div class="col-sm-3">
							<input type="text" id="orgname" name="name"
								placeholder="성명" class="form-control" minlength="2">

						</div>
					</div>
					<div class="form-group">
						<!-- 사번-->
						<label class="control-label col-sm-2" for="id">사번</label>
						<div class="col-sm-3">
							<input type="text" id="id" name="id"
								placeholder="사번" class="form-control" 
								minlength="4" required onkeyup="runAjax()">
							
						</div>
						<span id="checkVal"></span>
					</div>
					
					<div class="form-group">
						<!-- 패스워드-->
						<label class="control-label col-sm-2" for="pass">패스워드</label>
						<div class="col-sm-3">
							<input type="text" id="pass" name="pass"
								placeholder="패스워드" class="form-control" minlength="4" >

						</div>
					</div>
					<div class="form-group">
						<!-- 주소-->
						<label class="control-label col-sm-2" for="addr">주소</label>
						<div class="col-sm-3">
							<input type="text" id="addr" name="addr" 
							placeholder="주소"
								class="form-control" minlength="3" required>

						</div>
					</div>
					<!-- <div class="form-group">
						포인트
						<label class="control-label col-sm-2" for="point">포인트</label>
						<div class="col-sm-3">
							<input type="text" id="point" name="point" 
							placeholder="포인트"
								class="form-control" minlength="4" required>

						</div>
					</div> -->
					
					<div class="form-group">
						<!-- Button -->
						<div class="col-sm-3 col-sm-offset-2">
							<input type="submit" value="가입하기" class="btn btn-success"/>
						</div>
						<a href="/serverweb/member/search.do?action=LIST">회원목록조회</a>
					</div>
				</fieldset>
			</form>
	</div>
</body>
</html>

//search.html
<!DOCTYPE html>
<html>
		<head>
		<meta charset="UTF-8">
<title>Insert title here</title>
		</head>
			<body>
				<form method="post" action="/serverweb/member/search.do?action=SEARCH">
					검색:
						<select name="category">
							<option value="id">아이디</option>
							<option value="name">이름</option>
							<option value="addr">주소</option>
							<option value="deptno">부서</option>
						</select>
							<input type="text"  name="search">
							<input type="submit" value="검색">
				</form>
			</body>
</html>
                            
//search &list servlet                            
import java.io.IOException;
import java.io.PrintWriter;
import java.util.ArrayList;

import javax.servlet.RequestDispatcher;
import javax.servlet.ServletException;
import javax.servlet.annotation.WebServlet;
import javax.servlet.http.HttpServlet;
import javax.servlet.http.HttpServletRequest;
import javax.servlet.http.HttpServletResponse;

import member.MemberDAO;
import member.MemberDTO;

@WebServlet(name = "search", urlPatterns = { "/member/search.do" })
public class MemberSearchServlet extends HttpServlet {
	
	protected void doGet(HttpServletRequest req, HttpServletResponse resp) throws ServletException, IOException {
		doPost(req, resp);
	}
	protected void doPost(HttpServletRequest request, HttpServletResponse response) throws ServletException, IOException {
		request.setCharacterEncoding("UTF-8");
		//클라이언트 요청정보 추출
		String action = request.getParameter("action");
		MemberDAO dao = new MemberDAO();
		ArrayList<MemberDTO> userlist =  null;
		if(action.equals("SEARCH")) {
			String addr = request.getParameter("search");
			userlist = dao.search(addr);
		}else {
				userlist = dao.getMemberList();
		}
		//데이터공유
		request.setAttribute("userlist", userlist);
		//요청재지정
		RequestDispatcher rd = request.getRequestDispatcher("/member/list.jsp");
		rd.forward(request, response);
	}

}

 //insert servlet
import java.io.IOException;
import java.io.PrintWriter;

import javax.servlet.ServletException;
import javax.servlet.annotation.WebServlet;
import javax.servlet.http.HttpServlet;
import javax.servlet.http.HttpServletRequest;
import javax.servlet.http.HttpServletResponse;

import member.MemberDAO;
import member.MemberDTO;

@WebServlet(name = "memberInsert", urlPatterns = { "/member/insert.do" })
public class MemberInsertServlet extends HttpServlet {
	protected void doPost(HttpServletRequest request, HttpServletResponse response) throws ServletException, IOException {
		request.setCharacterEncoding("UTF-8");
		response.setContentType("text/html;charset=UTF-8");
		
		String deptno = request.getParameter("deptno");
		String name = request.getParameter("name");
		String id = request.getParameter("id");
		String pass = request.getParameter("pass");
		String addr = request.getParameter("addr");
		
		MemberDTO user = new MemberDTO(id ,pass, name, addr, deptno);
		MemberDAO dao = new MemberDAO();
		int result = dao.insert(user);
		
		PrintWriter out = response.getWriter();
		if(result >=1 ) {
			out.print("<h2>삽입성공</h2>");
		}else {
			out.print("<h2>삽입실패</h2>");
		}
	}
}                
  
 //delete servlet               
import java.io.IOException;
import java.io.PrintWriter;

import javax.servlet.ServletException;
import javax.servlet.annotation.WebServlet;
import javax.servlet.http.HttpServlet;
import javax.servlet.http.HttpServletRequest;
import javax.servlet.http.HttpServletResponse;

import member.MemberDAO;
import member.MemberDTO;

@WebServlet(description = "memberDelete", urlPatterns = { "/member/delete.do" })
public class MemberDeleteServer extends HttpServlet {
	protected void doGet(HttpServletRequest request, HttpServletResponse response) throws ServletException, IOException {
		request.setCharacterEncoding("UTF-8");
		response.setContentType("text/html;charset=UTF-8");
		PrintWriter out = response.getWriter();
		
		String id = request.getParameter("id");
		System.out.println(id);
		
		MemberDAO dao = new MemberDAO();
		int result = dao.delete(id);
				
		  if(result >0) { out.print("<h2>삭제성공</h2>"); }else {
		  out.print("<h2>삭제실패</h2>"); }	
	}
}
     
//read servlet
import java.io.IOException;
import java.io.PrintWriter;

import javax.servlet.RequestDispatcher;
import javax.servlet.ServletException;
import javax.servlet.annotation.WebServlet;
import javax.servlet.http.HttpServlet;
import javax.servlet.http.HttpServletRequest;
import javax.servlet.http.HttpServletResponse;

import member.MemberDAO;
import member.MemberDTO;

@WebServlet(description = "memberRead", urlPatterns = { "/member/read.do" })
public class MemberReadServer extends HttpServlet {
	protected void doGet(HttpServletRequest request, HttpServletResponse response) throws ServletException, IOException {
		request.setCharacterEncoding("UTF-8");
		response.setContentType("text/html;charset=UTF-8");
		PrintWriter out = response.getWriter();
		
		String id = request.getParameter("id");
		System.out.println(id);
		
		MemberDAO dao = new MemberDAO();
		MemberDTO dto = dao.read(id);
		System.out.println("dao >>>>>" +id);		
		
		request.setAttribute("user", dto);
		
		RequestDispatcher rd = request.getRequestDispatcher("/member/member_read.jsp");
		rd.forward(request, response);
	}
}  

//member_read.jsp
<%@ page language="java" contentType="text/html; charset=UTF-8"
    pageEncoding="UTF-8" import="member.MemberDTO"%>

<!DOCTYPE html>
<html>
<head>
<meta charset="UTF-8">
<title>Insert title here</title>
 <link rel="stylesheet" href="http://maxcdn.bootstrapcdn.com/bootstrap/3.3.6/css/bootstrap.min.css">
  <script src="https://ajax.googleapis.com/ajax/libs/jquery/1.12.0/jquery.min.js"></script>
  <script src="http://maxcdn.bootstrapcdn.com/bootstrap/3.3.6/js/bootstrap.min.js"></script>
</head>
<body>
		<%
				MemberDTO user = (MemberDTO)request.getAttribute("user");
		%>

	<div class="container-fluid">
			<form role="form" class="form-horizontal"
		action="/serverweb/action?deptno=<%= "001" %>&state=UPDATE" 
		method="get">
				<fieldset>
					<div id="legend">
						<legend>아래 양식을 작성해주세요.</legend>
					</div>
					<div class="form-group">
						<!-- 부서코드 -->
						<label class="control-label col-sm-2" for="deptcode">부서코드</label>
						<div class="col-sm-3">
						<%= user.getDeptno() %>	
						</div>
					</div>
					
					<div class="form-group">
						<!-- 부서명-->
						<label class="control-label col-sm-2" for="name">성명</label>
						<div class="col-sm-3">
							<!-- 성명을 이곳에 출력하세요 -->
							<%= user.getName() %>
							
						</div>
					</div>					
					<div class="form-group">
						<!-- 아이디-->
						<label class="control-label col-sm-2" for="id">아이디</label>
						<div class="col-sm-3">
							<!-- 아이디를 이곳에 출력하세요 -->
							<%= user.getId() %>
						</div>
					</div>
					<div class="form-group">
						<!-- 주소-->
						<label class="control-label col-sm-2" for="addr">주소</label>
						<div class="col-sm-3">
							<!-- 주소를 이곳에 출력하세요 -->
							<%= user.getAddr() %>
						</div>
					</div>

					<div class="form-group">
						<!-- 패스워드-->
						<label class="control-label col-sm-2" for="hiredate">패스워드</label>
						<div class="col-sm-3">
							<!-- 패스워드를 이곳에 출력하세요 -->
							<%= user.getPass() %>
						</div>
					</div>
					<div class="form-group">
						<!-- 포인트-->
						<label class="control-label col-sm-2" for="point">포인트</label>
						<div class="col-sm-3">
							<!-- 포인트를 이곳에 출력하세요 -->
							<%= user.getPoint() %>
						</div>
					</div>
				
					<div class="form-group">
						<!-- Button -->
						<div class="col-sm-3 col-sm-offset-2">
							<input type="button"
							 value="수정" class="btn btn-success"/>
						</div>
					</div>
				</fieldset>
			</form>
	</div>
</body>
</html>
                                 
//list.jsp        
<%@page import="member.MemberDTO"%>
<%@page import="java.util.ArrayList"%>
<%@ page language="java" contentType="text/html; charset=UTF-8"
    pageEncoding="UTF-8"  %>
<!DOCTYPE html>
<html>
<head>
<meta charset="UTF-8">
<title>Insert title here</title>
</head>
<body>

		<%
				ArrayList<MemberDTO> userlist = (ArrayList<MemberDTO>)request.getAttribute("userlist");
		%>

		<h1>사원목록</h1>
		<hr/>
		<table border='1' width="600">
			<tr bgColor='skyblue'>
				<th>아이디 </th>
				<th>성명</th>
				<th>패스워드</th>
				<th>주소</th>
				<th>포인트</th>
				<th>부서번호</th>
				<th>삭제</th>
			</tr>
			<%
			int size = userlist.size();
			for(int i =0; i<size; i++) {
				MemberDTO user = userlist.get(i);
			%>
			<tr>
				<td><a href="serverweb/member/read.do?id= <%= user.getId()%>"><%= user.getId( )%></a></td>
				<td><%= user.getName() %></td>
				<td><%= user.getPass() %></td>
				<td><%= user.getAddr() %></td>
				<td><%= user.getPoint() %></td>
				<td><%= user.getDeptno()%></td>
				<td><a href="serverweb/member/delete.do?id=<%= user.getId() %>">삭제</a></td>
				</tr>	
				<% } %>
			</table>
</body>
</html>                                         
```

