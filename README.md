# HTML
## 간단한 예제 사이트
https://lodos14.github.io/web_html/
## 1. HTML 기본 구조
\<!DOCTYPE html><br>
\<html><br>
&nbsp;&nbsp;\<head><br>
&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;본문 설명<br>
&nbsp;&nbsp;\</head><br>
&nbsp;&nbsp;\<body><br>
&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;본문<br>
&nbsp;&nbsp;\</body><br>
\</html>
## 2. 기본 문법 - 태그
### 강조
\<strong>

글씨 진하게


### 줄바꿈과 단락

p 태그를 통해서 단락의 경계를 분명히 하면서
CSS를 통해서 p 태그의 디자인을 자유롭게 변경할 수 있기 때문에
br 태그 보다 p 태그가 더 좋은 선택일 수 있다.

#### \<br>

    새로운 줄을 표현할 때는<br> 태그를 사용합니다.

새로운 줄을 표현할 때는
<br> 태그를 사용합니다.

#### \<p>
    
    단락<p>단락을 표현할 때 사용합니다.</p>
단락<p>단락을 표현할 때 사용합니다.</p>

### 링크
#### \<a>
\<a href = "주소">\</a> <br>
\<a href = "./about.html">\</a> 상대경로 가능<br>
\<a href = "#hello">\</a> 페이지내 이동 가능<br>
\<a href="mailto:메일주소">\</a> 메일쓰기<br>
\<a href="tel:전화번호">\</a> 전화걸기<br>
\<a href = "주소" target="_blank">\</a> 새 페이지를 열어서 이동

### 이미지
#### \<img>
\<img src="" alt="">
src 속성에 이미지 주소 또는 내 컴퓨터에 있는 사진 경로를 써주면 된다.<br>
alt 속성은 엑박이 뜨는 경우 대체로 텍스트를 넣어준다.

### 목록
ol : 순서가 있는 리스트 <br>
ul : 순서가 없는 리스트 <br>
li : 리스트를 나열 <br>
ul, ol의 자식은 무조건 li만 가능 <br>

#### \<ol>
    <ol>
      <li>사과</li>
      <li>수박</li>
      <li>바나나</li>
    </ol>
<ol>
    <li>사과</li>
    <li>수박</li>
    <li>바나나</li>
</ol>

#### \<ul>
    <ul>
      <li>사과</li>
      <li>수박</li>
      <li>바나나</li>
    </ul>
<ul>
    <li>사과</li>
    <li>수박</li>
    <li>바나나</li>
</ul>

### 정의 리스트
dl, dt=(key), dd=(value)<br>
dl의 자식요소는 div, dt, dd만 가능

    <dl>
      <dt>
        학습 學習 [학씁]
      </dt>
      <dd>
        1. noun 배워서 익힘.
      </dd>
      <dd>
        2. noun 심리 경험의 결과로 나타나는, 비교적 지속적인 행동의 변화나 그 잠재력의 변화. 또는 지식을 습득하는 과정
      </dd>
    </dl>

<dl>
  <dt>
    학습 學習 [학씁]
  </dt>
  <dd>
    1. noun 배워서 익힘.
  </dd>
  <dd>
    2. noun 심리 경험의 결과로 나타나는, 비교적 지속적인 행동의 변화나 그 잠재력의 변화. 또는 지식을 습득하는 과정
  </dd>
</dl>

### 인용
\<blockquote cite="주소">인용내용\</blockquote><br>
\<q>문단내에 인용내용\</q> <br>
\<cite>출처\</cite> <br>

    <blockquote>
        <p>
            이런 말이 있다. <q>
            우리가 겪을 수 있는 가장 아름다운 체험은 신비다.
            신비는 모든 참 예술과 과학의 근원이다.</q> 
        </p>
    <cite>- 알버트 아인슈타인</cite>
    </blockquote>
    
<blockquote>
    <p>
        이런 말이 있다.<q>
        우리가 겪을 수 있는 가장 아름다운 체험은 신비다.
        신비는 모든 참 예술과 과학의 근원이다.</q> 
    </p>
<cite>- 알버트 아인슈타인</cite>
</blockquote>

### div, span 의미없는 태그
div: 묶어줄 때<br>
span : 문단 내에 일부분을 css 줄 때

