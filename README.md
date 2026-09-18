# JW MD Agents

기획·개발·마케팅·재무·법무·GIS·데이터 등 **281개 도메인 전문가 에이전트** 팩.
설치하면 첫 질문을 보고 알맞은 전문가를 제안하는 **자동 라우팅**도 함께 켜집니다.

## 설치 (Claude Code에서)

```
/plugin marketplace add emforhs2002-bit/JW_md_agents
/plugin install company-agents
```

설치 후 **Claude Code를 새로 시작**하면 적용됩니다.

## 뭐가 되나요?

- 새 대화에서 질문하면 → "지금 질문은 OO 작업 같아요. 'OO 전문가'를 쓸까요?" 하고 제안
- "예" 하면 해당 전문가가 붙어서 처리
- 단순 질문/잡담이면 그냥 바로 답 (안 귀찮게)

## 업데이트

```
/plugin marketplace update jw-md-agents
```

## 구성

```
.claude-plugin/marketplace.json   마켓플레이스 등록
plugins/company-agents/
├── .claude-plugin/plugin.json    플러그인 정의
├── agents/                       전문가 281개
└── hooks/                        자동 라우팅 규칙 주입
```
