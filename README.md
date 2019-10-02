# 영어단어봇 제작
영어 교과서 본문에 나오는 단어를 학습하는데 도움을 주는 챗봇을 만들어봅니다.

## 제작 단계

### 영어 단어 준비

* 영어 단어 목록 작성
  + 중학교 단어 (20개): treatment, drown, rope, breathe, lay, come around, hold on to, insect, try to, upward, pain, check for, injured, wrap, support, keep A from B, worse, aid, accident, bone (출처: 천재 중3 영어교과서, Lesson 9, The ABCs of First Aid) 
  + 고등학교 단어 (26개): host, harsh, immediately, signal, slight, mature, risky, region, measure, influence, instinct, inclined, consequence, identify, connection, experiment, instrument, strengthen, adolescent, period, merely, dismiss, phase, insignificant, stage, insight (출처: 능률 고1 영어교과서, Lesson 8, How Teens Make Decisions)

* 각 단어의 자료 수집 및 정리
  + 항목: 발음, 품사, 의미, 영영풀이, 파생어, 파생전단어, 유의어, 반의어, 다른품사, 숙어, 단어관련이미지, 교과서예문, 예문해석
  + 위 항목은 필요에 따라 줄이거나 늘릴 수 있습니다.
  + 발음의 경우 발음기호와 함께 단어를 발음한 오디오 파일을 확보합니다.
  + 단어 자료를 아래한글이나 워드 파일로 작성할 수도 있으나 단어 관련 데이터를 수집하고 활용한다는 측면에서 엑셀 등과 같은 스프레드시트 파일로 작성하는 것을 추천합니다.

* 각 단어별 객관식 문제 제작
  + 항목: 지시문, 보기1, 보기2, 보기3, 보기4, 틀린보기힌트 3개, 정답, 문제설명, 문제관련추가자료
  + 객관식 문제가 그렇듯이 지시문과 4개의 보기는 한꺼번에 제시됩니다.
  + 틀린 보기를 선택했을 경우 보여줄 수 있는 힌트를 3개 준비합니다. 정답 보기를 선택했을 경우에는 문제설명을 보여줍니다.
  + 문제 관련하여 추가적으로 보여줄 내용이 있으면 관련 자료를 준비합니다.

### 단비(챗봇빌더) 사용 준비

* 단비 계정 생성
  + 단비 웹사이트: [https://danbee.ai/][https://danbee.ai/] 
  + 이미지
* 단비 계정 로그인
* 단비 화면 둘러보기
* 단비의 샘플 챗봇 사용해보기

### 챗봇 제작

* 빈 챗봇 생성하기
* 챗봇 썸네일, 챗봇 이름, 챗봇 카테고리, 챗봇 설명 작성
* 현재 챗봇 확인과 왼쪽 메뉴 살펴보기
* 기본 답변 중 Welcome Message, Default Fallback 수정 및 테스트
* 대화 채널 중 Frogue 테스트 (URL열기)
* 대화목록 선택
* 첫 intent 생성
  + 이름: greeting
  + 버튼: 영어단어봇 인사 드림
  + chatflow연결 후 대화흐름 생성 (greeting이라는 대화흐름chatflow가 자동적으로 생성됨)
* 첫 chatflow (greeting) 수정
* 기본 답변 중 Welcome Message의 연결 chatflow로 greeting 선택
* question_01 intent 및 question_01 chatflow 생성
  + question_01 chatflow 세부 대화흐름 작성
  + question_01 chatflow 파라미터 설정 및 세팅
