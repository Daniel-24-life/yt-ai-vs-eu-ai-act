# China AI Content Labeling Regulation: Source Summary

> Extracted: 2026-06-09
> Purpose: Dual-anchor blog (YT 6/2 × EU 8/2) China fact base

## Key Regulatory Instruments

| Instrument | Type | Published | Effective |
|-----------|------|-----------|-----------|
| 《人工智能生成合成内容标识办法》 | 行政法规（强制性） | 2025-03-14 | 2025-09-01 |
| GB 45438—2025 《网络安全技术 人工智能生成合成内容标识方法》 | 国家标准（强制性） | 2025-03 | 2025-09-01 |

## Dual-Label System (显式 + 隐式)

**显式标识** (Explicit Label):
- Text, voice, or graphic prompt visible to users
- Must clearly indicate content is AI-generated/synthetic

**隐式标识** (Implicit Label):
- Metadata + digital watermark embedded in the file
- Metadata JSON with mandatory fields:

```json
{
  "AIGC": {
    "Label": "1",
    "ContentProducer": "XXX公司",
    "ProduceID": "20250301001"
  }
}
```

## Five Covered Content Types

1. 文本 (Text)
2. 音频 (Audio)
3. 图像 (Image)
4. 视频 (Video)
5. 虚拟场景 (Virtual scenes)

## Four-Party Responsibility Chain

1. **生成合成服务提供者** (Generation service provider) — must add both labels
2. **应用程序分发平台** (App distribution platform) — must verify labels before listing
3. **内容传播服务提供者** (Content distribution platform) — must verify labels; add risk warning if missing
4. **用户** (End users) — prohibited from maliciously removing, altering, or forging labels

## Key Difference from EU Article 50

- EU Art.50: principle-level obligation ("machine-readable + detectable"), implementation left to market and future Code of Practice
- China: **engineering-level specification** — field names, formats, and methods are defined down to the JSON key level
- As of early 2026, only 8 of 27 EU member states had designated national supervisory authorities

## Source Links

1. 国家互联网信息办公室, 《人工智能生成合成内容标识办法》全文 — https://www.cac.gov.cn/2025-03/14/c_1743654684782215.htm
2. 国家标准全文公开系统, *GB 45438-2025* — https://openstd.samr.gov.cn/bzgk/std/newGbInfo?hcno=F32EA2A561F1886CD8D606513512D547
3. TC260, *GB 45438-2025 国标 PDF 全文* — https://www.tc260.org.cn/upload/2025-03-15/1742009439794081593.pdf
4. 中国政府网, *四部门联合发布 AI 标识办法新闻* — https://www.gov.cn/lianbo/bumen/202503/content_7014283.htm

---

*Sources v1 — last updated 2026-06-09*
