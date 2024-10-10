
#### HTML 태그(tag)
- HTML 태그는 태그 이름을 꺾쇠 괄호(<>)로 감싸서 표현합니다.
- 종료 태가 없는 태그 존재 \<img\> \<br\> \<hr\>
```
<태그이름>  // 시작 태그
</태그이름> // 종료 태그
```

#### HTML 기본 구조
```
<!DOCTYPE html> : 현재 문서가 HTML5 문서임을 명시합니다.
<html> : HTML 문서의 루트(root) 요소를 정의합니다.

<head> : HTML 문서의 메타데이터(metadata)를 정의합니다.
- 메타데이터(metadata)란 HTML 문서에 대한 정보(data)로 웹 브라우저에는 직접적으로 표현되지 않는 정보를 의미합니다.
- 이러한 메타데이터는 <title>, <style>, <meta>, <link>, <script>, <base>태그 등을 이용하여 표현할 수 있습니다.

<title> : HTML 문서의 제목(title)을 정의하며, 다음과 같은 용도로 사용됩니다.
- 웹 브라우저의 툴바(toolbar)에 표시됩니다.
- 웹 브라우저의 즐겨찾기(favorites)에 추가할 때 즐겨찾기의 제목이 됩니다.
- 검색 엔진의 결과 페이지에 제목으로 표시됩니다.

<body> : 웹 브라우저를 통해 보이는 내용(content) 부분입니다.
<h1> ~ <h6> : 제목(heading)을 나타냅니다.
<p> : 단락(paragraph)을 나타냅니다.
```
#### HTML 요소 구조
- 오류 방지를 위해 속성값은 언제나 따옴표로 표시
```
<p class = "para"></p>
<태그이름 속성이름="속성값">
```

#### 제목(Heading)
- 검색엔진은 각 웹 사이트의 내용을 바로 이 /<h/>태그를 이용하여 키워드를 수집한다.
- HTML 문서의 제목에 해당하는 부분을 \<big\>태그나 \<bold\>태그를 사용하여 표현하지 않도록 합니다.
```
<h1~h6>제목1의 크기입니다!</h1~h6>
```

#### 단락(Paragraph)
- 여러번 띄어쓰기 해도 하나의 띄어쓰기만 인식한다.
```
<p>단락 입니다. 띄어쓰기 여러번해도 한번만 적용</p>
```
- 형식 그대로 사용 하고 싶으면 \<pre\> 태그 사용
```
<pre>작성한 내용 그대로 화면에 반영</pre>
```
- 수평 가로 선 
```
<hr>
```

#### 서식
-  <b\></b\>태그는 단순히 화면의 텍스트를 굵게 표현해 줍니다.
```
<p><b>"이 부분"</b>은 단순히 글씨가 굵은 부분이에요!</p>
```

- <strong\></strong\>태그는 텍스트를 굵게 표현해줄 뿐만 아니라 그 내용이 중요하다는 의미도 함께 포함해 줍니다.
```
<p><strong>"이 부분"</strong>은 중요한 부분이라서 굵게 표현됐어요!</p>
```

- <i\></i\>태그는 단순히 화면의 텍스트를 이탤릭체로 표현해 줍니다.
```
<p><i>"이 부분"</i>은 단순히 글씨가 이탤릭체인 부분이에요!</p>
```

- <em\></em\>태그는 텍스트를 이탤릭체 뿐만 아니라 그 내용이 중요하다는 의미도 함께 포함해 줍니다.
```
<p><em>"이 부분"</em>은 중요한 부분이라서 이탤릭체로 표현됐어요!</p>
```

- <mark\></mark\>태그는 하이라이팅 효과를 표현해 줍니다.
```
<p><mark>"이 부분"</mark>만 하이라이팅하고 싶어요.</p>
```

- <del\></del\>태그(delete)는 텍스트 중앙에 가로줄을 만들어 마치 텍스트를 지운 것과 같은 효과를 내줍니다.
```
<p><del>"이 부분"</del>을 지운 것처럼 하고 싶어요.</p>
```

- <ins\></ins\>태그(insert)는 텍스트 밑에 가로줄을 만들어 마치 빈칸에 텍스트를 삽입한 것과 같은 효과를 내줍니다.
```
<p><ins>"밑줄 친 부분"</ins>에 들어갈 알맞은 말을 고르세요.</p>
```

- 위첨자는 <sup\></sup\>태그(superscript)를 사용하여, 아래첨자는 <sub\></sub\>태그(subscript)를 사용하여 각각 표현할 수 있습니다.
```
<p>X<sup>2</sup> + Y<sup>3</sup> = Z</p>
<p>물을 나타내는 화학식은 H<sub>2</sub>O 입니다.</p>
```

