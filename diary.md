
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

- <em\></em\>태그는 텍스트를 이탤릭체 뿐만 아니라 그 내용이 중요하다는 의미도 함께 포함해 줍니다.
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

