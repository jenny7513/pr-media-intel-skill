# PR 媒体情报研究 Skill（pr-media-intel）

> 一个专为 **PR / 公关 / 市场团队** 设计的 Claude Skill，帮助你快速摸清目标市场的媒体评测生态，制定精准的媒体接触策略。

---

## 🎯 这个 Skill 能做什么

给定一个**产品品类**和**目标国家/地区**，Skill 会自动搜索并整理：

| 输出内容 | 说明 |
|---|---|
| 📋 记者姓名 & Media Outlet | 具体到人名，不是泛泛的"科技媒体" |
| 🔍 评测关注点 | 该市场记者最在意哪些维度（如：CADR、导航技术、安全认证） |
| 🏷️ 品牌 & 机型偏好 | 哪些品牌被频繁推荐，哪些机型获得好评 |
| 📅 最佳接触时机 | 结合产品季节性，给出 pitch 的黄金窗口 |
| ⚠️ 雷区提示 | 哪些媒体不接受公关样机、有合规要求（如德国 GDPR） |
| ✅ PR 行动建议 | 可执行的媒体接触策略，含样机周期、材料清单 |

**支持语言**：中文、英文均可触发，输出语言跟随用户提问语言。

**支持国家/地区**：美国、英国、法国、德国、日本……可同时查询多个市场。

---

## 💬 使用方法

### 安装方式

将本仓库的 `SKILL.md` 文件安装到你的 Claude Code Skill 目录，或通过 Cowork 插件导入。

### 触发方式

只需用自然语言描述你的需求，Skill 会自动识别并启动。以下都是有效的触发语句：

**中文示例：**
```
我要给日本和美国媒体发空气净化器，先帮我了解一下各国媒体生态
```
```
哪些记者评测过扫地机器人？我需要做媒体接触策略
```
```
整理一下德国市场的智能门锁评测记者名单
```

**English examples:**
```
Which journalists in the US and Germany have reviewed robot vacuums this year?
```
```
I need a media landscape report for air purifiers in France and Japan for PR outreach
```
```
Who are the key reviewers covering smart home products in the UK?
```

---

## 📊 输出示例

以**扫地机器人（美国/德国）**为例，Skill 输出结构如下：

### 美国市场

| 记者/作者 | Media Outlet | 报道特点 |
|---|---|---|
| Millie Fender | Tom's Guide | 6年以上扫地机测试经验，Managing Editor，偏好 Shark、Roborock、Dyson |
| Jared Hannah | CNET | 真实场景测试，专注宠物毛发与障碍物识别，高度评价 Dreame |
| Rachel Cericola | Wirecutter / NYT | 25年智能家居资深编辑，购买决策影响力最大 |
| Alistair Charlton | TechRadar | 多媒体自由撰稿人，覆盖 Dyson、Narwal、Roborock、DJI |

**评测关注点：** 障碍物识别准确率、宠物毛发处理、自动集尘站、拖地功能（干湿分离）、App 易用性、噪音水平

**PR 行动建议（节选）：**
- 优先联系 Rachel Cericola（Wirecutter）：NYT 流量背书，购买转化率最高，建议提前 6-8 周接触
- Jared Hannah（CNET）重视实测数据，需准备宠物毛发测试视频素材
- ⚠️ Consumer Reports 不接受公关样机，需确保产品在市场可购买后自然进入评测

### 德国市场

| 记者/作者 | Media Outlet | 报道特点 |
|---|---|---|
| Frederic Hamann | GameStar.de | 德国最活跃的扫地机器人专家，深度覆盖 Dreame、Roborock、Ecovacs |
| Marius Nann | home&smart.de | 智能家居专家，覆盖各细分场景（宠物/多层/静音款） |
| Stefan Schomberg | Heise Bestenlisten | 20年资深测评人，技术受众，结构化 Top 10 排行 |

**评测关注点：** 地图建图精度、德语 App 支持、GDPR 数据隐私合规、噪音（≤60dB）、清洁站自动化程度

**PR 行动建议（节选）：**
- 优先联系 Frederic Hamann（GameStar）：德国该品类最具影响力的测评者，建议寄旗舰款并给足 3-4 周测试期
- ⚠️ 德国媒体对数据隐私极为敏感，产品需提前准备德语隐私政策文档和 GDPR 合规说明

---

## 🌍 已验证支持的品类

以下品类已经过实际测试，效果良好：

- 🤖 扫地机器人（Robot Vacuum）
- 💨 空气净化器（Air Purifier）

理论上支持任意消费电子 / 智能家居 / 户外电器品类。

---

## 📁 文件结构

```
pr-media-intel-skill/
└── SKILL.md        # Skill 核心指令文件
```

---

## 🔧 适用场景

- 准备海外媒体发布前的**媒体名单梳理**
- 制定**分国家 PR 策略**
- 新市场进入前的**媒体生态摸底**
- 给管理层准备的**竞品媒体曝光分析**
- 整理**记者画像**，辅助个性化 pitch

---

## 📝 License

MIT License — 欢迎自由使用和修改。
