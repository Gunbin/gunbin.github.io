---
title: "Markmap Test"
date: 2026-04-26
description: "Markmap 렌더링과 가독성을 점검하는 테스트 페이지"
keywords: ["markmap", "mindmap", "test"]
disableComments: true
---

# Markmap 테스트

아래 블록은 마크다운 헤딩 구조만으로 마인드맵을 렌더링합니다.  
렌더링이 되지 않으면 코드 그대로 보입니다.

```markmap
# TrendRadar 개선계획 v1.0
## P0 우선 진행
### 1-1 내부 링크 상단 집중
- 상단 50% 구간만 링크 삽입
- 부분 매칭 허용
- 동일 URL 1회 제한
### 1-2 이미지 레이어 확장
- Mermaid 유동 삽입
- Markmap 유동 삽입
- Hugo 숏코드 동시 적용
## P1 빠른 착수
### 3-1 Freshness 수동 버튼
- 오래된 글 1건 선택
- 네이버 뉴스 최신 제목 추출
- Lite 모델 1문장 요약 append
## 보류
### 2-2 주제 실로
### 3-2 Drip-Feeding 자동 스케줄러
### 3-3 텔레그램 아웃리치 봇
```

## 확인 포인트

- 노드 간 계층 구조가 트리 형태로 렌더링되는지
- 긴 한글 문구가 줄바꿈 없이 과도하게 깨지지 않는지
- 라이트/다크 모드 전환 시 가독성이 유지되는지
