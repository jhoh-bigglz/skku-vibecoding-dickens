# Vibe Coding in the Humanities: Dickens, *Sketches by Boz*

SKKU English 4034 · Introduction to Digital Humanities · Week 7 guest lecture (16 Oct 2026)
성균관대 「디지털인문학입문」 7주차 특강 자료

## 바로 열기 / Open
| | 무엇 / What | 링크 / Link |
|---|---|---|
| 앱 / App | **Boz Explorer**: 56편 그래프, 브라우저 안 순열검정, 단어 검색, 거리 시계 / dot plot, in-browser permutation test, word search, street clock | https://jhoh-bigglz.github.io/skku-vibecoding-dickens/explorer/ |
| 3D | 1830년대 코벤트가든, 「거리 — 아침」의 시간대별 장면(사람·말·수레를 자세히 만든 v2, **Close-up** 버튼으로 가까이) / Covent Garden in the 1830s, hour by hour (v2 with detailed figures; try **Close-up**) | https://jhoh-bigglz.github.io/skku-vibecoding-dickens/3d/ · 이전 판 / v1: https://jhoh-bigglz.github.io/skku-vibecoding-dickens/3d/v1.html |
| Lab | 선택 Lab(Colab 노트북, 제출 없음) / Optional lab (Colab notebook, nothing to submit) | [Open in Colab](https://colab.research.google.com/github/jhoh-bigglz/skku-vibecoding-dickens/blob/main/lab/dickens_lab.ipynb) |
| 실습 / Hands-on | 수업 실습 프롬프트 / Prompts for the in-class hands-on | [PROMPTS.md](PROMPTS.md) |

## 실습 파일 내려받기 / Download the lab files
[**dh-lab.zip**](https://github.com/jhoh-bigglz/skku-vibecoding-dickens/raw/main/dh-lab.zip)을 받아 바탕화면에 풀면 `dh-lab` 폴더 안에 `PROMPTS.md`가 보입니다. VS Code에서 그 폴더를 열고(File → Open Folder) 터미널(Terminal → New Terminal)에서 `vixcode`를 실행하세요.
Download **dh-lab.zip**, unzip it to your Desktop, open the `dh-lab` folder in VS Code (File → Open Folder) and run `vixcode` in the terminal (Terminal → New Terminal). You should see `PROMPTS.md` inside.

Windows에서 '압축 풀기(Extract All)'를 하면 `dh-lab` 안에 `dh-lab`이 한 번 더 생길 수 있습니다. 그때는 `PROMPTS.md`가 바로 보이는 안쪽 폴더를 여세요.
On Windows, "Extract All" may create `dh-lab\dh-lab`; open the inner folder, the one with `PROMPTS.md` directly inside.

## 들어 있는 것 / Contents
- `PROMPTS.md` 수업 실습 프롬프트(한/영) / in-class prompts (KO/EN)
- `data/` 「거리 — 아침」·「거리 — 밤」 정리본(한 줄 = 한 문단), 원래 56편 표(`sketches.csv`) / cleaned texts, one paragraph per line; the original 56 sketches as a table
  - 저장소의 `data/pg882.txt`는 Gutenberg 원문 파일을 고치지 않은 사본으로, Lab 노트북이 Gutenberg에 접속하지 못할 때 대신 받습니다(zip에는 없음). / `data/pg882.txt` in the repository is the unmodified Gutenberg file, a backup for the Lab notebook (not in the zip).
- `lab/` Colab 노트북과 안내 카드: 불용어+화이트리스트, 장소·거리 목록, collocation, 토픽 / Colab notebook and card
- `explorer/` · `3d/` 웹 앱과 3D 모델(파일 하나씩, 이 저장소에만 있고 zip에는 없음) / the web app and 3D model, one file each (in this repository only, not in the zip)

## 알아 둘 것 / Notes
- 텍스트: Project Gutenberg #882(1903 Chapman & Hall판)를 수업용으로 정리한 사본. 저작권이 끝난 공개 텍스트입니다. / Text: cleaned copy of Project Gutenberg #882; public domain.
- 숫자는 수업용 시안 분석입니다. 단어 목록과 정의는 분석자의 선택이며, 3D 모델의 높이·색·인물 배치는 추정입니다(`3d/sources.md`). / Numbers come from a prototype analysis for teaching; word lists are the analyst's choices; the 3D model marks its assumptions.
- AI에 개인정보나 다른 사람의 글을 붙여 넣지 마세요. / Don't paste personal data or other people's writing into an AI.
