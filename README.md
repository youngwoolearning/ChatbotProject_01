# 영어단어봇 제작
영어 교과서 본문에 나오는 단어를 학습하는데 도움을 주는 챗봇을 만들어봅니다.

## 제작 단계

### 영어 단어 준비
1. 영어 단어 목록 작성
2. 각 단어의 자료 수집 및 정리
3. 각 단어별 객관식 문제 제작

### 단비(챗봇빌더) 사용 준비
1. 단비 계정 생성
2. 단비 계정 로그인
3. 단비 화면 둘러보기
4. 단비의 샘플 챗봇 사용해보기

### 챗봇 제작
1. 빈 챗봇 생성하기
2. 챗봇 썸네일, 챗봇 이름, 챗봇 카테고리, 챗봇 설명 작성
3. 현재 챗봇 확인과 왼쪽 메뉴 살펴보기
4. 기본 답변 중 Welcome Message, Default Fallback 수정 및 테스트
5. 대화 채널 중 Frogue 테스트 (URL열기)
6. 대화목록 선택
7. 첫 intent 생성
 - 이름: greeting
 - 버튼: 영어단어봇 인사 드림
 - chatflow연결 후 대화흐름 생성 (greeting이라는 대화흐름chatflow가 자동적으로 생성됨)
8. 첫 chatflow (greeting) 수정
9. 기본 답변 중 Welcome Message의 연결 chatflow로 greeting 선택
10. question_01 intent 및 question_01 chatflow 생성
 - question_01 chatflow 세부 대화흐름 작성
 - question_01 chatflow 파라미터 설정 및 세팅