#### 인용구(Quotation)
- 짧은 인용구는 <q\></q\>태그를 사용하여 표현할 수 있으며, 자동으로 앞뒤에 큰따옴표가 붙습니다.
```
<p>HTML의 정의는
<q>웹 페이지를 만들기 위한 하이퍼텍스트 마크업 언어</q>
입니다.</p>
```
- 길이가 긴 인용문은 <blockquote\></blockquote\>태그를 사용하여 표현할 수 있습니다.
```
<p>HTML의 정의</p>
<blockquote>
인터넷 서비스의 하나인 월드 와이드 웹을 통해 볼 수 있는 문서를 만들 때 사용하는 프로그래밍 언어의 한 종류이다.
</blockquote>
```
- HTML에서 용어의 축약형을 표현하기 위해서는 <abbr\></abbr\>태그(abbreviation)를 사용합니다.
```
<p><strong><abbr title="HyperText Markup Language 5">HTML5</abbr></strong>
란 웹 문서를 제작하는 데 쓰이는 프로그래밍 언어인 HTML의 최신규격입니다.</p>
```
- <address\></address\>태그를 사용하면 HTML에서 이탤릭체로 주소를 표현할 수 있습니다.
```
<address>
    서울특별시<br>
    강남구 테헤란로
</address>
```

#### 문자셋(Character set)
-   HTML 문서가 저장될 때 사용된 문자셋에 대한 정보를 <head\>태그 내의 <meta\>태그에 명시합니다.

```
<meta charset="UTF-8">
```

#### HTML 스타일(Style)
- style 속성을 이용한 방법은 오직 단 하나의 HTML 요소에만 스타일을 적용할 수 있습니다.
- style 속성값에 사용되는 CSS 속성(property)과 속성값들은 세미콜론(;)을 이용하여 구분합니다.
- CSS 속성을 하나만 사용할 때나, 여러 개의 CSS 속성 중 맨 마지막 CSS 속성은 세미콜론(;)을 생략할 수 있습니다.
```
<태그이름 style="속성이름:속성값">

<h1 style="background-color:white; color:maroon; font-size:150%; text-align:center">
    style 속성을 이용하여 한 번에 스타일링 하기!
</h1>
```

- background 속성을 이용하면 HTML 요소의 배경을 이미지(image)로 설정할 수 있습니다.

```
<태그이름 background="이미지주소">
```

#### HTML 링크(Link)
- <a\>태그의 href 속성은 링크를 클릭하면 연결할 페이지나 사이트의 URL 주소를 명시합니다.
- <a\>태그는 텍스트나 단락, 이미지 등 다양한 HTML 요소에 사용할 수 있습니다.
```
<a href="링크주소">HTML 링크</a>
```
- a 태그의 target 속성
```
<h2><a href="/html/intro" target="_blank">새창</a></h2>
<h2><a href="/html/intro" target="_self">현재창</a></h2>
<h2><a href="/html/intro" target="_parent">부모 프레임</a></h2>
<h2><a href="/html/intro" target="_top">최상위 프레임</a></h2>
<h2><a href="/html/intro" target="myframe">지정된 프레임</a></h2>

<-- 아래는 지정된 프레임 코드-->
<iframe name="myframe" style="width:50%; height: 330px"></iframe>
```

- <a\>태그의 name 속성을 이용하면 간단한 책갈피를 만들 수 있습니다. 
```
<a href="#bookmark"><p>제목 3으로 갑시다!!!</p></a>
<h2><a name="bookmark"></a>제목 3</h2>
```

#### 이미지의 삽입
- HTML 문서에 이미지를 삽입할 때는 <img\>태그를 사용합니다.
- <img\> 태그는 종료 태그가 없는 빈 태그(empty tag)이며, 다음과 같은 문법으로 사용됩니다.
```
<img src="이미지주소" alt="대체문자열">
```
- 이미지에 <a\>태그를 이용하여 링크를 설정할 수 있습니다.
```
<a href="/html/intro" target="_blank">
  <img src="/examples/images/img_flag.png" alt="flag" style="width:320px; height:214px">
</a>
```

- 이미지의 크기 설정
```
<style>
    img {
        width:100%;
        border: 1px solid black;
    }
</style>
```

```
<img src="/examples/images/img_flag.png" alt="html size" width="320" height="214">
```

```
<img src="/examples/images/img_flag.png" alt="style size" style="width:320px; height:214px">
```

