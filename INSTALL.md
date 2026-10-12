# 실습 준비 안내 / Setup guide

**10/16(금) 특강 "Vibe Coding in the Humanities" · 모두 선택 사항 / everything here is optional**

수업 중 실습은 짧습니다. AI에게 디킨스 글을 분석할 **계획을 받아 읽어 보는 것**입니다. 노트북을 가져와 직접 해 보고 싶은 분만 준비하세요. 처음이면 20–40분 걸립니다. 강의실 Wi-Fi로는 여러 명이 동시에 설치하기 어려우니 **집에서 미리** 해 주세요.
*The in-class hands-on is short: you ask an AI for a **plan** to analyse a Dickens text and read it critically. Prepare only if you want to try it on your own laptop. First-time setup takes 20–40 minutes; please do it **at home** (the classroom Wi-Fi cannot handle many installs at once).*

설치가 안 됐거나 노트북이 없어도 괜찮습니다. **그냥 오세요.** 옆 사람과 함께하거나 화면을 보며 참여할 수 있습니다.
*No laptop, or setup failed? **Just come.** You can pair up or follow on screen.*

---

## 0. 무엇을 준비할지 고르기 / Choose your path

| | 무엇 / What | 준비 / Prepare |
|---|---|---|
| **A** | **Vix Code** (무료 AI 코딩 에이전트) / a free AI coding agent | 아래 1–3단계 / Steps 1–3 below |
| **B** | 이미 쓰고 있거나 가입할 예정인 **코딩 AI** (예: Claude Code, OpenAI Codex, Gemini CLI, Cursor) / a coding AI you already use or plan to subscribe to | 그 도구의 안내대로 설치하고, 1단계의 실습 폴더를 그 도구로 여세요 / install it as its docs say and open the lab folder from Step 1 with it |
| **C** | **AI 채팅만** (ChatGPT, Gemini, Claude 웹 등) / **just an AI chat** | 설치 없음. 수업 중 계획 받기 실습은 이것으로도 됩니다 / nothing to install; enough for the in-class planning exercise |

**Python은 선택입니다.** AI가 만든 코드를 **내 노트북에서 직접 실행**해 보려면 필요합니다(4단계). 수업 중 실습(계획 받기)에는 필요 없습니다. *Python is optional: you need it only to **run** the AI's code on your own laptop (Step 4), not for the in-class exercise.*

