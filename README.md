# TIL <!-- 편하게 블로그 쓰듯이 오류, 해결 및 방법 등등 작성하기! -->
## 작업폴더 설명
* `html_basic/` : html 기초 연습파일 모음
* `task/` : 과제 제출 폴더, 파일 모음(폴더명은 날짜별로 구성됨)
* `README.md` : 배운 내용 기록, 어려운 점 및 막힌 점 자유롭게 정리
----
### 2025/04/04 | HTML 3일차 | 문서와 레이아웃
* `h1~h6`, `p`, `br`, `strong`, `em`, `del`, `s`, `sup`, `sub`
## 블록태그
### H1 ~ H6태그 (제목) -> 문서 태그
* 제목의 중요도에 따라 6 -> 1 순으로 1에 가까워질수록 중요도가 올라간다.
* 웹사이트 로고의 경우 가장 중요한 &lt;h1&gt;레벨을 가진다.
* CSS 들어가게 되면 위 모양은 달라지기 때문에 대제목, 중제목, 소제목인 것만 외워두면 된다다
* 레벨 숫자 처리는 중간에 하나 띄면 안됩니다! 순서대로 내려가야 한다.
* 새로운 페이지 경로가 바뀌면 H1이 따로이다.
* 키워드 설정하지 않아도 H1,2,3 등에 잘 적어두면 그것도 키워드로 유입될 수 있다.
* 위 내용에 대해 키워드가 대제목(H1)과 더 연관될수록 좋다!
### P태그 (단락) -> 문서 태그
* 제목의 내용 용도로 주로 사용한다.
* 줄바꿈이 있다는 말은 블록태그가 닫혔기 때문이다.
* p와 h는 형제관계이다. (제목 안에 내용이 아니라 제목/내용이 따로 있으니 부모,자식관계가 아니라 형제 관계로 인식하기!)
### blockquote (긴 인용문) -> 문서 태그
* 내용 중 긴 인용문. 단락.
* cite : blockquote와 함께 쓰는 것으로, 출처 url주소를 쓴다.
### adress (연락처, 회사소개, 고객센터 등) -> 문서 태그
* 웹사이트의 관련 연락처, 소개, 고객센터 정보 등을 담을 때 사용한다.
* 다른 블록을 자식 또는 자손으로 배치할 수 없다. -> 인라인만 가능함
* footer 영역에 주로 사용한다.
* 내 회사, 내 사이트에 대한 내용만 작성해야 한다. (협력업체라도 적으면 안된다.)
* 카피라이트를 적고 싶다면 `&copy;`를 쓰면 된다.
### hr (수평선) -> 문서 태그
* 사이트 각 영역을 구분할 때 사용한다.
* CSS에서는 표현하지 않고 숨기는 경우가 대부분이다.
* 주석과 같이 태그 구조 이해에 주 용도로 사용한다.
* 화면에 줄이 보인다고 다 hr이라고 생각하면 안된다. (디자인영역!)
### 그룹 div -> 레이아웃 태그
* 2개 이상의 인라인 or 블록 요소를 묶어주는 그룹 태그이다.
* 포토샵의 '레이어'라고 생각하면 쉽다.
### a (링크태그) -> 하이퍼링크 태그
* 블록태그, 인라인태그가 둘다 가능하다.
* html &lt;a&gt; 요소(앵커요소)는 href 속성을 통해 다른 페이지나 같은 페이지의 어느 위치, 파일, 이메일 주소와 그 외 다른 URL로 연결할 수 있는 하이퍼링크를 만든다.
## 인라인태그
### br (줄바꿈) -> 문서 태그
* 블록 내에서 강제 줄바꿈이 필요한 경우 사용한다.
* 꼭 사용해야 할 때에만 사용해야 한다! -> 줄바꿈이 되면 한 사이트에서 봤을 때 강제로 줄바꿈이 되어서 모양이 이상해진다.
* 보통 글자수가 많지 않은 '제목' 등에 사용하게 된다.
* br태그는 닫힌 태그가 없기 때문에 빈태그이다.
### strong (강조) -> 문서 태그
* 중요성, 심각성 또는 긴급성
* 주로 내용 안에서 강조할 때 사용한다.
* 경고성 문구에 주로 사용한다. ex)19세 이상 관람, 잘못된 접근입니다...
* 제목은 이미 강조라는 뜻을 가지고 있기 때문에 사용하지 않는다.
* 스크린 리더 때 볼륨이 더 커진다.
### em (강조) -> 문서 태그
* 문장 내에서 특정 문맥의 강조할 때 사용한다.
* 단순히 강조할 때 사용한다.
* 스크린 리더 때 볼륨이 더 커진다.
* strong이랑 크게 구분하지는 않으나, 사전적인 내용으로 이해하기
### sub, sup (아래첨자, 위첨자) -> 문서 태그
* b,p 글자의 동그라미가 어디 있는지 확인하면 된다.
### s,del (교체or삭제) -> 문서 태그
* 가격에서 할인 전 금액과 같이 삭제된 부분을 표기한다.
* 보통 del태그를 쓰는 편이다.
### q (짧은 인용문) -> 문서 태그
* p태그 안에 쓰임
* 내용 중 짧은 인용문.
* cite : q와 함께 쓰는 것으로 자료 출처 url주소
### code (명령어 표기) -> 문서 태그
* 컴퓨터가 지원하는 다양한 명령어를 화면 표시할 경우
* &; : 특수문자를 넣겠다는 시작과 끝 단어. &와 ; 안에 lt,gt를 넣으면 특수문자 <>가 들어간다.
### 그룹 span
* 2개 이상의 인라인 요소를 묶을 때 사용한다.
----
### 2025/04/07 | HTML 4일차 | 레이아웃
## `div`와 `span` 그룹태그 사용법
* `div`, `span`
* 웹/앱 레이아웃 방향과 의미에 따라 2개 이상의 요소를 묶어주는 레이아웃 요소
* `div`는 생성시 반드시 그룹을 구분할 수 있는 이름을 설정해야 한다. `span`은 선택!
* 이름 작성 시 주의사항 : 반드시 용도에 맞는 의미있는 영단어 사용!!
* `div` 블록, 인라인 둘다 묶음이 가능하다.
* 기존에 블록 형제가 있다면 인라인태그가 형제로 들어갈 수 없다.
## 태그 + 이름 속성 class, id
* .class : 반복 유형 분류 시 사용, 반복지정가능
* #id : 전체 페이지 중 단 하나의 요소에만 지정 시 사용
* class, id는 태그 관계 없이 모든 태그에 적용할 수 있다.
* 추가정보 -> html에서는 .또는 #은 따로 적지 않고 class, id로 쓴다.
### id란?
* 이 웹페이지에서 '단 하나'다. -> 예) header, footer
* 큰 덩어리 개념으로 생각하면 된다.
* 예를들어, 학생들이 10층에 강의실 1003호를 찾아오는 것
### class란?
* 반복되는 내용 ->글꼴, 색상, 디자인 등
* 예를들어, 우리반에 mbti를 조사한다고 했을 때 각 유형이 여러명 나오는 것
### 하이퍼링크 &lt;a&gt; 절대경로
* 절대경로는 변하지 않는 주소로 쉽게 말해 흔히 알고 있는 웹 주소를 떠올리면 된다.
* [http://naver.com](http://naver.com은) 네이버가 망하지 않는 한 사라지거나 변경되지 않는 주소이다.
* 절대경로는 http:// 웹 프로토콜로 시작한다.
* http뒤에 s가 들어가면 보안이 걸린 웹 프로토콜이다.
* 링크는 가능한 넓게 잡아야 합니다. ‘여기’ 같은 단어 하나로 잡는건 안됌!!
### &lt;a href=""&gt; 링크 주소 속성
* href 속성 안 값은 링크 목적지 주소를 정확히 입력해야 한다.
* 링크주소는 일반적으로 '절대경로', '상대경로'로 나뉜다.
### &lt;a href=""target=""&gt; 링크 주소위치치 속성
* `_blank` : URL을 새로운 창에 표시한다.
* 새로운 탭으로 열린다.
### HTML 구조 공부 순서
1. 클론 코딩 & 클론 디자인할 사이트 정하기
2. 피그마에서 와이어프레임 만들기(레이어, 폴더 이름 주의)
3. 피그잼에 일부 화면 넘겨서 태그 계획하기
4. 계획한 태그를 가족과계에 맞게 트리구조 만들기
5. vs code에서 실제 HTML 작성하기(트리구조 순서에 맞게 바깥쪽->안쪽순서로!)
### 다른 환경에서 git 이어서 작업하기
1. 새폴더 연결하기
2. `git clone 저장소 주소 붙여넣기`
3. `cd 저장소폴더명`로 작성할 main 폴더 연결하기
4. 내용 추가 작성하기
5. `git status`로 저장 파일 확인하기
6. `git add .` 저장하기
7. `git status` 저장확인하기
8. `git commit -m '메모작성'` 작성한 내용 저장하기
9. `git push origin main` 하여 깃허브 업로드
### 학원에서 다시 내려받기
1. `TIL` 폴더 열어주기
2. `git pull origin main` 하여 전체 내려받기 후 수정
3. 동일하게 깃허브에 저장해주기