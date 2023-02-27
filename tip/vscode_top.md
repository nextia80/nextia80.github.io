
* 발췌 주소 : [https://en-percent.tistory.com/88](https://en-percent.tistory.com/88)

나는 평상시 이미 기본적인 틀을 구성되어 있는 코드를 만지고 있다
회사 웹페이지도 마찬가지로 이미 스타일과 로직이 설계된 코드를 만지다보니 굳이 들여쓰기나 공백을 신경 쓸 필요가 없었다

최근 회사 웹페이지에 새로운 카테고리를 추가하게 되면서 PHP소스를 새롭게 제작해야하는데 난관에 봉착했다
기존 CSS 스타일을 새롭게 추가해야하고....
이미 운영중인 웹페이지와 연동이 가능하도록 설정을 다 바꿔줘야하고....

결정적으로 나는 HTML을 제대로 배워본 적 없는 사람...........
뭐 여차저차 문제는 해결했는데 그 과정에서 정말 유용했던 정보를 얻었다

들여쓰기 넓이를 조절하는 법
![image](https://img1.daumcdn.net/thumb/R1280x0/?scode=mtistory2&fname=https%3A%2F%2Fblog.kakaocdn.net%2Fdn%2FcZpWad%2FbtrjLk6p6G9%2FkKWINwUrxk7roABDQaTDkk%2Fimg.png)

VScode 우측 하단을 보면 위 이미지처럼 코드에 대한 설명이 나온다
여기서 공백이 현재 2로 설정되어 있는걸 볼 수 있다
이게 바로 들여쓰기 넓이다
이 공백을 클릭하면.....
![image](https://img1.daumcdn.net/thumb/R1280x0/?scode=mtistory2&fname=https%3A%2F%2Fblog.kakaocdn.net%2Fdn%2Fbx5SPx%2FbtrjLw0eaDu%2FQnAGHFvpSR8p9KexIk2kPK%2Fimg.png)
이렇게 화면 상단에 작업선택란이 뜨게 된다
이부분에서 '공백을 사용한 들여쓰기'를 클릭하면
![image](https://img1.daumcdn.net/thumb/R1280x0/?scode=mtistory2&fname=https%3A%2F%2Fblog.kakaocdn.net%2Fdn%2FbkA2wH%2FbtrjKM94MGp%2FIZZJOfH3K4nqgJP9kckPwK%2Fimg.png)
이런식으로 현재 탭 크기를 조절할 수 있도록 되어 있다

* 주의해야 할 점!*
이 방법은 일시적인 수단에 불과하다
현재 이미지를 보다시피 숫자 2 옆에 '구성된 탭 크기'라고 쓰여져 있는걸 볼 수 있다
이 의미는 VScode 설정에서 탭 크기를 2로 고정값을 걸었다는 뜻이다
즉, 고정값을 건드려야만 추후 새롭게 만들 소스코드에서도 동일한 탭 크기를 사용할 수 있다는 것이다
들여쓰기 넓이 고정값으로 지정하기
관리 - 설정 으로 들어가서 검색창에 'indentation'이라고 검색하면 아래와 같은 설정 창이 뜬다
![image](https://img1.daumcdn.net/thumb/R1280x0/?scode=mtistory2&fname=https%3A%2F%2Fblog.kakaocdn.net%2Fdn%2Fc2ME7n%2FbtrjJyLgClo%2FUgUWkv1hto8BPbYyynMPzk%2Fimg.png)
여기서 확인해야할 사항

Editor : Insert Spaces

- 키보드에 'Tab'키를 누르면 공백으로 들여쓰기를 실행한다는 의미다
아마 대부분의 유저들은 기본적으로 체크되어 있을 것이니 패스~

Editor : Tab Size
- 이게 바로 들여쓰기 공백을 고정값을 정하는 것이다
- 자신이 원하는 숫자만큼의 크기를 공백으로 지정할 수 있다

*참고사항*
여기서 고정값을 잡았다 하더라도 내가 생성한 파일이 아닌, 다른 곳에서 생성되어 들어온 파일에는 적용되지 않는다

예를들어, 내가 고정값을 변경하기 전에는 공백값이 8이었다.
하지만 회사에서 사용중인 소스파일은 공백이 2로 제작된 파일로,
고정값이 8이었음에도 수정할 때마다 공백이 2로 반영되었다.
즉, 내가 처음부터 생성한 파일이 아니면 아무리 고정값이라 하더라도 반영되지 않는다는 점!

들여쓰기 자동정렬하기
PHP에 경우 워낙 열고 닫고 하는 문장이 많아서 들여쓰기가 참 민감하다
![image](https://img1.daumcdn.net/thumb/R1280x0/?scode=mtistory2&fname=https%3A%2F%2Fblog.kakaocdn.net%2Fdn%2FHiogg%2FbtrjLxEPYYm%2FCF54mB9ZXhkvIKtAEUb480%2Fimg.png)
만약 위와 같이 들여쓰기가 개판이 나있을 경우
1. 들여쓰기 정렬이 필요한 부분을 드래그해서 잡아준다
2. Ctrl + K, Ctrl + F를 차례대로 눌러준다
3. 자동정렬 끝!
진짜 순식간에 정렬이 끝나버린다
참으로 단축키를 알아두는건 내 업무와 멘탈을 윤택하게 해준다

이상 뒤늦은 꿀팁전수 끝!