### 사용자로부터 Input을 받기 위한 태그(form)
#### \<input>
    <input
      type="text"
      placeholder="공백 글씨" 
      minlength="5"
      maxlength="13"
      required
      value = "" />
      
 type : text, email, password, url, number(속성에 min, max 최소 최대값), file <br>
 \<input type="file" accept="png, jpg"/>  
 
 ### 폼양식에 이름을 붙이는 태그
 #### \<label>
    <label for="user-name">이름</label>
    <input type="text" id="user-name" />
    
 ### form(input) 예제
    <form action="#" method="POST">
      <label for="user-name">이름</label>
      <input type="text" id="user-name" required placeholder="이름" />

      <label for="user-id">아이디</label>
      <input
        type="text"
        required
        placeholder="아이디"
        minlength="5"
        maxlength="10"
        id="user-id"
      />

      <label for="user-password">비밀번호</label>
      <input
        type="password"
        required
        placeholder="비밀번호"
        minlength="6"
        maxlength="12"
        id="user-password"
      />

      <label for="user_email">이메일</label>
      <input type="email" required placeholder="이메일" id="user_email" />

      <label for="user-phone-number">전화번호</label>
      <input
        type="tel"
        required
        placeholder="전화번호 (***-****-****)"
        pattern="[0-9]{3}-[0-9]{4}-[0-9]{4}"
        id="user-phone-number"
      />

      <label for="user-age">나이</label>
      <input type="number" placeholder="만 나이" min="12" max="122" id="user-age"/>

      <label for="user-file">파일</label>
      <input type="file" accept="image/*, audio/*, video/*" id="user-file" />
      <button type="submit">가입하기</button>
    </form>

### input(radio & Checkbox)
Radio : 하나만 입력 가능 name추가 <br>
Checkbox : 다중입력가능
   
#### radio
    <form action="" method="GET">
        <input type="radio" name="apple1" value="subscribed" id="subscribed1" />
        <label for="subscribed1">구독중</label>
        <input type="radio" name="apple1" value="unsubscribed" id="unsubscribed2" />
        <label for="unsubscribed">미구독</label>
          <br>
        <input type="radio" name="apple2" value="subscribed" id="subscribed3" />
        <label for="subscribed3">구독중</label>
        <input type="radio" name="apple2" value="unsubscribed" id="unsubscribed4" />
         label for="unsubscribed4">미구독</label>
        <button>submit</button>
    </form>
    
#### Checkbox
    <form action="">
        <input type="Checkbox" name="skills" value="html" id="html"/>
        <label for="html">HTML</label>
        <input type="Checkbox" name="skills" value="css" id="css"/>
        <label for="css">css</label>
        <input type="Checkbox" name="skills" value="JS" id="JaveScript"/>
        <label for="JaveScript">JaveScript</label>
        <button>submit</button>
    </form>
    
### input(select)
    
    <form action="" method="GET">
        <label for="skill">스킬</label>
        <select multiple name="skill" id="skill">
          <option value="html" >HTML</option>
          <option value="css">CSS</option>
          <option value="JS">JavaScript</option>
        </select>
        <button>Submit</button>
    </form>

### input(textarea)

    <label for="123">자기소개</label>
    <textarea id="123" name="" id="" cols="30" rows="10" placeholder="자기소개"></textarea> 

### form(button)

    <form action="">
      <input type="text">
      <button type="button">버튼</button>
      <button type="submit">버튼</button>
      <button type="reset">버튼</button>
    </form>
  
### 테이블
table : 테이블 정의<br>
tr : 테이블 가로줄<br>
th : 테이블 헤더<br>
td : 테이블 데이터<br>

\<th scope = "row"> : 해당 셀이 가로 데이터에 대한 헤더<br>
\<th scope = "col"> : 해당 셀이 세로 데이터에 대한 헤더<br>
\<td rowspan="2"> : 세로 병합 <br>
\<td colspan="2"> : 가로 병합 <br>

    <table>
        <thead>
            <tr>
                <th>ID</th>
                <th>이름</th>
                <th>개발분야</th>
                <th>기타</th>
            </tr>
        </thead> 
        <tbody>
            <tr>
                <td>0001</td>
                <td>홍길동</td>
                <td>프론트엔드</td>
                <td></td> 내용이 없더라도 빈칸으로 놔둬야함
            </tr>
            <tr>
                <td>0002</td>
                <td>이순신</td>
                <td>백엔드</td>
                <td></td> 내용이 없더라도 빈칸으로 놔둬야함
            </tr>
        </tbody>
    </table>

<table>
    <thead>
        <tr>
            <th>ID</th>
            <th>이름</th>
            <th>개발분야</th>
            <th>기타</th>
        </tr>
    </thead> 
    <tbody>
        <tr>
            <td>0001</td>
            <td>홍길동</td>
            <td>프론트엔드</td>
            <td></td>
        </tr>
        <tr>
            <td>0002</td>
            <td>이순신</td>
            <td>백엔드</td>
            <td></td>
        </tr>
    </tbody>
</table>

 
## 3. 서버와 클라이언트
![클라이언트와서버](https://user-images.githubusercontent.com/81665608/135127512-d956e6f3-a375-46d6-8492-4c2d6569725a.png)



