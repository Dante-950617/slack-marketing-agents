# 퍼포먼스 마케팅 멀티 에이전트 (Claude Code in Slack용)

마켓핏랩 솔루션즈 — 슬랙에서 동작하는 리서치·소재/카피 에이전트.

## 구성

- `.claude/skills/pm-research/` — 리서치 에이전트 (팩트시트 게이트 → 교차 검증 리서치 → 표준 브리프)
- `.claude/skills/pm-creative-copy/` — 소재·카피 에이전트 (앵글 설계 → 매체별 카피·비주얼 디렉션 → A/B 설계)
- 각 스킬의 `references/decongel-project.md` — 데콘젤 프로젝트 검증 팩트시트

## 연동 (Max/Pro 플랜, Claude Code in Slack)

1. 이 저장소를 GitHub에 push
2. Slack App Marketplace에서 Claude 앱 설치 → Claude 계정 연결
3. Claude Code 설정에서 GitHub 연결 + 이 저장소 인증
4. 슬랙에서 `@Claude` 멘션 시 이 저장소를 지정해 작업 → `.claude/skills/`의 스킬이 자동 로드
5. 테스트: `@Claude 데콘젤 여름 시즌 리서치해줘`

## 사용

- 리서치: `@Claude ○○ 시장/경쟁사 리서치해줘`
- 소재: (스레드에서) `이 브리프로 메타 소재 4개 기획해줘`

프로젝트 지식 추가: 새 브랜드의 검증된 팩트가 쌓이면 `skills/*/references/`에 `{브랜드}-project.md`로 추가하고 SKILL.md 상단에 한 줄로 연결.
