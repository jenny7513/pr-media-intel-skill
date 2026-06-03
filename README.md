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
帮我整理2026年以来美国、法国、德国媒体记者对割草机器人的评测报告
```
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

以**割草机器人（美国/法国/德国）**为例，Skill 输出结构如下：

### 美国市场

| 记者/作者 | Media Outlet | 报道特点 |
|---|---|---|
| Ed Oswald | PCWorld / TechHive | 深度实测派，专注割草机器人多年，是PCWorld该品类核心撰稿人 |
| Derek Adams | TechRadar | 跟踪前沿新品，偏向体验类横评 |
| 编辑团队 | Tom's Guide | 强调真实使用场景，关注大面积草坪测试 |

**评测关注点：** 无线导航（无需埋线）、AWD全驱性能、边缘切割精度、静音水平、1000美元以内性价比

**PR 行动建议（节选）：**
- 优先联系 Ed Oswald（PCWorld）：该品类核心 KOL，建议附导航技术白皮书
- Tom's Guide 需提供 4-6 周长测试周期，提前备好大草坪测试样机
- ⚠️ Consumer Reports 不接受公关样机，需确保产品在市场可购买后自然进入评测

---

## 🌍 已验证支持的品类

以下品类已经过实际测试，效果良好：

- 🌿 割草机器人（Robot Lawn Mower）
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
