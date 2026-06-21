# 创作者 AI 内容合规自检 Checklist v1

> 发布前过一遍，5 分钟搞定三层标记合规

---

## 发布前自检（3 分钟）

### 平台标记

- [ ] YouTube：已在 Studio 勾选 "Altered or synthetic content"
- [ ] 如果使用 AI 生成逼真人脸/声音，确认标签不会被观众忽略
- [ ] 如果内容涉及真实人物肖像合成，额外检查是否符合 likeness detection 政策

### 元数据检查

- [ ] 导出视频文件，用 MediaInfo 或 C2PA 工具检查是否携带元数据
- [ ] 如果使用了 Veo / Sora / Runway 等工具生成，确认工具是否自动嵌入 C2PA 签名
- [ ] 跨平台分发时（TikTok → YouTube → 小红书），每层平台各自标记，互不通气

### 辖区合规

- [ ] 面向欧盟观众：确认 AI Act Art.50 义务（chatbot 披露 / deepfake 标签 / 机器可读水印）
- [ ] 面向中国观众：确认《标识办法》要求（显式 + 隐式双标识，元数据字段完整）
- [ ] 面向加州观众：确认 SB-942 隐式披露字段（提供商名 / AI 系统名+版本 / 生成时间 / 唯一 ID）

---

## 发布后自检（2 分钟）

- [ ] 在 YouTube 播放器界面确认标签可见
- [ ] 在视频描述区确认 AI 声明文字
- [ ] 在评论区置顶一条说明（"本视频使用 AI 配音/画面，详见描述"）
- [ ] 如果收到 "Altered or synthetic" 误标，知道申诉路径：YouTube Studio → 申诉

---

## 工具清单

| 用途 | 工具 | 链接 |
|------|------|------|
| C2PA 元数据检查 | Content Credentials Explorer | https://contentcredentials.org/verify |
| 视频元数据查看 | MediaInfo | https://mediaarea.net/MediaInfo |
| YouTube AI 标签说明 | YouTube Help Center | https://support.google.com/youtube/answer/14328491 |
| AI Act Art.50 原文 | EU AI Act Service Desk | https://ai-act-service-desk.ec.europa.eu/en/ai-act/article-50 |
| 中国《标识办法》全文 | 国家互联网信息办公室 | https://www.cac.gov.cn/2025-03/14/c_1743654684782215.htm |
| 加州 SB-942 全文 | California Legislative Info | https://leginfo.legislature.ca.gov/faces/billTextClient.xhtml?bill_id=202320240SB942 |

---

## 常见误区

| 误区 | 实际 |
|------|------|
| "AI Act 延期了，不急" | 只延了存量系统水印 4 个月到 12/2；新系统 8/2 零宽限 |
| "YouTube 标了就够了" | YouTube 标签只对齐平台层，制度层标记（EU/中国/加州）是独立义务 |
| "水印技术成熟了" | SynthID / C2PA 截图即失效，技术路线尚未定型 |
| "我不在欧洲，不受 AI Act 管" | Art.50 覆盖向欧盟观众提供服务的提供者，不看你在哪 |
| "删除标签就没事" | 中国《标识办法》明确用户恶意删除标识也违法 |

---

## 关键日期速查

| 日期 | 事件 | 紧急度 |
|------|------|--------|
| **2026-06-02** | YouTube 全量主动检测已启动 | ✅ 已生效 |
| **2026-08-02** | AI Act Art.50/99 全面适用 | ⏰ 41 天 |
| **2026-08-02** | 加州 AB-853 同日生效 | ⏰ 41 天 |
| **2026-12-02** | 存量系统水印补齐截止 | 📅 163 天 |

---

*Creator Checklist v1 · 2026-06-20*
