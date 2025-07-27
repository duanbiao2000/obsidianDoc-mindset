---
date: 2025-07-28 01:17
tags:
  - notion
  - Status/doing
---

好的，收到指令。我们将彻底废弃[[个人CEO周会]]这种基于单篇笔记的、孤立的、不可分析的模式。取而代之的是，我们将利用Notion的数据库和关联特性，构建一个**自动化的、可量化的、能与你的任务和项目系统深度集成的“个人绩效与状态审查系统”**。

这个系统的核心思想是：**每周回顾不应是一次从零开始的“回忆录”，而是一次基于过去一周结构化数据的“数据分析会”。**

---

### **Notion每周回顾系统：架构与工作流**

这个系统将由**一个核心的`Weekly Review`数据库**和**一系列关联到其他核心数据库（如任务、项目、习惯）的`Rollup`属性**构成。

#### **第一步：确保你的核心系统已数据库化**

在构建回顾系统前，你必须已经拥有以下几个核心数据库（如果还没有，请先建立）：

1. **`Tasks`数据库：** 管理所有任务，每个任务有`Status`（如`Done`）和`Project`关联。
2. **`Projects`数据库：** 管理所有项目，每个项目有`Status`（如`Completed`）。
3. **`Habit Tracker`数据库：** 每天记录完成的习惯。
4. **`Sources`数据库：** 记录阅读的书籍、文章等灵感来源。

---

#### **第二步：构建`Weekly Review`数据库 (The Core Engine)**

- **创建方法：** 新建一个页面，选择`Table`数据库，命名为`Weekly Review`。
- **核心属性 (Properties):**

| 属性名称 (Property Name)   | 属性类型 (Type) | 配置与说明 (Configuration & Rationale)                                                              |
| :--------------------- | :---------- | :--------------------------------------------------------------------------------------------- |
| `Week` (Title)         | Title       | **主键**。格式统一，如`W32: 2024-08-05 ~ 2024-08-11`。                                                   |
| `Date Range`           | Date        | **时间戳**。设置本周的起止日期，这是所有自动化`Rollup`的基础。                                                          |
| `Theme`                | Text        | **本周主题**。用一句话总结本周的核心感受或焦点。                                                                     |
| `✅ Tasks Completed`    | Rollup      | **自动化数据拉取**。关联到`Tasks`数据库，筛选`Done Date`在本周`Date Range`内的任务，计算`Count`。                          |
| `🚀 Projects Advanced` | Rollup      | **自动化数据拉取**。关联到`Projects`数据库，筛选`Last Edited`在本周`Date Range`内的项目，显示`Name`。                      |
| `💪 Habit Score`       | Rollup      | **自动化数据拉取**。关联到`Habit Tracker`数据库，筛选`Date`在本周`Date Range`内的记录，计算`Daily Score`的`Average`或`Sum`。 |
| `📚 Knowledge Input`   | Rollup      | **自动化数据拉取**。关联到`Sources`数据库，筛选`Created Time`在本周`Date Range`内的记录，显示`Source Name`。               |
| `🏆 Highlight`         | Text        | **高光时刻**。手动记录本周最开心或最有成就感的事。                                                                    |
| `🧗 Challenge`         | Text        | **挑战与困难**。手动记录本周遇到的主要障碍。                                                                       |
| `💡 Lesson Learned`    | Text        | **经验教训**。手动记录从挑战中学到的东西。                                                                        |
| `⭐ Weekly Rating`      | Select      | **自我评级**。选项：`★★★★★`, `★★★★☆`, `★★★☆☆`, `★★☆☆☆`, `★☆☆☆☆`。                                       |
| `➡️ Next Week's Focus` | Text        | **下周焦点**。明确下周最重要的1-3个目标。                                                                       |

---

#### **第三步：设计回顾工作流与模板 (The Workflow & Template)**

**1. 创建`Weekly Review`数据库模板**

- 在`Weekly Review`数据库中，创建一个名为“**New Weekly Review**”的模板。
- **模板核心：** 在模板的页面内容（Page Content）部分，使用`Linked Database`视图，创建几个预设好的“**本周数据仪表盘**”。

**模板页面内容示例：**

```markdown
---
### 回顾仪表盘 (Review Dashboard)
---

#### ✅ 本周完成的任务
*创建一个到`Tasks`数据库的链接视图，筛选条件为：*
- `Status` is `Done`
- `Done Date` is within `This Week` (或与当前页面的`Date Range`关联)

#### 🚧 本周遇到的挑战
*创建一个到`Tasks`数据库的链接视图，筛选条件为：*
- `Status` is `Blocked` or `Overdue`
- `Last Edited` is within `This Week`

#### 💡 本周的灵感输入
*创建一个到`Sources`数据库的链接视图，筛选条件为：*
- `Created Time` is within `This Week`

---
### 深度反思 (Deep Reflection)
---

**1. 基于数据，我本周的整体表现如何？**
> (观察上面的仪表盘和Rollup数据，写下你的分析)

**2. `Highlight`和`Challenge`背后的根本原因是什么？**
> 

**3. 我从`Lesson Learned`中提炼出的、下周可以立即应用的行动是什么？**
> 

**4. 下周的`Focus`如何确保我更接近我的长期目标？**
> 
```

**2. 每周回顾工作流 (The Weekly Ritual)**

- **时间：** 在你的日历上设置一个雷打不动的、每周一次的30分钟日程，例如周日晚上。
- **步骤：**

```
 1.  **启动（1分钟）：** 在`Weekly Review`数据库中，点击“New Weekly Review”模板，创建一个新的周报条目。填写`Week`标题和`Date Range`。
 2.  **数据审查（10分钟）：** **不要凭空回忆！** 而是直接审查模板中自动生成的“回顾仪表盘”和顶部的`Rollup`数据。这是**基于事实**的回顾。
 3.  **手动填写（10分钟）：** 根据数据审查的结果，填写`Highlight`, `Challenge`, `Lesson Learned`等手动字段。
 4.  **深度反思（5分钟）：** 回答模板页面中的4个深度反思问题。
 5.  **规划未来（4分钟）：** 填写`Next Week's Focus`，并创建下周的关键任务到你的`Tasks`数据库中。
```

---

### **结论：从“日记”到“个人CEO周会”**

将[[个人CEO周会]]迁移到Notion数据库，其核心转变在于：

- **从“记忆驱动”到“数据驱动”：** 你不再依赖模糊的记忆，而是基于系统自动为你聚合的、不可辩驳的数据进行分析。
- **从“孤立反思”到“系统联动”：** 你的回顾不再是一篇孤立的文档，而是与你的任务、项目、习惯、知识库完全打通的**中央控制室**。
- **从“耗时记录”到“高效决策”：** 80%的数据是自动化的，你只需将20%的精力投入到最高价值的“分析”和“决策”环节。

**停止写一篇“每周心情日记”。开始为你自己——你人生的CEO——主持一场高效、数据驱动的“每周绩效评估与战略规划会”。这才是Notion作为个人操作系统，在每周回顾这个场景下的正确打开方式。**
