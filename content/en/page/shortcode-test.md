---
title: "Shortcode Test"
date: 2026-04-26
description: "Validation page for Hugo tip/warning/info shortcodes."
keywords: ["hugo", "shortcode", "tip", "warning", "info"]
disableComments: true
---

# Hugo shortcode test

Below are style samples for `tip`, `warning`, and `info` shortcodes.

{{< tip >}}
**Tip:** Place internal links in the top half of the article first for better scanning flow.
{{< /tip >}}

{{< warning >}}
**Warning:** Repeating the same keyword link too often can look spammy. Keep one URL to one insertion.
{{< /warning >}}

{{< info >}}
**Info:** Markmap works well in automated pipelines because heading-based syntax has a low error rate.
{{< /info >}}

## Mixed markdown test

{{< info >}}
- list item
- **bold text**
- [Dev Lab link](/en/page/dev-lab/)
{{< /info >}}
