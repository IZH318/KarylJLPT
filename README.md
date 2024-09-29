# 캬루와 함께하는 JLPT
![녹화_2024_09_30_06_02_07_419 mp4_snapshot_00 00 000](https://github.com/user-attachments/assets/83e933ba-6f00-4b80-9ba5-dc9ce0d018fb) <BR>
(🖥 메인 화면) <BR> <BR>

캬루와 함께 JLPT 공부 할 수 있는 웹 사이트입니다. <BR>
🔗 URL: https://izh318.github.io/KarylJLPT/ <BR> <BR>

필수 기초 단어뿐만 아니라, JLPT N5부터 JLPT N1까지 다양한 난이도를 선택할 수 있습니다. <BR>
(* 2024-09-06 기준 총 6,877 단어 등록)

<BR> <BR> <BR>

## 🔍 웹 사이트 미리보기
![녹화_2024_09_30_06_07_35_180 mp4_snapshot_00 02 458](https://github.com/user-attachments/assets/9876cd7d-cfeb-438c-9f70-384a76f080a5) <BR>
(🖥 웹 사이트 첫 로딩 화면) <BR> <BR>

![녹화_2024_09_30_06_02_07_419 mp4_snapshot_00 00 000](https://github.com/user-attachments/assets/83e933ba-6f00-4b80-9ba5-dc9ce0d018fb) <BR>
(🖥 메인 화면) <BR> <BR>

![녹화_2024_09_30_06_02_07_419 mp4_snapshot_00 05 654](https://github.com/user-attachments/assets/c6a3e3fe-16f7-422b-a239-a8592e8c15c0) <BR>
(🖥 난이도 문제 수 설정 화면) <BR> <BR>

![녹화_2024_09_30_06_02_07_419 mp4_snapshot_00 40 468](https://github.com/user-attachments/assets/e8458e32-e201-4add-85a3-ba8b923a28f8) <BR>
(🖥 난이도 문제 수 설정 후 로딩 화면) <BR> <BR>

![녹화_2024_09_30_06_02_07_419 mp4_snapshot_01 56 687](https://github.com/user-attachments/assets/4fec30c1-8396-4894-9893-92586bef26bf) <BR>
(🖥 사용자 지정 문제 난이도, 문제 수, 문제 출제 유형 설정 화면) <BR> <BR>

![녹화_2024_09_30_06_02_07_419 mp4_snapshot_02 10 435](https://github.com/user-attachments/assets/c0f877f0-601c-42e8-9235-b4b261e60a82) <BR>
(🖥 사용자 지정 문제 난이도, 문제 수, 문제 출제 유형 설정 후 로딩 화면) <BR> <BR>

![녹화_2024_09_30_06_02_07_419 mp4_snapshot_00 41 334](https://github.com/user-attachments/assets/57ebead5-0955-4740-ae63-a35867bc7106) <BR>
(🖥 문제, 선택지, 추가 기능 반환 화면) <BR> <BR>

![녹화_2024_09_30_06_02_07_419 mp4_snapshot_02 14 198](https://github.com/user-attachments/assets/21fd9d34-f97e-4626-81b5-934a222d57e7) <BR>
(🖥 결과 로딩 화면) <BR> <BR>

![녹화_2024_09_30_06_02_07_419 mp4_snapshot_00 57 251](https://github.com/user-attachments/assets/4954d964-3236-402c-b411-77f92a57ae2b) <BR>
(🖥 결과 화면) <BR> <BR>

![녹화_2024_09_30_06_02_07_419 mp4_snapshot_00 59 867](https://github.com/user-attachments/assets/08a7fda4-3262-4508-b4eb-bd7a21fb1d92) <BR>
(🖥 정오표 화면 - 오답 항목 강조 기능 활성화 (기본값)) <BR> <BR>

![녹화_2024_09_30_06_02_07_419 mp4_snapshot_01 33 064](https://github.com/user-attachments/assets/af9743d5-d76c-4c11-b01d-fb9f11996b50) <BR>
(🖥 정오표 화면 - 오답 항목 강조 기능 활성화 (강조 색 변경)) <BR> <BR>

![녹화_2024_09_30_06_02_07_419 mp4_snapshot_01 36 342](https://github.com/user-attachments/assets/97f2e4e0-b109-4dcf-86e4-f37862d70f83) <BR>
(🖥 정오표 화면 - TTS 목록 선택) <BR> <BR>

![녹화_2024_09_30_06_02_07_419 mp4_snapshot_01 47 332](https://github.com/user-attachments/assets/0fe3f39c-eb9f-42b6-865f-6096fc4aeb79) <BR>
(🖥 정오표 화면 - 인쇄) <BR> <BR>

![녹화_2024_09_30_06_02_07_419 mp4_snapshot_00 35 432](https://github.com/user-attachments/assets/7d6c6094-b2aa-46d2-b1bd-c863866446ed) <BR>
(🖥 메인 이동 화면)

<BR> <BR> <BR>

## 🛠️ 기능

### 중요 기능 정의

1. **데이터 구조 정의**:
   - `const questions = {};`: 문제를 난이도별로 저장
   - `let score = 0;`: 사용자 점수 저장
   - `let selectedDifficulty = "";`: 현재 선택된 난이도 저장
   - `let displayedAnswers = [];`: 현재 질문에 대한 보여진 답변 목록 저장
   - `let selectedDifficulties = [];`: 사용자가 선택한 난이도의 목록 저장
   - `let totalQuestions = 0;`: 전체 문제 수 저장

2. **UI 초기화 (`resetElements`)**:
   - 메인 화면의 캐릭터 이미지를 표시하고, 각종 체크박스와 텍스트 박스를 초기화
   - 특정 날짜에 Confetti 효과를 실행

3. **로딩 화면 표시 (`showLoadingScreen`, `hideLoadingScreen`)**:
   - `showLoadingScreen`: 로딩 화면을 보이게 설정
   - `hideLoadingScreen`: 비동기적으로 로딩 화면을 숨김

4. **문제 로딩 (`loadQuestions`)**:
   - CSV 파일(`Questions.csv`)을 비동기로 가져옴
   - 네트워크 응답이 정상적이지 않으면 오류 메시지를 콘솔에 출력
   - PapaParse 라이브러리를 사용하여 CSV 파일을 파싱, 각 문제를 난이도별로 `questions` 객체에 저장

5. **특정 날짜 확인 (`isTodaySpecialDate`)**:
   - 현재 날짜가 특정 날짜인지 확인 후 해당 날짜일 경우 효과 적용

6. **페이지 로드 시 문제 데이터 로드 (`window.onload`)**:
   - 페이지가 로드될 때 로딩 화면을 표시하고, 문제 데이터를 로드한 후 로딩 화면을 숨김
   - UI 요소를 초기화하여 준비 상태로 만듦

<BR>

### 문제 설정

- 사용자가 난이도를 선택하면 확인 팝업 창 표시
- '예'를 클릭 시 문제 수 설정(사용자 지정 난이도 선택 시 난이도 및 문제 수 설정) 창 표시, '아니요'를 클릭 시 메뉴로 이동
- 난이도 및 문제 수 설정 창 표시에서 취소 버튼 클릭 시 메인 메뉴로 이동

#### 사용자 지정 문제 선택 시 다음 기능 제공

- 사용자가 난이도를 체크박스로 선택하여 다중 난이도 지정 가능
- 출제 유형 선택 (라디오 버튼)
    - 난이도별: 각 난이도에서 무작위로 문제를 선택
    - 총 무작위: 선택된 모든 문제에서 무작위로 문제 선택

#### 문제 설정 공통 사항

- 입력에서 온점(`.`) 자동 삭제
- 마우스 휠로 숫자 증가 또는 감소
- 발음 표시 여부 설정 가능
- 최대 및 최소값을 설정하여 사용자가 입력할 수 있는 범위 제한
    - 난이도 미 선택: 설정 창으로 이동
    - 입력값이 숫자가 아닐 때: 입력 값 초기화
    - 1 이하: 입력 값 초기화
    - 선택된 전체 문제 수 초과: 선택된 전체 문제 수의 최대값으로 설정

<BR>

### 퀴즈

- 사용자가 설정한 값(* 난이도, 문제 수, (사용자 지정 문제 전용) 출제 유형)을 기준으로 문제 출제
- 문제와 답변 선택지(4지선다)를 무작위로 섞어서 배치
- 문제 건너뛰기 버튼 클릭 시 오답으로 처리
- 처음으로 돌아가기 버튼 클릭 시 메인 화면으로 이동
- 화면 하단 진행 바 표시 (* 현재 문제 번호 / 전체 문제 수)
- 문제를 다 풀면 결과 화면 표시

<BR>

### 결과

- 점수 표시
- 각 점수(0점, 10점 단위)별 이미지 전환
- 점수가 90점 이상일 때 Confetti 효과 재생
- 점수가 90점 이상, 문제 수가 선택한 난이도의 전체 문제 수 80% 이상일 경우 상장 다운로드 버튼을 표시

- 상장 다운로드 버튼 클릭 시 이름 입력 팝업 창 표시
- 상장 다운로드 시 난이도, 이름, 현재 시스템 날짜를 기록하여 *.png 이미지로 저장

- 정오표 버튼 클릭 시 정오표 창 표시
- 번호, 과목, 문제, 발음, 보기, 정답, 선택, 정오 내용 표시 (* 단, 인쇄할 때는 발음 열 미 표시)
- 오답 항목 강조 기능 활성화 시 정오가 X인 항목의 행에 강조 색으로 배경 색 지정
- TTS 모델은 기본적으로 ja-JP 선택, 드롭박스를 통해 다양한 TTS 모델 선택 가능
- 인쇄 버튼 클릭 시 정오표 인쇄 가능

<BR> <BR> <BR>

## 🥇 상장 예시
( 🧪 테스트 환경: 모든 난이도 선택, 시스템 날짜 2024년 09월 30일) <BR> <BR>

![2024930034922_캬룽☆](https://github.com/user-attachments/assets/a5acc456-8ee4-4f7c-bd7b-e431157df26e) <BR>
(예시 01) 이름이 입력 되는 공간(밑줄) 안에 글자가 들어오는 경우, 지정 폰트 크기 유지 <BR> <BR>

![2024930034852_너와 만나고, 너와 떠나는 배신의 그 끝에서](https://github.com/user-attachments/assets/d735684b-5269-43be-aaaa-4edda8356c23) <BR>
(예시 02) 이름이 입력 되는 공간(밑줄) 밖으로 글자가 나가는 경우, 입력 된 글자 수에 맞게 적절히 폰트 크기 조절 <BR>

<BR> <BR> <BR>

## 📝 출처

- **단어 리소스 원본**:  
  켜자마자 일본어 (강제로 일본어공부-JLPT, JPT) <BR>
  🔗 URL: https://play.google.com/store/apps/details?id=net.dayword.jpkr <BR>

- **단어 리소스 추출 도구** (* 자체 제작 및 수정):  
  (Word Apps) 켜자마자 일본어 DB 복호화 및 추출 <BR>
  🔗 URL: https://github.com/IZH318/Word-Apps-JLPT-JPT-Decryption-and-extraction-tools <BR> <BR>

- **상장 이미지 리소스**:  
  gdoc.io <BR>
  🔗 URL: https://gdoc.io/certificate-templates/certificate-of-completion-free-google-docs-template/ <BR>
  
  Freepik <BR>
  🔗 URL: https://www.freepik.com/free-vector/flat-design-first-class-stamp-collection_32684752.htm <BR> <BR>

- **폰트**:  
  Allison <BR>
  🔗 URL: https://fonts.google.com/specimen/Allison <BR>
  
  Noto Serif Korean <BR>
  🔗 URL: https://fonts.google.com/noto/specimen/Noto+Serif+KR <BR> <BR>

- **메인 캐릭터 및 배경 이미지 리소스**:  
  株式会社Cygames © プリンセスコネクト！Re:Dive (プリコネR) <BR>

<BR> <BR> <BR>
