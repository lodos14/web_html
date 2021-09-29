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

    
## 3. 서버와 클라이언트
![클라이언트와서버](https://user-images.githubusercontent.com/81665608/135127512-d956e6f3-a375-46d6-8492-4c2d6569725a.png)