수업 뒤 혼자 더 해 보는 **선택 Lab**은 Google 계정만 있으면 설치 없이 Colab에서 열립니다: [Colab에서 열기 / Open in Colab](https://colab.research.google.com/github/jhoh-bigglz/skku-vibecoding-dickens/blob/main/lab/dickens_lab.ipynb) (제출 없음 / nothing to submit)

---

## 1. 실습 파일 받기 / Get the lab files (A·B)

1. [**dh-lab.zip**](https://github.com/jhoh-bigglz/skku-vibecoding-dickens/raw/main/dh-lab.zip)을 받아 바탕화면에 압축을 풉니다. *Download **dh-lab.zip** and unzip it to your Desktop.*
2. `dh-lab` 폴더 안에 `PROMPTS.md`가 바로 보이면 됩니다. Windows에서 `dh-lab` 안에 `dh-lab`이 또 있으면 **안쪽 폴더**를 쓰세요. *You should see `PROMPTS.md` right inside `dh-lab`. On Windows, if there is a `dh-lab` folder inside `dh-lab`, use the **inner** one.*
3. 안에는 「거리 — 아침」·「거리 — 밤」 텍스트(Project Gutenberg 원문을 수업용으로 정리한 사본), 실습 프롬프트, Lab 노트북이 있습니다. *It holds the two Dickens texts (cleaned copies of the Project Gutenberg original), the prompts and the lab notebook.*

## 2. 프로그램 설치 / Install the programs (A)

1. **VS Code**: https://code.visualstudio.com
2. **Node.js (LTS)**: https://nodejs.org
   - 설치 중 "Automatically install the necessary tools" 체크박스가 나오면 **체크하지 마세요.** *If you see "Automatically install the necessary tools", leave it **unchecked**.*
3. **Windows만 / Windows only — Git for Windows**: https://git-scm.com/downloads/win
   - 모든 화면에서 기본값 그대로 Next. 설치가 끝나면 **컴퓨터를 한 번 재시작**하세요. *Accept all defaults, then **restart your computer** once.*
4. **Mac만 / Mac only — 개발자 도구 / developer tools**: Vix Code 설치기가 `python3`를 씁니다. 터미널에서 아래를 입력하세요. "개발자 도구 설치" 창이 뜨면 **설치**를 누르세요(5–15분). *The Vix Code installer needs `python3`. Type this in Terminal; if a developer-tools window appears, click **Install** (5–15 min).*
   ```
   python3 --version
   ```

## 3. Vix Code 설치 / Install Vix Code (A)

2단계를 모두 마친 뒤 **새** 터미널을 여세요. Windows는 **PowerShell**을 쓰세요(cmd는 안 됩니다). *After Step 2, open a **new** terminal. On Windows use **PowerShell**, not cmd.*

- **Mac** (터미널 / Terminal)
  ```
  curl -fsSL https://vixcode.ai/install.sh | bash
  ```
- **Windows** (PowerShell)
  ```
  irm https://vixcode.ai/install.ps1 | iex
  ```
- 브라우저가 열리면 **2분 안에** 로그인하세요(GitHub 또는 Google 계정). 시간을 넘기면 터미널에 `vixcode-login`을 입력합니다. *A browser opens: log in **within 2 minutes** (GitHub or Google account). If it times out, type `vixcode-login`.*
- 설치가 끝나면 Vix Code가 자동으로 켜집니다. `/exit`를 입력해 종료하세요. *Vix Code starts by itself after installing. Type `/exit` to close it.*

### 동작 확인 / Check that it works (5분 / 5 min)
1. VS Code를 **완전히 종료했다가** 다시 켭니다. *Fully quit VS Code and reopen it.*
2. File → Open Folder로 1단계의 `dh-lab` 폴더를 엽니다. *Open the `dh-lab` folder from Step 1 (File → Open Folder).*
3. Terminal → New Terminal을 열고 `vixcode`를 입력한 뒤, 다음 문장을 넣습니다. *Open Terminal → New Terminal, type `vixcode`, then enter:*
   ```
   이 폴더에 hello.txt 파일을 만들고 그 안에 hello라고 써 줘.
   ```
   *(English: Create a file hello.txt in this folder and write hello in it.)*
4. 파일을 만들어도 되는지 물으면 Enter(또는 1/Yes)를 누릅니다. 답이 오기까지 1–2분 걸릴 수 있습니다. **VS Code 왼쪽 파일 목록에 `hello.txt`가 생기면 준비가 끝난 것입니다.** *Approve with Enter (or 1/Yes); replies can take 1–2 minutes. **You're ready when `hello.txt` appears in the file list.***

설치 결과는 따로 알려 주지 않아도 됩니다. *No need to report back.*

## 4. (선택) Python: 코드를 직접 실행하려면 / (Optional) Python, to run code yourself

수업 뒤 AI가 만든 분석 코드를 내 노트북에서 실행해 보고 싶은 분만 설치하세요. *Only if you want to run the AI's analysis code on your own laptop after class.*

- **Mac:** 2-4단계의 `python3`로 충분합니다. *The `python3` from Step 2-4 is enough.*
- **Windows:** https://www.python.org/downloads/ 에서 **"Download Python install manager"** 버튼을 누릅니다. *Click the **"Download Python install manager"** button.*
  1. 받은 파일을 실행해 **Install**을 누릅니다. *Run the file and click **Install**.*
  2. 영어 질문이 나오는 검은 창이 뜨지 않으면 시작 메뉴에서 **Python install manager**를 실행합니다. *If no black window with questions appears, start **Python install manager** from the Start menu.*
  3. **PATH 질문**(`Add commands directory to your PATH now? [y/N]`)에만 **`y`**를 입력하고 Enter. *For the **PATH question** only, type **`y`** and press Enter.*
  4. **다른 질문은 모두 그냥 Enter.** Python을 내려받는 동안 1–2분 기다립니다. 더 묻지 않고 창이 닫히면 끝입니다. *Press **Enter for every other question**, wait 1–2 minutes; it is done when the window closes.*
  5. **새** PowerShell 창에서 `py --version`을 입력해 `Python 3.`으로 시작하는 버전이 나오면 됩니다. *In a **new** PowerShell, `py --version` should print a version starting with `Python 3.`*
- AI에게 코드를 실행하게 할 때 Windows에서는 이렇게 덧붙이세요: "윈도우에서는 python 대신 py로 실행해." *On Windows, tell the AI: "run it with py, not python."*

---

## 문제가 생기면 / Troubleshooting

- **"vixcode on Windows requires git-bash"**: Git for Windows(2-3)가 없거나 설치 뒤 재시작하지 않은 경우입니다. 설치하고 컴퓨터를 재시작한 뒤 다시 `vixcode`. *Install Git for Windows (2-3), restart the computer, run `vixcode` again.*
- **VS Code 터미널에서만 "'vixcode' 용어가 … 인식되지 않습니다" / "not recognized"**: Vix Code를 설치하기 전에 켜 둔 VS Code라서 그렇습니다. **VS Code를 완전히 껐다가 다시 켜세요.** *VS Code was open before the install: **quit it completely and reopen**.*
- **"vixcode를 찾을 수 없음 / command not found" (Mac 포함)**: 터미널이나 VS Code를 완전히 껐다가 다시 켜세요. *Fully restart the terminal or VS Code.*
- **"Node.js not found"**: 2-2를 설치한 뒤 **새** 터미널에서 다시 시도하세요. *Install Node.js, then retry in a new terminal.*
- **"python3 not found" (Mac)**: 터미널에서 `xcode-select --install`을 입력해 개발자 도구를 설치한 뒤 다시 시도하세요. *Run `xcode-select --install`, then retry.*
- **Windows 설치 중 빨간 오류 문구가 보임**: 마지막에 로그인 창이 뜨면 정상입니다. 안 뜨면 새 PowerShell에서 `vixcode-login`. *If a login window appears at the end, you're fine; otherwise run `vixcode-login` in a new PowerShell.*
- **Windows에서 `python`을 입력했더니 Microsoft Store가 열림**: `py --version`을 써 보세요. 버전이 나오면 `python` 대신 `py`를 쓰면 됩니다. 안 나오면 시작 메뉴에서 **'앱 실행 별칭 관리'**를 열어 **'Python (default)'**와 **'Python install manager'**를 켠 뒤(켜져 있으면 껐다 켜기) 새 PowerShell에서 다시. *If `python` opens the Microsoft Store, try `py --version`. Otherwise open **"Manage app execution aliases"**, turn on **"Python (default)"** and **"Python install manager"**, and retry in a new PowerShell.*
- **PATH 질문에 그냥 Enter를 눌렀음**: 시작 메뉴에서 Python install manager를 다시 실행하거나 `py install --configure`를 입력하면 질문이 다시 나옵니다. 이번엔 `y`. *Run Python install manager again (or `py install --configure`) and answer `y`.*
- 그래도 안 되면 괜찮습니다. **그냥 오세요.** AI 채팅(C)이나 옆 사람과 함께 참여할 수 있습니다. *Still stuck? **Just come**: use an AI chat (C) or pair up.*

## 알아 두세요 / Notes

- Vix Code를 비롯한 AI 도구는 대화 내용을 외부 서버로 보냅니다. **개인정보나 미공개 연구 자료는 넣지 마세요.** *AI tools send your prompts to external servers. **No personal or unpublished data.***
- Vix Code는 이름이 비슷한 'Vix'(getvix.dev)와 다른 프로그램입니다. *Vix Code is not the same as "Vix" (getvix.dev).*
- 강의실에는 책상이 없고 콘센트가 부족합니다. **노트북을 완전히 충전해 오세요.** 음료는 반입할 수 없습니다. *There are no desks and few outlets: **charge your laptop fully**. No drinks inside.*
