# PROMPTS: 복사해서 붙여 넣는 프롬프트 / Copy-paste prompts

**준비:** [dh-lab.zip](https://github.com/jhoh-bigglz/skku-vibecoding-dickens/raw/main/dh-lab.zip)을 풀고, VS Code에서 `dh-lab` 폴더를 연 뒤(File → Open Folder) 그 터미널에서 `vixcode`를 실행합니다. 다른 폴더에서 실행하면 data/ 파일을 찾지 못합니다.
**Setup:** unzip dh-lab.zip, open the `dh-lab` folder in VS Code (File → Open Folder) and run `vixcode` in its terminal. Started in another folder, it cannot find the data/ files.

**순서:** ① 메모장에 내가 알고 싶은 것을 한 줄로 쓴다 → ② 아래 상자 하나를 통째로 복사해 `[ ]` 자리에 그 한 줄을 넣는다 → ③ Vix Code(또는 아무 AI 채팅)에 붙여 넣는다 → ④ **실행하지 말고, 받은 계획을 읽고 이상한 곳을 찾는다.**
**Steps:** ① write one line in a notepad: what do you want to know? → ② copy one whole box and put that line in `[ ]` → ③ paste it into Vix Code (or any AI chat) → ④ **don't run anything; read the plan and find what's wrong.**

한국어(KO)나 영어(EN) 중 하나만 쓰세요. / Use the KO box or the EN box, not both.

---

## P1 · 계획만 받기 / Plan only (수업 실습 / in class)

**KO**
```text
목적: 디킨스 「거리 — 아침」과 「거리 — 밤」을 비교해 [내가 알고 싶은 것]을 알고 싶다.
자료: 이 폴더의 data/streets_morning.txt 와 data/streets_night.txt 만 쓴다. 인터넷에서 내려받지 않는다.
아직 파일을 만들거나 실행하지 말고 계획만 세워 줘: 단계, 단계마다 만들 파일, 맞게 됐는지 확인하는 방법.
```

**EN**
```text
Goal: compare Dickens's "The Streets—Morning" and "The Streets—Night" to find out [your question].
Data: use only data/streets_morning.txt and data/streets_night.txt in this folder. Do not download anything.
Don't create or run anything yet. Just give me a plan: the steps, the files each step will make, and how to check that each step worked.
```

**계획을 읽을 때 볼 것 / Read the plan for:**
- [ ] 내 질문을 정말 숫자로 바꿨나? 무엇을 세는가? / Did it turn my question into something countable? What exactly is counted?
- [ ] 단어 목록을 누가 정하나? AI가 마음대로 늘리지 않나? / Who chooses the word lists? Does the AI add words on its own?
- [ ] 두 글의 길이를 맞춰 비교하나(1,000단어당 등)? / Does it compare at the same scale (e.g., per 1,000 words)?
- [ ] 단계마다 확인 방법이 있나? / Does every step have a check?
- [ ] 폴더 밖에 쓰거나 인터넷에 접속하지 않나? / Does it stay inside the folder and offline?

---

## P2 · (선택) 계획대로 실행 / (Optional) Run the plan — 수업 뒤 / after class

**KO**
```text
위 계획에서 [고칠 점]을 고친 뒤 실행해 줘. 파이썬과 matplotlib만 쓰고, 결과는 results/ 폴더에 표(csv) 하나와 그래프(png) 하나로 남겨 줘.
파일은 UTF-8로 읽고 써 줘. 그래프의 제목과 축 이름은 영어로 써 줘(한글은 네모로 깨질 수 있어).
숫자는 지어내지 말고, 결과를 세 줄로 해석하되 한계를 하나 꼭 적어 줘.
윈도우에서는 python 대신 py로, 맥에서는 python3로 실행해.
```

**EN**
```text
Fix [what to change] in the plan above, then run it. Use only Python and matplotlib, and save one table (csv) and one chart (png) in a results/ folder.
Read and write files as UTF-8. Write the chart title and axis labels in English.
Don't invent numbers. Give a three-line reading of the result, including one limitation.
On Windows, run py instead of python; on Mac, run python3.
```

---

자료: Project Gutenberg #882(1903 Chapman & Hall판)를 수업용으로 정리한 사본(저작권 만료 텍스트). Source: cleaned copy of Project Gutenberg #882 (public domain).