- 이미지 테두리 설정
```
<img src="/examples/images/img_flag.png" alt="이미지 테두리" 
    style="width:320px; height:214px; border: 3px solid black">
```

#### 리스트
- 순수가 없는 리스트
```
<ul>
    <li>사과</li>
    <li>멜론</li>
    <li>바나나</li>
</ul>

CSS의 list-style-type 속성을 사용하면 리스트 요소 앞에 위치하는 마커(marker)를 다른 모양으로 변경할 수 있습니다.

- disc : 검정색 작은 원 모양 (기본설정)
- circle : 흰색 작은 원 모양
- square : 사각형 모양
```

- 순서가 있는 리스트
```
<ol>
    <li>사과</li>
    <li>멜론</li>
    <li>바나나</li>
</ol>
```

- 정의 리스트
```
<dl>
    <dt>용어</dt>
    <dd>용어에 대한 정의</dd>
    <dt>용어</dt>
    <dd>용어에 대한 정의</dd>
</dl>
```

#### HTML 테이블(Table)
```
<table style="width:100%">
    <tr style="background-color:lightgrey">
        <th>참치</th>
        <th>고래</th>      
    </tr>
    <tr>
        <td>상어</td>
        <td>문어</td>
    </tr>
    <tr>
        <td>오징어</td>
        <td>고등어</td>
    </tr>
</table>
```
- 테이블의 열 합치기
```
<table style="width:100%">
    <tr>
        <td>참치</td>
        <td colspan="2">고래</td>        
    </tr>
    <tr>
        <td>상어</td>
        <td>문어</td>        
        <td>꽁치</td>
    </tr>
</table>
```
- 테이블의 행 합치기
```
<table style="width:100%">
    <tr>
        <td rowspan="2">상어</td>
        <td>문어</td>        
        <td>꽁치</td>
    </tr>
    <tr>
        <td>고등어</td>        
        <td>돌고래</td>
    </tr>
</table>
```
- 테이블의 캡션 설정
```
<table style="width:100%">
    <caption>캡션</caption>
    <tr>
        <td>참치</td>
        <td>고래</td>
        <td>날치</td>    
    </tr>
</table>
```

#### 블록과 인라인
- 블록(block) 타입의 요소
- display 속성값이 블록(block)인 요소는 언제나 새로운 라인(line)에서 시작하며, 해당 라인의 모든 너비를 차지합니다.
```
<p>, <div>, <h>, <ul>, <ol>, <form>
```
- <div\></div\>
```
<div style="">
 여기 부분의 스타일을 한번에 적용
</div>
```

- 인라인(inline) 타입의 요소 
- display 속성값이 인라인(inline)인 요소는 새로운 라인(line)에서 시작하지 않습니다.
- 또한, 요소의 너비도 해당 라인 전체가 아닌 해당 HTML 요소의 내용(content)만큼만 차지합니다.
```
<span>, <a>, <img>
```

- <span\></span\>
```
<p>
<span style="">해당 부분만 다른스타일 적용</span>
</p>
```

#### iframe 
- iframe 요소는 기본적으로 검정색 테두리(border)를 가집니다.
- <a\> 태그의 target 으로 프레임 지정을 해주면 페이지 변경 가능
```
<iframe src="/css/intro" name="frame_target" style="width:100%; height:400px;"></iframe>
<p>
    <a href="/php/intro" target="frame_target">PHP 수업 확인하러 가기 =></a>
</p>
```

> class 와 id 의 차이는 class 는 복수사용, class 는 단일 사용

#### form 요소
- GET 방식은 주소에 데이터(data)를 추가하여 전달하는 방식입니다. 데이터가 주소 입력창에 그대로 나타나며, 전송할 수 있는 데이터의 크기 또한 제한적입니다. 따라서 검색 엔진의 쿼리(query)와 같이 크기가 작고 중요도가 낮은 정보를 보낼 때 주로 사용합니다.

- POST 방식은 데이터(data)를 별도로 첨부하여 전달하는 방식입니다. 데이터가 외부에 드러나지 않으며, 전송할 수 있는 데이터의 크기 또한 제한이 없습니다. 따라서 보안성 및 활용성이 GET 방식보다 좋습니다.
```
<form action="처리할페이지주소" method="get|post"></form>
```

