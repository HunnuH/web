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

