이번주에는 css 요소들과 함께 flexbox layout을 배웠다. 이를 바탕으로 개구리를 같은 색깔의 연잎 위에 올리도록 하는 과제를 수행했다. flexbox layout으로 아이템이 배열될 방향을 정할 수 있었다. 각 문제마다 CSS 속성에 대한 설명도 써 있어서 쉽게 익힐 수 있었다.

1. 다음은 과제를 하면서 사용한 CSS 속성들이다.

   - justify-content: flex-start는 요소들을 왼쪽으로 정렬한다.
   - justify-content: flex-end는 요소들을 오른쪽으로 정렬한다.
   - justify-content: center는 요소들을 가운데로 정렬한다.
   - justify-content: space-between는 요소들 사이를 동일한 간격으로 둔다.
   - justify-content: space-around는 요소들 주위를 동일한 간격으로 둔다.

   - align-items: flex-start는 요소들을 제일 위쪽으로 정렬한다.
   - align-items: flex-end는 요소들을 제일 아래쪽으로 정렬한다.
   - align-items: center는 요소들을 세로선 상의 가운데로 정렬한다.

   - flex-direction: row는 요소들을 텍스트 방향으로 정렬한다.
   - flex-direction: row-reverse는 요소들을 텍스트 반대 방향으로 정렬한다.
   - flex-direction: column는 요소들을 위에서 아래로 정렬한다.
   - flex-direction: column-reverse는 요소들을 아래에서 위로 정렬한다.

   - flex-wrap: wrap는 요소들을 여러 줄로 나누어 정렬한다.
   - flex-direction과 flex-wrap을 같이 사용하기 위해 flex-flow를 사용할 수 있다.

2. 다음은 각 단계에 대한 답이다.

   - 1단계: justify-content: flex-end;
   - 2단계: justify-content: center;
   - 3단계: justify-content: space-around;
   - 4단계: justify-content: space-between;
   - 5단계: align-items: flex-end;
   - 6단계: justify-content: center; align-items: center;
   - 7단계: justify-content: space-around; align-items: flex-end;
   - 8단계: flex-direction: row-reverse;
   - 9단계: flex-direction: column;
   - 10단계: flex-direction: row-reverse; justify-content: flex-end;
   - 11단계: flex-direction: column; justify-content: flex-end;
   - 12단계: flex-direction: column-reverse; justify-content: space-between;
   - 13단계: justify-content: center; align-items: flex-end; flex-direction: row-reverse;
   - 18단계: flex-wrap: wrap;
   - 19단계: flex-direction: column; flex-wrap: wrap;
   - 20단계: flex-flow: column wrap;