#### input 요소
- 텍스트 입력
```
<input\>태그의 type 속성 값을 "text"로 설정하면, 사용자로부터 한 줄의 텍스트를 입력 받을 수 있습니다.

<input type="text" name="search">
```
- 비밀번호 입력
```
<input>태그의 type 속성값을 "password"로 설정하면, 사용자로부터 비밀번호를 입력받을 수 있습니다.

<input type="password" name="password">
```
- 라디오 버튼
```
<input>태그의 type 속성값을 "radio"로 설정하면, 사용자로부터 여러 개의 옵션(option) 중에서 단 하나의 옵션만을 입력받을 수 있습니다.


<input type="radio" name="lecture" value="html" checked> HTML <br>
<input type="radio" name="lecture" value="css"> CSS <br>
```
- 체크 박스
```
<input>태그의 type 속성값을 "checkbox"로 설정하면, 사용자로부터 여러 개의 옵션 중에서 다수의 옵션을 입력받을 수 있습니다.

<input type="checkbox" name="lecture" value="html" checked> HTML <br>
<input type="checkbox" name="lecture" value="css"> CSS <br>
<input type="checkbox" name="lecture" value="cpp" disabled> C++

# disabled 속성을 이용하여 해당 옵션을 선택할 수 없게 설정할 수도 있습니다.
```
- 파일 선택
```
<input\>태그의 type 속성값을 "file"로 설정하면, 사용자로부터 파일을 전송받을 수 있습니다.

<input type="file" name="upload_file" accept="image/*">
# accept 속성을 이용하여 입력받을 수 있는 파일의 확장자 및 종류를 명시할 수 있습니다.
```
- 선택 입력
```
select 요소는 여러 개의 옵션이 드롭다운 리스트(drop-down list)로 되어 있으며, 그중에서 단 하나의 옵션만을 입력받을 수 있습니다.

<select name="fruit">
    <option value="apple"> 사과
    <option value="orange" selected> 귤
    <option value="strawberry"> 딸기
    <option value="peach"> 복숭아
</select>
```
- 문장 입력
```
textarea 요소는 사용자로부터 여러 줄의 텍스트를 입력받을 수 있습니다.

<textarea name="message" rows="5" cols="30"></textarea>

# rows 속성과 cols 속성을 이용하여 textarea 요소의 크기를 자유롭게 지정할 수 있습니다.
```
- 버튼
```
<button type="button" onclick="alert('버튼을 클릭하셨군요!')">
    버튼을 눌러주세요.
</button>
```
- 전송 버튼
```
<input>태그의 type 속성값을 "submit"으로 설정하면, 사용자로부터 입력받은 데이터(data)를 서버의 폼 핸들러로 제출하는 버튼을 만들 수 있습니다.
폼 핸들러 -> action ="해당 부분" 으로 전송

<form action="/examples/media/request.php">
    어릴 때 자신의 별명을 적어주세요 : <br>
    <input type="text" name="nickname" value="별명"><br><br>
    <input type="submit" value="전송">
</form>
```
- 필드셋(fieldset)
```
fieldset 요소는 form 요소와 관련된 데이터들을 하나로 묶어주는 역할을 합니다.
legend 요소는 fieldset 요소 안에서만 사용할 수 있으며, fieldset 요소의 제목을 나타냅니다.

<form action="/examples/media/request.php">
    <fieldset>
        <legend>입력 양식</legend>
        이름 : <br>
        <input type="text" name="username"><br>
        이메일 : <br>
        <input type="text" name="email"><br><br>
        <input type="submit" value="전송">
    </fieldset>
</form>

```

##### input 요소의 속성
- value 속성
```
value 속성은 input 요소의 입력 필드(input field)에 나타나는 초깃값을 설정합니다.
```
- readonly 속성
```
readonly 속성은 사용자가 입력 필드를 볼 수는 있으나, 수정할 수는 없도록 설정합니다.
disabled 속성과 다른 점은 전송 버튼(submit)을 누르면 초깃값이 서버로 전송된다는 점입니다.
```
-  disabled 속성
```
disabled 속성은 사용자가 입력 필드를 아예 사용할 수 없도록 설정합니다.
disabled 속성이 설정된 입력 필드는 사용할 수도 없고, 클릭할 수도 없습니다.
또한, readonly 속성과는 달리 전송 버튼(submit)을 눌러도 초깃값이 서버로 전송되지 않습니다.
```
-  maxlength 속성
```
maxlength 속성은 입력 필드에 입력할 수 있는 문자의 최대 길이(length)를 설정합니다.
```

-  size 속성
```
size 속성은 입력 필드에 보여지는 input 요소의 크기(size)를 설정합니다.
maxlength 속성과는 달리 입력 필드가 한 번에 보여줄 수 있는 문자의 최대 개수만을 의미합니다.
따라서 입력될 수 있는 문자의 최대 길이는 maxlength 속성값에 따라 달라지며, size 속성과는 전혀 무관합니다.
```
