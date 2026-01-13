# 技术信号采集任务配置

**最后更新**：2026年01月13日（北京时间）

---

## 🎯 任务目标

采集今日技术信号（AI Productivity、Web3 Infrastructure、Open Source、Crypto News），生成简洁邮件发送并备份到 GitHub。

---

## 📋 核心策略

### 1. **数据源权重**

- **Twitter（70-80%）**：主要数据源
  - 官方账号：产品发布、功能更新
  - 极客讨论：技术细节、实践经验
  - 普通用户：真实反馈、创意玩法
  - 热度话题：trending、高互动
  
- **其他来源（20-30%）**：
  - Hacker News：Show HN、技术讨论
  - Reddit：社区反馈、实践分享
  - Indie Hackers：创业者视角
  - GitHub Trending：开源项目

### 2. **搜索策略**

#### Twitter 搜索（6-8 次）
1. `ChatGPT OR GPT-4 OR OpenAI` - OpenAI 动态
2. `Claude OR Anthropic` - Anthropic 动态
3. `Gemini OR Google AI OR Bard` - Google AI 动态
4. `AI tools OR AI productivity OR AI workflow` - AI 工具实践
5. `Ethereum OR Vitalik OR Web3` - Web3 动态
6. `DeFi OR crypto infrastructure` - 加密货币基础设施
7. `GitHub trending OR open source` - 开源项目
8. `developer productivity OR coding tips` - 开发者实践

#### 其他搜索（2-3 次）
1. Hacker News 热门讨论
2. Reddit 技术社区
3. GitHub Trending 页面

### 3. **筛选标准**

#### 必须满足
- ✅ 时效性：24 小时内发布
- ✅ 热度：高转发/点赞/评论
- ✅ 价值：有实践/讨论/数据/洞察

#### 多样性要求
- ✅ 公司多样：OpenAI、Anthropic、Google、Meta、Microsoft 等
- ✅ 领域多样：AI、Web3、开源、开发者工具
- ✅ 人群多样：极客、普通用户、创业者、分析师
- ❌ 避免：单一公司/产品占比超过 30%

#### 优先级
- ⭐⭐⭐⭐⭐ 重大发布：新产品、重大更新
- ⭐⭐⭐⭐ 实践评测：知名开发者的第一手体验
- ⭐⭐⭐⭐ 行业趋势：权威媒体的深度分析
- ⭐⭐⭐ 社区讨论：高质量的技术讨论
- ⭐⭐⭐ 创意项目：有趣的 Show HN 项目

### 4. **深度验证**

只打开 **4-5 个最关键页面**：
- 重大新闻的官方报道
- 知名开发者的深度评测
- 权威媒体的行业分析
- 高质量的技术讨论帖

### 5. **输出格式**

#### 邮件格式：简洁 Markdown
```markdown
# 今日技术信号 - YYYY年MM月DD日（北京时间）

## 🤖 AI Productivity

### 1. [标题]
**来源**：[平台]（发布时间）  
**链接**：[原文链接]

[简短描述，2-3 句话]

---

### 2. [标题]
...
```

#### 不需要
- ❌ 复杂 HTML 样式
- ❌ CSS 动画效果
- ❌ 精美排版
- ❌ 图片嵌入

#### 必须保留
- ✅ 原文链接
- ✅ 来源标注
- ✅ 发布时间
- ✅ 清晰结构
- ✅ 简短描述

---

## 🕐 时区配置

**写死北京时间**：
```bash
TZ='Asia/Shanghai' date '+%Y-%m-%d'
```

所有日期显示、文件命名、邮件标题都使用北京时间。

---

## 📦 GitHub 备份

**仓库**：632591029/tech-signal-knowledge-base  
**目录**：signals/  
**文件命名**：
- Markdown：`YYYY-MM-DD_tech_signals.md`
- HTML（如需要）：`YYYY-MM-DD_tech_signals.html`

---

## 💰 积分优化目标

| 阶段 | 目标消耗 | 优化措施 |
|------|---------|---------|
| 搜索 | 20-25 积分 | 合并相关搜索，6-8 次 Twitter + 2-3 次其他 |
| 筛选 | 3-5 积分 | 基于 snippet 快速筛选 |
| 验证 | 12-15 积分 | 只打开 4-5 个关键页面 |
| 生成 | 5-8 积分 | 简化 Markdown，去掉复杂 HTML |
| **总计** | **40-50 积分** | 相比初始 100+ 积分，节省 50% |

---

## 📊 质量指标

- **信号数量**：12-15 条
- **领域分布**：
  - AI Productivity：40-50%
  - Web3 & Crypto：25-30%
  - Open Source：15-20%
  - 开发者实践：10-15%
- **来源分布**：
  - Twitter：70-80%
  - Hacker News：10-15%
  - 其他：5-10%
- **人群覆盖**：
  - 极客/开发者：50%
  - 普通用户：30%
  - 创业者/分析师：20%

---

## 🚫 避免的问题

1. **单一公司偏向**：不要让某个公司（如 Claude）占比超过 30%
2. **极客偏向**：不要只关注技术细节，也要关注用户体验和商业洞察
3. **过度优化**：不要为了节省积分而牺牲信号质量
4. **时区错误**：必须使用北京时间，不能依赖系统自动检测
5. **仓库错误**：必须推送到 tech-signal-knowledge-base，不是 lifeStart

---

## ✅ 执行检查清单

- [ ] 确认北京时间
- [ ] Twitter 搜索 6-8 次（覆盖各大 AI 公司）
- [ ] 其他来源搜索 2-3 次
- [ ] 筛选出 15-20 条候选信号
- [ ] 检查多样性（公司、领域、人群）
- [ ] 深度验证 4-5 个关键页面
- [ ] 生成简洁 Markdown 邮件
- [ ] 发送邮件到 a632591029@gmail.com
- [ ] 备份到 tech-signal-knowledge-base 仓库
- [ ] 确认积分消耗在 40-50 范围内

---

**配置版本**：v2.0  
**生效日期**：2026年01月13日
