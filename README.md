# css_1
Created with CodeSandbox

![1](https://user-images.githubusercontent.com/37132897/157812077-5cd6a960-4538-472c-a51b-949f42e8dbee.JPG)

- 현재 올린 소스 : 외부에서 폰트 가져온것과, 아이콘 가져온것에 대한 소스.
- 아래 설명들은 + 그전에 추가로 배운것들 정리

css
caniuse.com

css 사용 관련
- 내부 css : html 안에 있는 css
- 외부 css : 외부에 css 파일 따로 만들어서 작성 후에,
- link rel="stylesheet" href="폴더명/파일명" 으로 불러와서 사용 가능. 

만약, css에도 h1에 색상을 주었고, h1 태그에도 직접적으로 태그에 색상을 주었다 치면, 그 태그에 가장 가까운 css를 반영시킨다.
ex) css 보다 h1 style="color:green;" 우세 
p{hello}*20 하면 p태그로 감싸진 hello 텍스트 문장이 20개가 나온다. 

기타 팁 관련
- 페이지에서 ctrl+shift+i 누르면 개발자 도구 가 열리고,
- 거기서 ctrl+shift+c 나 마우스 커서 모양 누르면, 디자인에 대한 소스 정보를 알 수 있다.

- 여백 같은거는 코딩을 직접 한게 아니기 때문에, 나중에 결과물에서 의도치 않은 화면을 만들어내기도한다. 
- 그래서, 구글에서 css reset 을 쳐서, 나오는 웹사이트의 css 문구를 복사해서,
css 파일에 붙여넣어서 초기화를 처음에 한번 시켜주고 시작하는것이 좋다. 
 
style 태그 안에 ~ {

} ~ 부분을 선택자(selector) 라고 하고, 
괄호 안에 color:blue; 가 들어간다고 치면,
color 를 속성(property), blue 를 값(value) 라고한다.

- color 속성은, color name 으로 줄 수 도 있고, 16진수로 줄 수 도 있다.
ex) color:blue; , color:#000000; 
만약, 16진수로 할경우 총 6자리의 수 가 있는데, 앞에서부터 2자리 씩 r, g, b 부분을 맡는다.
- 구글에서 html color code 쳐서, 홈페이지 들어가면, 16진수 컬러 색상 볼 수 있다.
- 구글에서 html color name 쳐서, 홈페이지 들어가면, 컬러 네임으로 된 색상 볼 수 있다.

내부 css 사용 예시 관련
- 만약, style 안에서 div > p 하고 중괄호 해서 내용 넣으면, div 안에 있는 p태그에만 적용이 된다.
- style 안에서 * 하고 중괄호 해서 내용 넣으면, 모든 태그에 그 내용이 적용이 된다.
- style 안에서 #one 하고 중괄호 해서 내용 넣으면, body 에 있는 태그들 중에 one 이라는 ID를 가진 태그에만 css가 적용이 된다.
- style 안에서 .two 하고 중괄호 해서 내용 넣으면, two라는 클래스를 가져온다.

id 관련 ex) h1 id="one"
- html 안의 id 는 중첩 없이 유일하게 작성 해주어야한다.

class 관련 ex) h1 class = "two"
- class 는 id 와 다르게, 여러 클래스의 css 적용을 받을 수 있다.
Ex) h1 class = "one two"  하면, 내부 css 에서 .one 과 .two 에 적용시킨 css들이 다 h1에 적용이 된다는 소리.

p는 body 글자 사이즈를 그대로 물려받는다. 
사이즈에 em,rem 단위 등 있다.
google fonts 에 원하는 폰트 찾을 수 있다.(한글 지원되는걸로 할것)
- 원하는 폰트 눌러서, select this style 눌러서, css 복사해서 적용하고싶은 내용에 넣고,
위에 link 부분도 복사해서 head 안에 넣어주면 적용이 된다.
- google fonts 에서 icons 눌러서 원하는 아이콘 눌러서, span 으로 된 css 소스 
body 안에 넣어주고 outlined 부분을 지운 span class=material-icons 로 불러서 사용.
- font awesome 에서도 아이콘 사용가능하다.

padding 관련
- 4개의 padding : 10px 20px 30px 40px - 12시,3시,6시,9시 방향 여백
- 3개의 padding : 10px 20px 30px - 10이 탑, 30이 바텀, 20이 좌우 여백
- 2개의 padding : 10px 20px - 상하, 좌우 여백

- box-sizing: border-box; 는 설정해둔, width의 값을 고정시켜준다.

