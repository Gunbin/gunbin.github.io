---
title: "Mermaid Flowchart Test"
date: 2026-04-26
description: "현재 Hugo 템플릿에서 Mermaid 플로우차트 렌더링을 테스트하는 페이지"
keywords: ["mermaid", "flowchart", "test"]
disableComments: true
---

# Mermaid 플로우차트 테스트

아래 다이어그램이 노드/화살표 형태로 렌더링되면 Mermaid가 정상 지원되는 상태입니다.  
코드 블록 그대로 텍스트로 보이면 테마 또는 렌더링 스크립트 설정이 필요한 상태입니다.

## 샘플: Flowchart (기본 TD)

```mermaid
flowchart TD
    A[사용자 페이지 진입] --> B{Mermaid 지원 여부}
    B -->|지원됨| C[다이어그램 렌더링]
    B -->|미지원| D[코드 블록 텍스트 출력]
    C --> E[테마 확인 완료]
    D --> F[Mermaid JS 로드 설정 필요]
```

## 확인 체크리스트

- 도형 박스와 화살표가 시각적으로 보이는지
- 다이어그램 내부 한글 텍스트가 깨지지 않는지
- 다크 모드에서 선/텍스트 가독성이 유지되는지

## 추가 샘플: Sequence Diagram

요청과 응답 흐름을 표현할 때 유용한 형태입니다.

```mermaid
sequenceDiagram
    participant U as User
    participant B as Blog
    participant G as Gemini API
    U->>B: 주제 입력
    B->>G: 초안 생성 요청
    G-->>B: 본문 + Mermaid 반환
    B-->>U: 렌더링된 포스트 제공
```

## 추가 샘플: Mindmap

핵심 주제와 하위 키워드 구조를 한 번에 보여줄 때 좋습니다.

```mermaid
mindmap
  root((자동화 포스팅))
    주제수집
      트렌드
      키워드
    본문생성
      제목
      요약
      본문
    시각요소
      Mermaid
      표
      체크리스트
    품질검수
      금칙어
      사실성
      문장길이
```

## 추가 샘플: Timeline

이슈 발생 순서나 정책 변화 흐름을 정리할 때 적합합니다.

```mermaid
timeline
    title 자동화 블로그 개선 타임라인
    1단계 : 신뢰 페이지 구축
    2단계 : 푸터 링크 추가
    3단계 : 댓글 비노출 적용
    4단계 : Mermaid 렌더링 활성화
```

## 추가 샘플: Pie

카테고리 비중이나 트래픽 비율 같은 간단 분포를 보여줄 때 사용합니다.

```mermaid
pie title 카테고리별 포스팅 비중(예시)
    "Tech and IT" : 35
    "Finance" : 25
    "Life and Health" : 20
    "Entertainment" : 20
```

## 추가 샘플: Flowchart (LR)

좌우 흐름형 프로세스를 확인하는 샘플입니다.

```mermaid
flowchart LR
    I[이슈 감지] --> K[키워드 정리]
    K --> D[초안 작성]
    D --> V{검수 통과?}
    V -->|예| P[게시]
    V -->|아니오| R[수정 후 재검수]
    R --> V
```

## 추가 샘플: State Diagram

상태 전이(초안 -> 검토 -> 발행 등)를 표현할 때 좋습니다.

```mermaid
stateDiagram-v2
    [*] --> Draft
    Draft --> Review : 검수 요청
    Review --> Published : 승인
    Review --> Draft : 수정 필요
    Published --> Archived : 보관
```

## 추가 샘플: Class Diagram

객체/모듈 구조 관계를 도식화할 때 사용합니다.

```mermaid
classDiagram
    class PostGenerator {
      +fetchTrends()
      +generateDraft()
      +validateOutput()
    }
    class Publisher {
      +publish()
      +updateSitemap()
    }
    PostGenerator --> Publisher : sends content
```

## 추가 샘플: ER Diagram

데이터 구조(엔터티 관계)를 설명할 때 유용합니다.

```mermaid
erDiagram
    AUTHOR ||--o{ POST : writes
    POST ||--o{ TAG_MAP : has
    TAG ||--o{ TAG_MAP : mapped
    POST {
      int id
      string title
      string slug
      datetime published_at
    }
    TAG {
      int id
      string name
    }
```

## 추가 샘플: Journey

사용자 경험 단계별 만족도를 보여줄 때 사용합니다.

```mermaid
journey
    title 방문자 경험 흐름
    section 탐색
      홈 진입: 5: 사용자
      관심 글 클릭: 4: 사용자
    section 읽기
      본문 스캔: 4: 사용자
      다이어그램 이해: 5: 사용자
    section 행동
      다른 글 이동: 4: 사용자
      북마크/공유: 3: 사용자
```

## 추가 샘플: Gantt

콘텐츠 제작 일정을 시각화할 때 적합합니다.

```mermaid
gantt
    title 자동 포스팅 주간 일정
    dateFormat  YYYY-MM-DD
    section 수집
    이슈 수집           :done,  a1, 2026-04-20, 1d
    키워드 정리         :done,  a2, 2026-04-21, 1d
    section 작성
    초안 생성           :active, b1, 2026-04-22, 2d
    품질 점검           :       b2, after b1, 1d
    section 발행
    게시 및 배포         :       c1, after b2, 1d
```

## 추가 샘플: Git Graph

브랜치/배포 흐름을 설명할 때 사용합니다.

```mermaid
gitGraph
    commit id: "init"
    branch feature-mermaid
    checkout feature-mermaid
    commit id: "add samples"
    commit id: "fix style"
    checkout main
    merge feature-mermaid
    commit id: "deploy"
```

