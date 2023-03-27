1. git의 명령어 add, commit, push는 각각 어떤 역할을 하는지 정리하고, git pull과 fetch의 차이점을 정리하시오.
   
   - 변화들을 쌓아놓는 공간인 Staging Area에 변화를 쌓기 (옮기기) 위해 git add 명령어를 사용한다. 그리고  git commit은 이 staging area의 변화들을 엮어 이름을 지어줄 수 있다. 이것으로 Local Repository인 .git directory에  저장된다.  이제 Local Repository에서 push를 통해 Remote Repository로 commit한 내용을 push할 수 있다. 깃허브는 Remote Repository에 포함된다. 여기에서 제공하는 하나의 서버이며 저장소이다. 즉, 이를 통해 코드를 공유하고 협업을 할 수 있다.

   - Fetch와 Pull을 통해 서로의 코드를 받아서 볼 수 있다. git pull은 Remote Repository에 있는 변화(변경된 사항)를 확인하고 Local Repository로 가져와 그 내용을 합친다. 반면, git fetch는 Remote Repository에 있는 변화를 Local Repository로 가져오기 전에 단순히 그 변화를 확인하고 싶을 때 사용한다. 확인하라는 명령은 전달하지만, 변경된 데이터를 Local Repository로 가져오지는 않는다.

2. 지난 주와 이번주 학습 내용을 정리하고 WIL을 작성하여 제출한다.
   
   - 1주차에는 수업 커리큘럼과 웹이 어떻게 이루어져있는지에 대하여 배웠다. URN이란 Uniform Resource Name으로, 이름으로 찾기가 가능하다. 강사님은 이를 도서 출판 번호로 비유하셨다. 책마다 고유한 코드를 가지고 있는 것이다. URL의 L은 Location으로, 그 위치를 나타낸 것이다. 이는 프로토콜과 DNS 주소로 이루어져있다. 그리고 본격적인 웹 스터디에 앞서 홍익대학교 홈페이지를 해부해보았다. 웹은 HTML (자료), CSS (UI), JS (제어)로 이루어져있는데, 이를 하나씩 없애가며 홈페이지가 점점 단순해지는 것을 볼 수 있었고, 이를 통해 웹이 어떻게 만들어지는지 가시적으로 알게 되었다.

    - 2주차에는 깃(Git)이란 무엇인가에 대하여 배웠다. 강사님은 깃을 닥터스트레인지에 비유하시며 코드의 분기를 만들고 합치는 것, 그리고 특정 시점으로 되돌아가는 기능이 있다고 하셨다. 깃이 관리하는 파일에는 untracked, unmodified, modified, staged의 상태가 있다. 내 작업공간을 Working Directory라고 하고, Staging Area는 내가 만든 변화를 모아놓는다. 그리고 commit한 코드는 Local Repository에 저장된다. 강의를 들으면서 그러면 깃과 깃허브가 뭐가 다른지 궁금증이 생겼는데, 강사님이 깃허브는 깃 + Hub로, Remote Repository를 제공하는 서버 중 하나이며 저장소라고 알려주셔서 그 차이점을 알게 되었다. 내가 코드를 짜면 git이 그 변화를 감지해 중간에 모아놨다가, commit하면 Local Repository에 넘겨준다. 그리고 협업과 공유를 위해 외부 저장소인 서버 Remote Repository , 즉 깃허브가 필요한 것이라는 것을 배웠다. 그리고 실습을 진행하여 내 github repository를 만들었다.