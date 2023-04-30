* 다음은 PoiemaWeb의 html5에서 2번부터 5번까지와 css에서 1번부터 4번, 7번부터 9번까지의 내용 중 새로 알게 된 내용이나 기억할 내용을 정리한 것이다.

# HTML

1. HTML5
   - HTML5 문서는 반드시 !DOCTYPE html 태그로 시작해 문서 형식을 HTML5로 지정하고, 실질적인 HTML document를 2행부터 html 태그와 /html 태그 사이에 기술한다. 그 아래 document title, 외부 파일의 참조, 메타데이터의 설정 등을 head 태그와 /head 태그 사이에 기술하고, 이는 브라우저에는 표시되지 않는다. 웹 브라우저에 출력되는 모든 요소는 body 태그와 /body 태그사이에 위치한다.
   - 빈 요소는 content를 가질 수 없는 요소를 말하며, 이는 attribute만 가질 수 있다.

2. Semantic Web
   - 검색엔진 검색 사이트 이용자가 검색할 만한 키워드를 예상해 검색 키워드에 대응하는 인덱스를 만드는 인덱싱을 한다. 여기 사용하는 정보는 웹사이트의 HTML 코드이다. 이때 Semantic element를 해석한다.
   - Semantic tag란 브라우저, 검색엔진, 개발자 모두에게 content의 의미를 명확하게 설명하는 역할을 한다.
   - Semantic Web이란 웹에 존재하는 수많은 웹페이지들에 메타데이터를 부여해 기존의 잡다한 데이터 집합이었던 웹페이지를 의미와 관련성을 가지는 거대한 데이터베이스로 구축하고자 한다.

3. Tag
   - 문서 형식 정의 (Document Type Definition) 태그는 출력할 웹 페이지의 형식을 브라우저에게 전달한다. 문서의 최상위에 위치하며 대소문자를 구별하지 않는다. HTML5에서는 !DOCTYPE html과 같이 기술한다.
   - html tag는 모든 HTML 요소의 부모 요소이며 웹페이지에 단 하나만 존재한다. 
   - head tag는 메타데이터를 포함하기 위한 요소이며 웹페이지에 단 하나만 존재한다.
   - title tag는 문서의 제목을 정의한다. 이는 브라우저의 탭에 표시된다.
   - link tag는 외부 리소스와의 연계 정보를 정의한다. HTML과 외부 CSS 파일을 연계할 때 주로 사용된다.
   - script tag는 client-side JavaScript를 정의한다.
   - meta tag는 description, keywords, author, 기타 메타데이터 정의에 사용되고, 메타 데이터는 브라우저, 검색엔진 등에 의해 사용된다. charset attribute는 브라우저가 사용할 문자셋을 정의한다.

4. Text tag
   - Heading tag는 제목을 나타낼 때 사용하며 h1~h6가 있다. Semantic Web의 의미를 살려 제목 의외에는 사용을 지양한다.
   - 글자 형태 태그에서 i는 Italic체를 지정한다. em은 emphasized text를 지정한다. del은 deleted text를 지정한다. ins는 inserted text를 지정한다. sub는 subscripted text, sup는 superscripted text를 지정한다.
   - 본문 태그에서 pre는 형식화된 text를 지정한다. hr는 수평줄을 삽입한다. q는 짧은 인용문을 지정한다. blockquote는 긴 인용문 블록을 지정한다.

# CSS

1. CSS 기본 문법
   - CSS는 HTML의 각 요소의 style을 정의해 화면에 어떻게 렌더링하면 되는지 브라우저에게 설명하기 위한 언어이다.
   - Selector는 스타일을 적용하고자 하는 HTML 요소를 선택하기 위해 CSS에서 제공하는 수단이다.
   - Selector로 HTML 요소를 선택하고 {} 내에 property와 값을 지정하는 것으로 style을 정의할 수 있다. 여러개를 연속해 지정할 수 있으며 ;으로 구분한다.
   - Embedding style로 HTML 내부에 CSS를 포함시킬 수 있다. 하지만 Link style을 사용하는 것이 좋다.
   - Inline style은 HTML 요소의 style property에 CSS를 기술하는 방식이다. 하지만 Link style을 사용하는 것이 좋다.

