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

