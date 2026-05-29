# color-skill

> 🇺🇸 [English README](./README.md)

**팔레트 스크린샷에서 뽑아낸 강한 보색 두 톤 HTML 컬러 시스템 — 검은 무대 위 큰 컬러 블록, 라운드 패널, 고대비 타이포그래피.**

## 사전 요구

- **Claude Cowork 또는 Claude Code** 환경

## 목표

대부분의 생성 HTML은 안전하고 흐릿한 팔레트로 수렴한다. 이 스킬은 반대로 간다 — 강한 보색 대비와 큰 컬러 블록으로 첫인상을 잡는다. 검은 무대 위에 색 패널을 놓고, 각 패널은 배경색과 글자색을 1:1로 강하게 맞물리게 만들어 인스타 팔레트 카드 같은 리듬을 만든다.

## 사용 시점 & 방법

`컬러 스킬`, `color-skill`, `this color pattern`, `컬러 패턴`, `팔레트 HTML` 또는 강한 보색 블록·라운드 패널·고대비 타이포·보색 리듬의 HTML 페이지/사이트/리포트를 요청할 때 발동한다. 팔레트 스크린샷을 주거나 색을 설명하면 페이지를 생성한다.

## 사용 사례

| 상황 | 프롬프트 | 동작 |
|---|---|---|
| 팔레트 → 페이지 | `"이 팔레트로 HTML 만들어줘"` | 검은 무대 + 보색 패널 페이지 생성 |
| 리포트 스타일링 | `"컬러 스킬로 리포트 꾸며줘"` | 콘텐츠에 고대비 블록 리듬 적용 |
| 팔레트 카드 | `"인스타 팔레트 카드 스타일로"` | 인스타 스타일 팔레트 카드 생성 |

## 주요 기능

- **검은 무대 베이스** — 페이지 배경 `#000000`/`#050505`/`#07090b`에서 시작
- **1:1 컬러 페어링** — 각 패널의 배경과 글자를 보색 쌍으로 맞물림
- **큰 라운드 패널** — 고대비 타이포의 볼드 블록
- **팔레트 스크린샷 구동** — 레퍼런스 이미지에서 색 추출·적용

## 설치

```bash
git clone https://github.com/jasonnamii/color-skill.git ~/.claude/skills/color-skill
```

## 업데이트

```bash
cd ~/.claude/skills/color-skill && git pull
```

`~/.claude/skills/`에 배치된 스킬은 Claude Code 및 Cowork 세션에서 자동으로 사용 가능합니다.

## Cowork Skills

25개 이상의 커스텀 스킬 중 하나입니다. 전체 카탈로그: [github.com/jasonnamii/cowork-skills](https://github.com/jasonnamii/cowork-skills)

## 라이선스

MIT License — 자유롭게 사용, 수정, 공유 가능합니다.
