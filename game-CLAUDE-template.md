# {게임 이름}

## 개요
{한 줄: 무슨 게임/활동인지}

## AI-Labs 허브 연동 (필수)
이 게임을 처음 배포하거나 아래 카드 정보(제목·설명·URL·태그)가 바뀌면:
→ `ai-labs` 레포의 `games.json`에 반영한다. (Claude가 push 시 먼저 상기)

### 허브 카드 정보 (games.json 원본)
- id:     {kebab-case 고유 id}
- column: {inquiry | novel | future}   (탐구·증명 / 비주얼노벨 / 다음형식)
- tag:    {예: 중2 · 4단원 사각형}
- title:  {이모지 + 제목}
- desc:   {한 줄 설명}
- url:    {배포 URL}
- cta:    {예: 게임 시작 →}

## 배포
GitHub Pages — {배포 URL}
