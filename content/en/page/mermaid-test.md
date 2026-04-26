---
title: "Mermaid Gallery"
date: 2026-04-26
description: "Mermaid rendering samples for this Hugo theme."
keywords: ["mermaid", "flowchart", "test"]
disableComments: true
---

# Mermaid gallery

If diagrams render as shapes and arrows, Mermaid is working.  
If you only see raw code, check theme and Mermaid loader settings.

## Sample: Flowchart (TD)

```mermaid
flowchart TD
    A[Page load] --> B{Mermaid supported?}
    B -->|Yes| C[Render diagram]
    B -->|No| D[Show code block]
    C --> E[OK]
    D --> F[Need Mermaid JS]
```

## Checklist

- Boxes and arrows render visually
- Labels are readable
- Light/dark mode contrast is OK

## Sample: Sequence Diagram

```mermaid
sequenceDiagram
    participant U as User
    participant B as Blog
    participant G as Gemini API
    U->>B: topic
    B->>G: draft request
    G-->>B: body + Mermaid
    B-->>U: rendered post
```

## Sample: Mindmap

```mermaid
mindmap
  root((Auto posting))
    collect
      trends
      keywords
    draft
      title
      summary
      body
    visuals
      Mermaid
      tables
      checklists
    QA
      banned words
      facts
      length
```

## Sample: Timeline

```mermaid
timeline
    title Site improvements
    step1 : trust pages
    step2 : footer links
    step3 : comments off on static pages
    step4 : Mermaid enabled
```

## Sample: Pie

```mermaid
pie title Post mix (example)
    "Tech and IT" : 35
    "Finance" : 25
    "Life and Health" : 20
    "Entertainment" : 20
```

## Sample: Flowchart (LR)

```mermaid
flowchart LR
    I[Detect issue] --> K[Keywords]
    K --> D[Draft]
    D --> V{QA pass?}
    V -->|Yes| P[Publish]
    V -->|No| R[Revise]
    R --> V
```

## Sample: State Diagram

```mermaid
stateDiagram-v2
    [*] --> Draft
    Draft --> Review : request review
    Review --> Published : approve
    Review --> Draft : needs work
    Published --> Archived : archive
```

## Sample: Class Diagram

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

## Sample: ER Diagram

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

## Sample: Journey

```mermaid
journey
    title Reader journey
    section Browse
      Home: 5: Reader
      Open post: 4: Reader
    section Read
      Skim: 4: Reader
      Diagram: 5: Reader
    section Act
      Next post: 4: Reader
      Share: 3: Reader
```

## Sample: Gantt

```mermaid
gantt
    title Weekly schedule (example)
    dateFormat  YYYY-MM-DD
    section Collect
    trends           :done,  a1, 2026-04-20, 1d
    keywords         :done,  a2, 2026-04-21, 1d
    section Write
    draft            :active, b1, 2026-04-22, 2d
    QA               :       b2, after b1, 1d
    section Ship
    publish          :       c1, after b2, 1d
```

## Sample: Git Graph

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
