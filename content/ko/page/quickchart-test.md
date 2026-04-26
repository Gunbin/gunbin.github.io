---
title: "QuickChart.io Test"
date: 2026-04-26
description: "QuickChart.io URL 기반 차트 렌더링 테스트 페이지"
keywords: ["quickchart", "chart", "test", "dev lab"]
disableComments: true
---

# QuickChart.io Test

이 페이지는 `QuickChart.io`의 URL 파라미터(`c`) 방식으로 차트 이미지가 정상 렌더링되는지 확인합니다.

## 1) Bar Chart 샘플

![QuickChart Bar Sample](https://quickchart.io/chart?w=760&h=360&c=%7Btype%3A%27bar%27%2Cdata%3A%7Blabels%3A%5B%27Mon%27%2C%27Tue%27%2C%27Wed%27%2C%27Thu%27%2C%27Fri%27%5D%2Cdatasets%3A%5B%7Blabel%3A%27Visitors%27%2Cdata%3A%5B120%2C190%2C170%2C220%2C260%5D%2CbackgroundColor%3A%27rgba(59%2C130%2C246%2C0.7)%27%7D%5D%7D%2Coptions%3A%7Bplugins%3A%7Blegend%3A%7Bdisplay%3Atrue%7D%7D%7D%7D)

## 2) Line Chart 샘플

![QuickChart Line Sample](https://quickchart.io/chart?w=760&h=360&c=%7Btype%3A%27line%27%2Cdata%3A%7Blabels%3A%5B%27Jan%27%2C%27Feb%27%2C%27Mar%27%2C%27Apr%27%2C%27May%27%2C%27Jun%27%5D%2Cdatasets%3A%5B%7Blabel%3A%27Signups%27%2Cdata%3A%5B32%2C45%2C58%2C61%2C72%2C84%5D%2CborderColor%3A%27rgb(16%2C185%2C129)%27%2CbackgroundColor%3A%27rgba(16%2C185%2C129%2C0.18)%27%2Ctension%3A0.35%2Cfill%3Atrue%7D%5D%7D%2Coptions%3A%7Bplugins%3A%7Blegend%3A%7Bdisplay%3Atrue%7D%7D%7D%7D)

## 3) Pie Chart 샘플

![QuickChart Pie Sample](https://quickchart.io/chart?w=760&h=360&c=%7Btype%3A%27pie%27%2Cdata%3A%7Blabels%3A%5B%27SEO%27%2C%27Content%27%2C%27Dev%27%2C%27Ops%27%5D%2Cdatasets%3A%5B%7Bdata%3A%5B35%2C30%2C20%2C15%5D%2CbackgroundColor%3A%5B%27%233b82f6%27%2C%27%2310b981%27%2C%27%23f59e0b%27%2C%27%23ef4444%27%5D%7D%5D%7D%2Coptions%3A%7Bplugins%3A%7Blegend%3A%7Bposition%3A%27bottom%27%7D%7D%7D%7D)

## 원본 URL 예시

```text
https://quickchart.io/chart?w=760&h=360&c={type:'bar',data:{labels:['Mon','Tue'],datasets:[{label:'Visitors',data:[120,190]}]}}
```

