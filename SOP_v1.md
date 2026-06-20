# SOP v1: AI 合规内容项目流程 · 2026-06-15

> 从 0 到 1 完成 AI 视频标注合规指南的全流程复盘，供后续项目复用

---

## Phase 1: 研究 & 素材收集（Day 1-2）

### 1.1 政策原文抓取
- [ ] EU AI Act: EUR-Lex 全文 + Art.50/99 专项
- [ ] 中国《标识办法》+ GB 45438-2025 全文
- [ ] 加州 SB-942 / AB-2655 / AB-853 全文
- [ ] YouTube 官方 Blog + Help Center

### 1.2 媒体报道 & 技术分析
- [ ] TechCrunch / PPC Land / xix.ai 等一手报道
- [ ] Tech Fast Forward / MIT Tech Review 技术分析
- [ ] 行业标准文档（C2PA / SynthID）

### 1.3 时间线梳理
- [ ] 列出所有关键日期，标注"事实锚"vs"制度锚"
- [ ] 识别核心洞察（60 天窗口期）
- [ ] 输出 `timeline.md` + `timeline.mmd`（Mermaid 格式）

**产出**：`sources/` 目录（4 个政策摘要）+ `timeline.md` + `references.md`

---

## Phase 2: 核心内容撰写（Day 3-5）

### 2.1 主稿撰写
- [ ] 确定标题（SEO 优化：GitHub + 微信公众号）
- [ ] 确定结构：三层标签 → 水印技术 → 延期假消息 → 60 天时间线 → 一次抢跑 → 三个判断
- [ ] 撰写 `README.md`（GitHub 版，完整参考文献）
- [ ] 撰写 `draft_v1.md`（微信公众号版，精简参考文献 + 二维码）

### 2.2 数据可视化
- [ ] 双锚时间轴（`timeline-dual-anchor.png`）
- [ ] 四源对照表（`four-source-comparison.png`）
- [ ] 封面图（`cover-wechat.png`，900×383）
- [ ] GitHub 二维码（`github-repo-qr.png`）

**关键决策**：
- 主锚选择：YouTube 6/2（媒体广泛报道日）vs 3/10（官方 blog）vs 5/30（PPC Land）→ 选 6/2
- 图引用方式：GitHub raw URL（公众号粘贴后自动渲染）

**产出**：`README.md` + `draft_v1.md` + `images/`（4 张图）

---

## Phase 3: SEO & 分发准备（Day 6）

### 3.1 GitHub Pages 配置
- [ ] `_config.yml`（Jekyll SEO：title / description / og:image）
- [ ] 启用 GitHub Pages（main branch / root）
- [ ] 验证 URL：`https://daniel-24-life.github.io/yt-ai-vs-eu-ai-act/`

### 3.2 社交分发素材
- [ ] `social-copy.md`（Twitter 短版 + 朋友圈版 + 群转发版）
- [ ] `twitter-thread_v1.md`（10 条推文 thread）
- [ ] `zhihu-article_v1.md`（知乎/即刻长文版）
- [ ] `xiaohongshu-v1.md`（小红书图文版，2 条笔记）
- [ ] `分发工具包_v1_20260615.md`（全渠道 checklist + 评论区种子 + 媒体邀请模板）

### 3.3 参考文献扩展
- [ ] 从 17 条扩展到 25 条（新增技术源：NVIDIA SynthID / C2PA / Cisco / MIT Tech Review）
- [ ] 同步更新 `references.md` + `draft_v1.md` + `zhihu-article_v1.md`

**产出**：全渠道分发素材就位

---

## Phase 4: 发布 & 分发（Day 7）

### 4.1 公众号发布
- [ ] 公众号后台 → 新建图文 → 切 markdown 编辑器
- [ ] 标题字段：`YT 把欧盟的 deadline 抢跑了 60 天`
- [ ] 封面图上传：`cover-wechat.png`
- [ ] 正文：复制 `draft_v1.md` 全文 → 粘贴
- [ ] 粘贴后检查 3 个图位（line 5/74/99）
- [ ] 预览 → 发送（或定时）

### 4.2 发完 30 分钟内同步分发
- [ ] 朋友圈：贴短版 + 封面图
- [ ] 微信群（技术/合规群）：贴短版
- [ ] Twitter：贴 10 条 thread
- [ ] 知乎/即刻：贴长文版
- [ ] 小红书：贴图文版（2 条笔记）
- [ ] 评论区种子：自己在各平台底下抛钩子

### 4.3 分发后追踪
- [ ] 24 小时内回复所有评论
- [ ] 48 小时后看数据，决定是否追加内容
- [ ] 收集反馈，为 v2 版本积累素材

---

## Phase 5: 复盘 & 迭代（T+7d / T+30d）

### 5.1 T+7d 数据回流
- [ ] 填写 `data-tracking_v1.md`（各平台阅读量 / 互动量 / 转化率）
- [ ] 收集评论区高频问题，整理成 FAQ
- [ ] 识别 v2 版本需要补充的内容

### 5.2 T+30d v2 版本
- [ ] 根据 8/2 后首批执法案例更新主稿
- [ ] 根据评论区 FAQ 追加内容
- [ ] 更新参考文献（新增 5-10 条）
- [ ] 重新生成可视化图表（v2）

---

## 关键经验

### 内容策略
- **核心洞察先行**：60 天窗口期是整篇文章的钩子，不是结论
- **三层标签结构**：显式/隐式/制度性，层层递进，读者容易理解
- **后记点睛**："我没点它，它自己出现了"——把抽象合规拉到个人体验

### 技术决策
- **GitHub Pages 托管**：零成本、可版本控制、URL 稳定
- **图引用 GitHub raw URL**：公众号粘贴后自动渲染，换图零成本（同名覆盖）
- **Markdown 双版本**：`README.md`（GitHub 完整版）+ `draft_v1.md`（公众号精简版）

### 分发策略
- **平台特性裁剪**：Twitter 280 字 / 知乎长文 / 小红书 9:16 图文
- **评论区种子**：发布后 30 分钟内自己抛钩子，引导讨论
- **媒体邀请模板**：主动出击，扩大传播面

---

## 可复用资产

- `sources/`：4 个政策摘要模板
- `timeline.md` + `timeline.mmd`：时间线模板
- `policy-comparison.csv`：四源对照表模板
- `_config.yml`：GitHub Pages SEO 模板
- `分发工具包_v1_20260615.md`：全渠道分发 checklist

---

*SOP v1 · 2026-06-15*
