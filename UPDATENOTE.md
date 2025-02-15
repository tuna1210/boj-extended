## v1.5.3

2021/08/09

**Features**

- 어두운 테마
- - 이미지를 어둡게 변환하여 표시 [(#20)](https://github.com/joonas-yoon/boj-extended/issues/20)
- 채점 현황
- - 채점이 종료되면 몇 퍼센트(%)에서 틀렸는 지 임시로 표시 (해당 페이지의 전역 변수)
- 그룹
- - 그룹 목록에서 내부 메뉴로 바로 이동할 수 있는 링크 추가

**Fixes**

- 제출 현황에서 너비가 떨리는 현상 재수정 [(#18)](https://github.com/joonas-yoon/boj-extended/issues/18)
- - `display` 여부를 인라인 스타일에서 클래스로 변경
- 복사 버튼의 CSS 제거
- - 소스 보기 화면에서 다르게 보여서 제거
- 어두운 테마
- - 드롭 다운의 아이템 폰트 색상 변경 [(#21)](https://github.com/joonas-yoon/boj-extended/issues/21)
- - 일부 배경이 어둡게 남은 것 변경 (depth에 따른 밝기 조정)

## v1.5.2

2021/07/26

**Fixes**

- 제출 현황에서 너비가 떨리는 현상 수정 [(#18)](https://github.com/joonas-yoon/boj-extended/issues/18)
- - 제출 결과 너비를 고정

## v1.5.1

2021/07/25

**Features**

- 유저 프로필 페이지에 VS 버튼 추가

**Changes**

- VS 페이지에서 유저 아이디 클릭 시 프로필로 연결

## v1.5.0

20201/07/25

**Features**

- 유저 VS 추가
- - 과거 URL(`/vs/user1/user2`)를 그대로 지원

## v1.4.6

20201/07/02

**Changes**

- 유저 프로필의 문제 표시 수 수정 [(#16)](https://github.com/joonas-yoon/boj-extended/issues/16)
- - 더보기 추가

**Fixes**

- 그룹 내의 스코어 보드에 CSS가 적용되지 않은 것 수정 [(#17)](https://github.com/joonas-yoon/boj-extended/issues/17)

## v1.4.5

20201/05/05

**Features**

- 제출 결과 텍스트의 숫자 치환 추가 [(#15)](https://github.com/joonas-yoon/boj-extended/issues/15)
- - '채점 중'과 '부분 점수'의 텍스트 포맷에 숫자 사용 가능 (치환자는 `:number:`)

**Changes**

- 제출 현황의 컬럼 너비 수정

## v1.4.4

20201/02/21

**Changes**

- `db.json`에 업데이트 시간 추가
- 로컬 DB에 없는 문제 정보는 원격 저장소(github)에서 가져오도록 변경 [(#11)](https://github.com/joonas-yoon/boj-extended/issues/11)

**Fixes**

- CSS 일부 수정
- - 스크롤 바, 즐겨찾기 버튼, 복사 버튼
- 오타 수정

## v1.4.3

2021/02/06

**Features**

- 문제 화면에서 해당 문제의 질문 개수 표시

**Fixes**

- GA 코드 버그 수정
- 게시판에서 문제 제목 오류 수정

## v1.4.2

2021/01/31

**Features**

- Google Analytics 추가
- 게시판에서도 문제 제목 표시 [(#6)](https://github.com/joonas-yoon/boj-extended/issues/6)

**Changes**

- 어두운 테마를 약간 밝게 조정

**Fixes**

- 어두운 테마를 불러오는 방식 수정 [(#7)](https://github.com/joonas-yoon/boj-extended/issues/7)
- - `localStorage`로 깜빡임 현상 해결
- babel 빌드 설정 수정

## v1.4.1

2021/01/30

**Features**

- 문제 타이머 추가

**Fixes**

- `chrome.stroage.sync`의 불필요한 동기화를 줄임
- - Config 클래스의 버퍼를 먼저 참조하고, 변화가 생기면 동기화 (딜레이 낮춤)
- - background로 옮겨서 메시지 전달로 대응 [(#5)](https://github.com/joonas-yoon/boj-extended/issues/5)
- 제출 결과 텍스트의 원본을 유지 (숨김)

## v1.4.0

2021/01/27

**Features**

- 제출 결과 텍스트를 변경 가능
- - 일부 결과는 보류 (채점 중, 부분 점수, 런타임 에러)
- 옵션 페이지 추가 [(#1)](https://github.com/joonas-yoon/boj-extended/issues/1)
- - '확장 프로그램의 옵션' 또는 'BOJ의 설정 페이지의 왼쪽 메뉴'에서 접근 가능

## v1.3.1

2021/01/25

**Features**

- 넓게 보기 추가
- 채점 현황
- - 내 제출 결과에는 강조 표시 (파란색 굵은 수직선)
- - 런타임 오류의 도움말을 간단히 표시 (도움말에서 긁어옴)
- 그룹 멤버 정렬 추가

**Fixes**

- 어두운 테마 버그 수정

## v1.3.0

2021/01/25

**Features**

- 어두운 테마 추가
- Github action으로 빌드 자동화

## v1.2.1

**Fixes**

- 코드 안정화

## v1.2.0

**Features**

- 채점 현황에도 문제 제목을 표시

## v1.1.0

2021/01/24

**Fixes**

- 코드 리팩토링
- Github action으로 문제 DB를 사이트와 동기화

## v1.0.0

2021/01/21

**Features**

- 유저 프로필 페이지에서 문제 번호와 문제 제목 표시
- `chrome.storage.sync`에 저장하여 설정 동기화
