# ai-labs — 게임·활동 통합 허브

## 개요
서울사대부중 2학년 수학 게임·탐구활동의 단일 카탈로그.
선생님용 통합 입구. 학생은 카드 링크로 각 게임의 독립 배포 페이지로 이동한다.
배포: https://getbetterwithu.github.io/ai-labs/

## 구조 원칙 (절대 준수)
- 카드 ↔ 게임 = **링크만**. 임베딩·iframe·submodule 금지.
- 게임 본체는 각자 **독립 레포**. 이 허브에 게임 파일을 넣지 않는다.
- 카드는 `games.json`에서 **자동 생성**. `index.html`에 카드를 직접 쓰지 않는다.
- 새 게임 추가 = `games.json`에 항목 1개. 그게 전부.

## 게임 추가/갱신 프로토콜
사용자가 "게임N을 허브에 반영해줘" 하면:
1. 해당 게임 레포를 최신화(pull/clone) 후 그 CLAUDE.md의 "허브 카드 정보" 블록을 읽는다.
2. `games.json`의 `games` 배열에 항목 1개 추가/수정 (column: inquiry|novel|future).
3. 커밋·push (getbetterwithu 계정).

## 파일
- `index.html` — games.json을 fetch해 카드 자동 생성 (디자인 고정, 카드 하드코딩 금지)
- `games.json` — 컬럼 정의 + 전체 게임 카드 목록 (단일 진실 원천)
- `game-CLAUDE-template.md` — 새 게임 레포에 넣을 표준 CLAUDE.md 템플릿
