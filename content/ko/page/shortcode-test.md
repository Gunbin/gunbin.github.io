---
title: "Shortcode Test"
date: 2026-04-26
description: "Hugo tip/warning/info 숏코드 렌더링 테스트 페이지"
keywords: ["hugo", "shortcode", "tip", "warning", "info"]
disableComments: true
---

# Hugo Shortcode 테스트

아래는 `tip`, `warning`, `info` 숏코드 스타일 샘플입니다.

{{< tip >}}
**핵심 팁:** 내부 링크는 글 상단 50% 구간에서 먼저 배치하면, 사용자 스캔 동선이 더 자연스럽습니다.
{{< /tip >}}

{{< warning >}}
**주의:** 과도한 동일 키워드 반복 링크는 스팸 신호로 보일 수 있으므로 URL당 1회 제한을 권장합니다.
{{< /warning >}}

{{< info >}}
**보충 정보:** Markmap은 헤딩 기반이어서 LLM 출력 오류율이 낮아 자동화 포스팅과 궁합이 좋습니다.
{{< /info >}}

## 마크다운 혼합 테스트

{{< tip >}}
- 리스트
- **굵은 글씨**
- [링크 예시](/ko/page/dev-lab/)
{{< /tip >}}
