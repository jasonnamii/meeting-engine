# meeting-engine

> 🇺🇸 [English README](./README.md)

**회의 설계·퍼실리테이션·후처리 엔진. 행동과학과 퍼실리테이션 연구에 기반한 아젠다 설계→진행 가이드→회의록→액션아이템 추출 전주기 프로토콜.**

## 사전 요구

- **Claude Cowork 또는 Claude Code** 환경

## 목표

대부분의 회의는 사람이 아니라 구조가 잘못되어 실패한다. 이 스킬은 Kaner의 Diamond of Participation, Kahneman의 Decision Hygiene 등 연구 기반 프로토콜로 회의를 설계한다 — 의사결정 프레임 선택, 집단 병리 방어, 상황별 퍼실리테이션 패턴 매칭까지.

## 사용 시점 & 방법

회의, 아젠다, 퍼실리테이션, 회의록 언급 시 자동 발동. 3모드: **설계**(회의 전), **정리**(회의 후 노트 구조화), **시스템**(반복 회의 비효율 진단). "내일 이사회 아젠다 짜줘", "회의록 정리해줘", "주간회의가 비효율적이야" 등으로 호출.

## 사용 사례

| 상황 | 프롬프트 | 동작 |
|---|---|---|
| 이사회 준비 | `"내일 이사회 아젠다 짜줘"` | 집단 병리 스크리닝 → 의사결정 프레임 선택(RAPID/동의/자문) → 시간배분 아젠다 + 진행 스크립트 |
| 회의 노트 정리 | `"회의 노트 정리해줘"` | 결정사항, 액션아이템(Who+What+When), 파킹랏, 논의 요약으로 구조화 |
| 반복 회의 진단 | `"주간회의가 비효율적이야"` | 7대 비효율 패턴 매칭 → 행동과학 근본 원인 → 구조적 처방 |

## 주요 기능

- **집단 병리 스크리닝** — 설계 전 필수. Groupthink, Abilene Paradox, Production Blocking, Social Loafing, Anchoring, Status Effect, Noise 7가지 위험 점검
- **의사결정 프레임 선택** — RAPID, Sociocracy 동의, Advice Process, Amazon 묵독, Toyota 네마와시, Bridgewater 투명성 중 최적 프레임 라우팅
- **퍼실리테이션 패턴 매칭** — Kaner Diamond, Liberating Structures 33종, ToP ORID 중 상황별 최적 구조 매칭
- **허브+스포크 아키텍처** — 경량 SKILL.md 허브 + 4개 전문지식 reference 파일 온디맨드 로딩

## 연동 스킬

- **[ceo-pipeline](https://github.com/jasonnamii/ceo-pipeline)** — 로드맵 마일스톤 → 진척리뷰 아젠다 자동 생성
- **[metric-tracker](https://github.com/jasonnamii/metric-tracker)** — 대시보드 지표 → 리뷰 회의 연동
- **[risk-radar](https://github.com/jasonnamii/risk-radar)** — 리스크 리뷰 회의 아젠다 자동 생성
- **[management-skill](https://github.com/jasonnamii/management-skill)** — 실행시스템 회의 프로토콜

## 설치

```bash
git clone https://github.com/jasonnamii/meeting-engine.git ~/.claude/skills/meeting-engine
```

## 업데이트

```bash
cd ~/.claude/skills/meeting-engine && git pull
```

`~/.claude/skills/`에 배치된 스킬은 Claude Code 및 Cowork 세션에서 자동으로 사용 가능합니다.

## Cowork Skills

25개 이상의 커스텀 스킬 중 하나입니다. 전체 카탈로그: [github.com/jasonnamii/cowork-skills](https://github.com/jasonnamii/cowork-skills)

## 라이선스

MIT License — 자유롭게 사용, 수정, 공유 가능합니다.
