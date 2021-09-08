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