2. Selector
   - Universal Selector는 HTML 문서 내 모든 요소를 선택한다.
   - Type Selector는 지정된 태그명을 가지는 요소를 선택한다.
   - ID Selector는 id attribute 값을 지정해 일치하는 요소를 선택한다.
   - Attribute Selector는 지정된 attribute를 갖는 모든 요소를 선택한다.
   - Descendant Combinator에서 자신의 1 level 상위에 속하는 요소를 부모 요소, 1 level 하위에 속하는 요소를 자식 요소라고 하고, 자신보다 n level 하위에 속하는 요소를 후손 요소라고 한다.
   - Sibling Combinator는 동위 관계에서 뒤에 위치하는 요소를 선택할 때 사용한다.
   - Negation pseudo-class는 selector에 해당하지 않는 모든 요소를 선택한다.
   - Pseudo-Element Selector는 요소의 특정 부분에 스타일을 적용하기 위해 사용된다.

3. CSS Property 값의 단위
   - CSS에서 사용하는 대표적인 크기 단위는 px (절대값), em, % (상대값)이다.
   - px는 요소의 크기나 이미지의 크기 지정에 주로 사용된다.
   - rem은 최상위 요소의 사이즈를 기준으로 삼는다. r은 root를 의미한다.
   - Viewport 단위는 상대적인 단위로 viewport를 기준으로 한 상대적 사이즈이다.

4. BOX Model
   - Box는 content, padding, border, margin으로 구성된다.
   - margin, padding property는 content의 4개의 방향인 top, right, left, bottom에 대해 지정할 수 있다.
   - margin property에 auto 키워드를 설정하면 해당 요소를 중앙 정렬할 수 있다.
   - max-width property로 브라우저 너비가 요소의 너비보다 좁아질 때 자동으로 요소의 너비를 줄어들게 할 수 있다.
   - border-width property는 테두리의 두께를 지정한다. 4개 방향에 대해 지정할 수 있다.
   - border-color property는 테두리의 색상을 지정한다.
   - box-sizing property는width, height property의 대상 영역을 변경할 수 있다.

5. Font & Text
   - font-size property는 텍스트의 크기를 정의한다.
   - font-style property는 Italic체 지정, font-weight property는 폰트 굵기를 지정한다.
   - line-height property는 텍스트의 높이를 지정한다.
   - text-decoration property로 링크 underline을 제거할 수 있다.
   - white space property는 공백, 들여쓰기, 줄바꿈에 대한 동작을 제어한다.

6. Position
   - position property는 요소의 위치를 정의한다.
   - static은 기본 위치로, position property를 지정하지 않았을 때의 위치이다. 이미 설정된 position을 무력화하기 위해 사용될 수 있다.
   - relative는 기본 위치를 기준으로 좌표 property를 사용해 위치를 이동시킨다.
   - absolute는 부모 요소 또는 가장 가까이 있는 조상 요소를 기준으로 좌표 property만큼 이동한다.
   - fixed는 스크롤이 되더라도 화면에서 사라지지 않고 항상 같은 곳에 위치한다.

7. Float
   - float property는 레이아웃을 구성할 때 블록 레벨 요소를 가로 정렬하기 위해 사용된다. 본래 이미지와 텍스트가 있을 때 이미지 주위를 텍스트로 감싸기 위해 만들어진 것이다.
   - float property를 사용하지 않은 블록 요소들은 수직으로 정렬된다. float:left로 왼쪽부터 가로 정렬, float:right로 오른쪽부터 가로정렬시킬 수 있다.
   - 중앙 가로 정렬은 margin property를 사용해야 한다.