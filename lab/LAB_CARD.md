# 디킨스 실습실 / Dickens Lab
**『Sketches by Boz』를 코드로 읽기 · 선택 실습 · 제출 없음**
*Reading Sketches by Boz with code · optional · no submission*
SKKU 특강 "Vibe Coding in the Humanities" (2026-10-16) 후속 / follow-up

## 무엇인가요? / What is it?
- 교수님 슬라이드의 과제 목록 6가지를 Google Colab 노트북 하나(`dickens_lab.ipynb`)로 해 봅니다. 특강에서 끝까지 하지 못한 부분입니다.
  The six tasks from the professor's task list, in one Colab notebook — the parts the lecture did not finish.
- 과제마다: 연구 질문 한 줄 → AI에 붙여 넣을 프롬프트(한/영) → 막히면 보낼 고치기 프롬프트 예시 → 실행되는 참고 코드 → "나는 무엇을 정했나?"
  Each task: a research question → a prompt for any AI (KO/EN) → an example fix-it prompt for when it goes wrong → working reference code → "What did you decide?"
- 방법: AI로 코드를 만들고, 실행하고, 고칩니다. 그다음 참고 코드 결과와 비교합니다.
  Method: generate code with an AI, run it, fix it, then compare with the reference.

## 여는 법 / How to open (설치 없음 / nothing to install)
1. https://colab.research.google.com 에 구글 계정으로 접속 / sign in with a Google account
2. **File → Upload notebook** → `dickens_lab.ipynb` 선택 / choose the file
   또는 링크로 열기 / or open the link: https://colab.research.google.com/github/jhoh-bigglz/skku-vibecoding-dickens/blob/main/lab/dickens_lab.ipynb
   링크로 열면 첫 실행 때 경고 창이 뜹니다. **Run anyway**를 누르고, 고친 내용을 남기려면 **File → Save a copy in Drive**. / Via the link: click **Run anyway** at the warning; **File → Save a copy in Drive** keeps your edits.
3. 위에서부터 셀 실행(▶ 또는 Shift+Enter). **섹션 0을 먼저.** / Run cells from the top. **Section 0 first.**
   뒤 과제는 앞 과제의 변수를 씁니다. 중간 과제부터 하려면 먼저 **Runtime → Run all**(모두 실행). / Later tasks use earlier variables: to start mid-way, first use **Runtime → Run all**.

## 과제 체크리스트 / Task checklist (총 60–90분 / min)
- [ ] **0. 준비** 텍스트 내려받기 / Setup: download the text — 5분
- [ ] **1. 정제** Gutenberg 머리말·꼬리말·메타데이터 제거, 원래 56편만 남기기(1903년판에 함께 묶인 다른 작품 3종 제외) / Strip header, footer, metadata; keep the original 56 (drop the 3 later works bundled in the file) — 10분
- [ ] **2. 불용어** 불용어 제거 + 화이트리스트(Mr, Mrs, Miss, Sir, Lord). 그리고 is·are·we vs I·said·was: 지운 단어가 장르 신호라면? / Stopwords + whitelist; function words as genre signals — 15분
- [ ] **3. 장소** 언급된 장소와 빈도 / Places and frequencies — 10분
- [ ] **4. 거리** 언급된 거리와 빈도 ('Monmouth-street' 같은 하이픈·소문자 표기 처리) / Streets and frequencies (hyphens, lowercase) — 10분
- [ ] **5. 연어** 로그우도비·PMI, 이름을 뺄 때와 둘 때 / Collocations with and without names — 10분
- [ ] **6. 토픽** NMF(선택: LDA), 300단어 조각, 이름을 뺄 때와 둘 때 / Topic modelling, 300-word chunks — 15분

한 과제만 해도 충분합니다. 막히면 그 과제의 참고 코드를 실행하고 다음으로 넘어가세요.
One task is enough. If stuck, run the reference cell and move on.

## 제출 없음 / No submission
- 점수도 확인도 없습니다. 결과 파일(`places.csv`, `streets.csv` 등)과 "무엇을 정했나?"에 대한 답은 **기말 프로젝트의 방법론 메모**로 쓰세요.
  Nothing is graded or collected. Keep your files and decisions as notes for your final project.
- 네트워크와 지도는 다음 수업에서 합니다. 이 실습의 장소·거리·이름 목록이 그 입력이 됩니다.
  Networks and maps come in the next classes; your lists from this lab are their input.

## 개인정보 / Privacy
- 노트북은 여러분의 구글 계정 Colab에서 실행되고, 저작권이 끝난 공개 텍스트(Project Gutenberg #882)만 씁니다. 연사나 학교로 아무것도 전송되지 않습니다.
  It runs in your own Colab and uses only a public-domain text. Nothing is sent to the speaker or the school.
- AI에 이름·학번·연락처 같은 개인정보나 다른 사람의 글을 붙여 넣지 마세요.
  Do not paste personal data or other people's writing into an AI.
- Colab 파일은 세션이 끝나면 지워집니다. 필요한 결과는 내려받으세요.
  Colab files are deleted when the session ends; download what you need.
