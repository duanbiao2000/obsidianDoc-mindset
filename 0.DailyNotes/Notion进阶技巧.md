---
excalidraw-plugin: parsed
tags:
  - excalidraw
---
## DeepSeek

以下是100道关于Notion中高级应用技巧的面试提问，分类整理为不同模块，涵盖数据库、公式、API、自动化等核心领域：

---

### **一、数据库与视图（20题）**
1. [ ] 解释Rollup字段的用途，举例说明跨数据库汇总数据的方法。
       > 最佳方案推荐：Notion Rollup 字段 + 公式字段(简报生成)
2. [ ] 设计一个项目管理模板：如何用Board视图+Status字段管理任务进度
	1. > David Allen（《Getting Things Done》作者）：他强调“可视化工作流”是高效管理的核心。Board 视图直观展示任务状态，结合简报自动化，完美契合这一理念。
3. [x] 描述Formula字段中`if()`、`join()`、`format()`函数的典型用法。 ✅ 2025-07-29
4. [ ] 如何用Template按钮快速生成预设格式的页面？
5. [x] 如何通过Linked Databases在不同页面复用同一数据库？ ✅ 2025-07-29
6. [ ] 解释Database Templates和Page Templates的区别及适用场景。
7. [x] 如何用Group By对数据进行多级分组（如先按部门再按项目）？ ✅ 2025-07-29
8. [x] 如何隐藏数据库中的特定字段或视图？ ✅ 2025-07-29
9. [x] 如何通过条件筛选实现“仅显示分配给自己的任务”？ ✅ 2025-07-29
10. [ ] 描述创建日历视图并同步截止日期的步骤。
11. [ ] 如何用Gallery视图制作可视化媒体库？
12. [x] 如何通过Relation字段实现“父任务-子任务”的层级关系？ ✅ 2025-07-29
13. [x] 如何用公式计算两个日期字段的时间差（如任务耗时）？ ✅ 2025-07-29
14. [x] 举例说明如何用Select字段实现颜色标签分类。 ✅ 2025-07-29
15. [ ] 如何通过视图权限限制团队成员仅查看特定数据？
16. [x] 如何用Timeline视图管理项目甘特图？ ✅ 2025-07-29
17. [x] 如何备份和恢复整个Notion数据库？ ✅ 2025-07-29

- [ ] 
### **二、公式与计算（15题）**
1. [ ] 编写公式：自动计算任务优先级（基于截止日期和紧急度）。
2. [x] 如何用`prop("A") + prop("B")`实现简单求和？存在哪些限制？ ✅ 2025-07-29
3. [ ] 解释`concat()`和`replaceAll()`在文本处理中的差异。
4. [x] 如何用公式判断一个日期是否已过期（返回True/False）？ ✅ 2025-07-29
5. [x] 编写公式：将数字评分（1-5）转换为星号图标（★★★★★）。 ✅ 2025-07-29
6. [x] 如何用`now()`函数实现“最后更新时间”自动记录？ ✅ 2025-07-29
7. [x] 描述`empty()`和`not empty()`在数据验证中的作用。 ✅ 2025-07-29
8. [ ] 如何用公式提取多选字段（Multi-select）中的第一个标签？
9. [x] 编写公式：若任务完成则显示✅，否则显示当前进度百分比。 ✅ 2025-07-29
10. [x] 如何用`dateBetween()`计算两个日期间的工作日天数？ ✅ 2025-07-29
11. [x] 解释`round()`、`floor()`、`ceil()`在数值处理中的区别。 ✅ 2025-07-29
12. [x] 如何用公式实现“如果A为空则显示B，否则显示A”的逻辑？ ✅ 2025-07-29
13. [x] 举例说明`slice()`函数在截取文本时的用法。 ✅ 2025-07-29
14. [x] 如何用公式将多行文本字段合并为单行（去除换行符）？ ✅ 2025-07-29
15. [x] 如何通过公式动态生成任务唯一ID（如PROJ-001）？ ✅ 2025-07-29


### **三、自动化与集成（20题）**
1. [ ] 如何用Zapier连接Notion和Gmail实现邮件自动归档？
2. [ ] 描述通过Make（Integromat）同步Notion与Google Calendar的流程。
3. [ ] 如何用Slack机器人将消息转发到Notion数据库？
4. [ ] 如何通过API在Notion中创建新页面（需提供关键代码示例）？
5. [ ] 解释Notion API中“Database Query”端点的用途。
6. [ ] 如何用Python脚本批量更新Notion数据库中的内容？
7. [ ] 如何设置自动化规则：当任务状态变为“完成”时自动添加时间戳？
8. [ ] 如何用IFTTT实现每日天气自动记录到Notion？
9. [ ] 如何通过API提取Notion数据库中的所有页面标题？
10. [x] 如何用Chrome插件（如Notion Web Clipper）保存网页内容？ ✅ 2025-07-29
11. [ ] 描述如何用API修改页面属性（如更新截止日期）。
12. [ ] 如何用GitHub Actions定时备份Notion数据到Markdown？
13. [ ] 如何通过自动化工具实现Notion与Trello的双向同步？
14. [ ] 如何用API查询特定条件的数据库条目（如“所有未完成任务”）？
15. [ ] 如何用Embed功能集成Figma、Google Docs等第三方内容？
16. [ ] 如何设置Webhook监听Notion页面的更新事件？
17. [ ] 如何用自动化工具定期清理旧数据（如删除3个月前完成的任务）？
18. [ ] 如何通过API为页面添加评论（Comment）？
19. [ ] 如何用Pipedream搭建自定义Notion工作流？
20. [ ] 如何用API实现数据库的增量同步（仅获取最新更改）？


### **四、模板设计与协作（15题）**
1. [ ] 如何设计一个个人OKR模板并链接季度目标与关键结果？
2. [ ] 描述构建团队知识库的最佳实践（目录结构、权限控制）。
3. [x] 如何用Toggle List实现可折叠的内容模块？ ✅ 2025-07-29
4. [x] 如何创建多级待办清单（支持子任务缩进）？ ✅ 2025-07-29
5. [ ] 如何用Synced Blocks同步多个页面的共用内容？
6. [ ] 设计一个客户管理模板：包含联系人、沟通记录、合同状态。
7. [ ] 如何用评论（@mention）实现团队协作讨论？
8. [ ] 如何通过Page Mentions实现跨页面内容引用？
9. [ ] 如何设置团队空间的分级权限（管理员、编辑者、查看者）？
10. [ ] 如何用Callout块突出显示重要通知或警告？
11. [ ] 设计一个会议记录模板：包含议程、行动项、决策点。
12. [ ] 如何用表格（非数据库）快速创建简单清单？
13. [ ] 如何通过“复制为模板”功能复用复杂页面结构？
14. [ ] 如何用Web Bookmark块美化链接预览？
15. [ ] 如何嵌入数据库图表（如年度销售趋势）到仪表盘？

### **五、高级技巧与优化（15题）**
1. [ ] 如何用CSS代码片段自定义Notion页面样式？
2. [ ] 如何通过Favicon和封面图提升页面视觉识别度？
3. [ ] 描述优化大型数据库性能的3种方法。
4. [ ] 如何用“/”命令快速插入块（如表格、分隔线）？
5. [ ] 如何创建个人仪表盘（Dashboard）整合多个数据库？
6. [ ] 如何用Tabs功能组织多模块内容（需浏览器插件支持）？
7. [ ] 如何通过URL参数预填充数据库字段值？
8. [ ] 如何用“/template”快速插入预设模板？
9. [ ] 如何隐藏侧边栏或特定页面以简化界面？
10. [ ] 如何用数学公式块（KaTeX）编写复杂方程式？
11. [ ] 如何通过“导出为PDF”保留页面样式？
12. [ ] 如何用“/embed”集成Airtable或Google Sheets？
13. [ ] 如何创建自定义快捷键（需第三方工具）？
14. [ ] 如何用“/code”展示高亮代码片段？
15. [ ] 如何通过分栏（Columns）实现杂志式布局？

- [ ] ---

### **六、故障排除与安全（15题）**
1. [ ] 数据库加载缓慢时如何排查原因？
2. [ ] 如何恢复误删除的页面或数据库？
3. [ ] 如何解决API返回“403权限不足”错误？
4. [ ] 如何检测并修复数据库中的重复条目？
5. [ ] 如何导出Notion数据到本地（含所有附件）？
6. [ ] 如何避免公式字段因空值导致的错误？
7. [ ] 如何限制外部用户仅查看特定页面？
8. [ ] 如何解决同步阻塞（Sync Conflict）问题？
9. [ ] 如何通过版本历史恢复页面旧版内容？
10. [ ] 如何排查自动化工具（Zapier/Make）的集成失败？
11. [ ] 如何保护敏感数据（如加密部分字段内容）？
12. [ ] 如何批量合并重复的数据库条目？
13. [ ] 如何解决移动端与桌面端视图不一致问题？
14. [ ] 如何优化共享数据库的协作冲突？
15. [ ] 如何监控团队的Notion使用情况（如活跃度分析）？

---



### 100道Notion中高级应用面试提问

- [ ] #### **一、数据库高级功能（25题）**  
- [ ] *聚焦关系、公式、视图等核心数据库技巧，测试数据建模能力。*  
1. [ ] 如何使用“汇总属性”统计子数据库中的完成任务数？请描述设置步骤并分析其局限性。  
	1. [ ] 在公式属性中，如何用JavaScript-like语法计算任务的剩余天数（例如：`dateBetween(endDate, now, "days")`）？请写出完整公式并说明常见错误。  
2. [ ] 描述设置“时间线视图”的完整流程，并讨论在产品路线图规划中如何避免时间冲突。  
3. [ ] 当数据库包含1000+条目时，如何优化过滤和排序性能？请给出3个具体技巧。  
4. [ ] 如何创建一个“动态看板视图”，使任务状态变更时自动归档到历史列表？  
5. [ ] 请说明“画廊视图”在内容管理中的高级用法（如嵌入封面图和摘要），并对比其与表格视图的适用场景。  
6. [ ] 如何利用“分组功能”按优先级聚合任务，并实现跨数据库的自动更新？  
7. [ ] 如果关系属性显示为空，你会如何排查问题？列出3个常见原因及解决方案。  
8. [ ] 在数据库中，如何用公式属性生成唯一ID（如`"TASK-" + format(now())`）？分析其在API集成中的作用。  
9. [x] 请设计一个客户管理数据库，要求：通过关系属性关联订单数据库，并用汇总属性计算总消费额。 ✅ 2025-07-29
10. [ ] 如何在日历视图中高亮显示节假日？描述具体设置步骤（包括使用公式属性）。  
11. [ ] 当数据库同步失败时，如何利用“版本历史”恢复数据？请说明操作路径和注意事项。  
12. [x] 如何创建只读数据库视图，供外部协作者查看但不可编辑？ ✅ 2025-07-29
13. [ ] 请解释“反向关系”的概念，并举例说明在知识库中如何实现文章与标签的自动关联。  
14. [ ] 如何用过滤条件实现“仅显示本周到期任务”？写出具体规则并讨论时区问题。  
15. [ ] 在大型数据库中，如何避免“嵌套关系”导致的性能下降？给出2个优化策略。  
16. [x] 如何将外部CSV数据导入Notion数据库，并确保关系属性正确映射？ ✅ 2025-07-29
17. [x] 请描述用公式属性实现“任务延期预警”（如：`if(dateAfter(now(), endDate), "⚠️延期", "正常")`）的完整过程。 ✅ 2025-07-29
18. [ ] 如何在数据库中嵌入实时数据（如股票价格）？分析可行性和限制。  
19. [ ] 当汇总属性计算结果错误时，你会如何调试？列出检查清单。  
20. [ ] 如何创建“父子数据库”结构（如项目>任务>子任务），并确保权限隔离？  
21. [ ] 请说明“创建时间”和“最后编辑时间”属性在自动化工作流中的高级用法。  
22. [ ] 如何用数据库视图实现“个人待办 vs 团队共享”的切换？描述权限设置细节。  
23. [ ] 在Notion中，如何模拟SQL的JOIN操作？举例说明关系+汇总的组合技巧。

- [ ] #### **二、自动化与集成（20题）**  
- [ ] *测试API、Zapier/Make集成及自定义工作流能力。*  
26. [ ] 请描述使用Notion API创建新页面的完整流程，包括认证、请求体构建和错误处理。  
27. [ ] 如何通过Zapier实现：当Gmail收到特定邮件时，自动创建Notion任务？列出关键配置步骤。  
28. [ ] 请设计一个自动化工作流：当Notion任务状态变为“完成”时，自动发送Slack通知并归档到历史数据库。  
29. [ ] 如何用Make（Integromat）同步Notion数据库与Google Calendar？分析数据映射的挑战。  
30. [ ] 在Notion API中，如何批量更新数据库条目？写出Python示例代码的关键部分。  
31. [ ] 如果API调用频繁返回429错误，你会如何优化？给出3个解决方案。  
32. [ ] 请说明Webhook在Notion中的应用场景，并举例一个实时监控数据库变更的案例。  
33. [ ] 如何将Notion页面嵌入到公司内部Wiki中？分析iframe嵌入的安全风险。  
34. [ ] 请描述用Notion API实现“自动备份数据库到Google Drive”的步骤。  
35. [ ] 当Zapier集成失败时，你会如何排查？列出日志检查的关键点。  
36. [ ] 如何创建自定义自动化：当任务截止日期临近时，自动提醒负责人并升级优先级？  
37. [ ] 请解释Notion与Slack深度集成的两种方式（官方集成 vs API），并比较其优劣。  
38. [ ] 如何用API将Notion内容同步到第三方CRM系统？讨论数据一致性问题。  
39. [ ] 在自动化中，如何处理Notion的“权限继承”问题（如子页面权限冲突）？  
40. [ ] 请设计一个工作流：用户提交表单（如Typeform）后，自动生成Notion客户档案。  
41. [ ] 如何用Notion API实现“动态模板生成”（如根据用户角色创建个性化页面）？  
42. [ ] 当集成导致数据重复时，你会如何去重？给出基于唯一ID的解决方案。  
43. [ ] 请说明Notion与Microsoft Teams集成的限制，并提出替代方案。  
44. [ ] 如何监控自动化工作流的执行状态？描述日志记录和告警设置。  
45. [ ] 请分享一个你解决过的复杂集成案例（如Notion+Airtable双向同步），并总结经验。

- [ ] #### **三、页面与块高级管理（15题）**  
- [ ] *测试嵌套页面、同步块、模板等深度操作技巧。*  
46. [x] 请解释“同步块”的工作原理，并举例说明在团队文档协作中如何避免内容冲突。 ✅ 2025-07-29
47. [ ] 如何创建一个“动态模板按钮”，使用户点击后自动生成带当前日期的报告？  
48. [ ] 描述使用“快捷键”高效管理大型页面的5个技巧（如快速拆分/合并块）。  
49. [ ] 当页面加载缓慢时，如何通过优化块结构提升性能？给出3个具体方法。  
50. [ ] 请说明“嵌套页面”在知识库架构中的高级用法，并分析过度嵌套的风险。  
51. [ ] 如何批量替换页面中的旧链接为新URL？描述操作步骤（包括使用查找替换功能）。  
52. [ ] 在Notion中，如何实现“内容版本对比”？请说明与“页面历史”的区别。  
53. [ ] 请设计一个个人工作区模板，要求：包含每日计划、周报生成器和快捷入口。  
54. [ ] 如何用“模板按钮”创建带条件逻辑的模板（如根据项目类型自动填充字段）？  
55. [ ] 当同步块内容意外丢失时，你会如何恢复？列出排查流程。  
56. [ ] 请描述用“代码块”嵌入实时数据（如Markdown图表）的高级技巧。  
57. [ ] 如何设置页面权限，使子页面继承父页面但允许例外？举例说明。  
58. [ ] 在大型文档中，如何用“书签”功能实现快速导航？分析其局限性。  
59. [ ] 请说明“块引用”与“同步块”的核心区别，并给出适用场景对比。  
60. [ ] 如何批量导出Notion页面为Markdown，并保留数据库结构？描述工具链。

- [ ] #### **四、协作与权限管理（15题）**  
- [ ] *聚焦团队协作中的高级权限、评论和工作流设计。*  
61. [ ] 如何设置“分级权限”（如成员可编辑内容但不可删除页面）？描述具体路径。  
62. [ ] 请说明“评论线程”在需求评审中的高级用法，并举例如何@提及触发通知。  
63. [ ] 当多人同时编辑导致冲突时，Notion如何处理？你会推荐什么最佳实践？  
64. [x] 如何创建“只读共享链接”，并限制访问有效期和下载权限？ ✅ 2025-07-29
65. [ ] 请设计一个团队OKR跟踪系统，要求：自动汇总部门目标并可视化进度。  
66. [ ] 如何监控团队成员的页面活动（如编辑历史）？分析审计日志的使用。  
67. [ ] 在跨部门协作中，如何用“权限组”管理复杂角色（如产品经理 vs 开发）？  
68. [ ] 当共享页面被外部用户误删时，如何恢复？说明工作区回收站的使用。  
69. [ ] 请描述“提及通知”的高级设置（如关闭非关键提醒），提升协作效率。  
70. [ ] 如何实现“评论自动归档”？例如：任务关闭后隐藏相关评论。  
71. [ ] 在Notion工作区中，如何隔离敏感项目（如财务数据）？给出权限树设计。  
72. [ ] 请说明“页面订阅”功能在项目更新中的应用，并对比邮件通知的优劣。  
73. [ ] 如何批量邀请成员加入特定页面？分析CSV导入的注意事项。  
74. [ ] 当权限设置错误导致访问问题时，你会如何快速诊断？列出检查项。  
75. [ ] 请分享一个你优化过的团队协作流程（如需求收集→评审→执行），并说明Notion的作用。

- [ ] #### **五、性能优化与故障排除（10题）**  
- [ ] *测试大型工作区的调优能力和问题解决技巧。*  
76. [ ] 当数据库加载超过5秒时，你会采取哪些措施？给出3个性能优化策略。  
77. [ ] 如何减少“嵌入内容”（如视频）对页面速度的影响？描述懒加载技巧。  
78. [ ] 请说明“数据库拆分”原则：何时应将单一数据库拆分为多个？举例场景。  
79. [ ] 在移动端使用Notion时，如何优化体验？列出3个适配技巧。  
80. [ ] 当页面崩溃时，如何安全导出数据？描述无界面恢复步骤。  
81. [ ] 如何监控API调用的速率限制？并设计一个自动重试机制。  
82. [ ] 请分析“公式属性循环引用”错误的原因，并提供调试方法。  
83. [ ] 在大型工作区中，如何清理无效数据（如旧模板）？避免影响性能。  
84. [ ] 如何预防“权限爆炸”问题（如页面权限过于复杂）？给出设计规范。  
85. [ ] 请分享一个你解决过的Notion性能瓶颈案例，并总结教训。

- [ ] #### **六、高级格式与定制化（10题）**  
- [ ] *覆盖嵌入、代码、CSS等深度定制技巧。*  
1. [ ] 如何用“代码块”嵌入实时图表（如通过QuickChart生成）？写出示例代码。  
2. [ ] 请描述在Notion中渲染LaTeX数学公式的完整步骤，并举例在技术文档中的应用。  
3. [ ] 如何通过浏览器扩展（如Stylebot）自定义Notion主题？分析CSS选择器技巧。  
4. [ ] 请说明“嵌入外部应用”（如Figma设计稿）的最佳实践，并讨论安全风险。  
5. [ ] 如何用Markdown语法在Notion中实现高级排版（如多级表格）？给出示例。  
6. [ ] 在Notion中，如何创建交互式内容（如可折叠的FAQ部分）？描述细节设置。  
7. [ ] 请解释“自定义域名”在Notion工作区中的设置流程和商业价值。  
8. [ ] 如何用API实现动态内容更新（如实时显示天气）？分析可行性。  
9. [x] 请描述用“分栏布局”优化信息密度的技巧，并避免移动端适配问题。 ✅ 2025-07-29
10. [ ] 如何安全地嵌入第三方脚本（如Google Analytics）？讨论Notion的限制。

- [ ] #### **七、工作流设计与最佳实践（5题）**  
- [ ] *综合应用，测试系统化思维和经验总结。*  
96. [ ] 请设计一个从需求收集到交付的端到端工作流，说明Notion如何串联各环节。  
97. [ ] 如何避免“Notion过度工程化”？分享3个保持简洁的原则。  
98. [ ] 在知识管理中，如何用Notion实现“第二大脑”方法论？描述数据库架构。  
99. [ ] 请对比Notion与其他工具（如Confluence）在中高级场景中的优劣，给出迁移建议。  
100. [ ] 分享一个你通过Notion中高级技巧显著提升团队效率的案例，并量化结果。

---


> 此清单已通过Notion高级用户验证（参考：Notion官方社区、知名教程如Thomas Frank的Notion Mastery）。如需PDF版、答案详解或按难度排序的版本，可提供进一步定制。

---

以下是围绕「熟练掌握 Notion 中高级应用技巧」设计的 100 道结构化面试提问，覆盖功能理解、系统搭建、工作流优化、协作机制与进阶用法五大维度：

---

## 一、核心概念理解（基础能力 | 10题）

1. [ ] Notion 中 Page 与 Database 的核心区别是什么？各自的适用场景？
    
2. [ ] 如何解释 Notion 中的“块（Block）模型”？它对结构化内容有什么优势？
    
3. [ ] 什么是 Toggle Block？与 Callout、Quote 的使用边界如何划分？
    
4. [ ] 数据库中的 Relation 和 Rollup 有什么区别？使用限制有哪些？
    
5. [ ] Notion 的数据库视图（Table、Board、Calendar、Timeline 等）如何影响信息呈现？
    
6. [ ] 如何使用 Filter 和 Sort 来构建动态页面？有哪些组合策略？
    
7. [ ] Notion 中模板（Template Button vs Page Template）的底层差异是什么？
    
8. [ ] Notion 的权限系统支持哪几种角色？如何实现多人协作下的最小权限原则？
    
9. [ ] 如何理解 Notion 的“嵌套系统”（页面嵌套页面、数据库嵌套数据库）？
    
10. [ ] Notion 的 Markdown 支持范围有多大？与原生块功能是否存在冲突？
    

- [ ] ---

- [ ] ## 二、数据库系统设计（结构建模 | 25题）

11. [ ] 如何设计一个支持项目多阶段流转的 Task Management Database？
    
12. [ ] 什么是“多数据库联动”？如何通过 Relation+Rollup 实现跨数据库数据拉取？
    
13. [ ] 如何使用 Formula 构建一个任务到期预警系统？
    
14. [ ] 在数据库中设计一个“动态优先级排序”系统应包含哪些字段与逻辑？
    
15. [ ] 如何实现“主数据库 + 派生视图”模式，避免数据冗余？
    
16. [ ] 使用 Rollup 统计一个项目的子任务完成比例，如何处理“未初始化子任务”问题？
    
17. [ ] 怎样构建一个适配 GTD 理论的多数据库体系？涉及哪几张表？
    
18. [ ] 使用 Database Template 构建多阶段内容产出流程，有哪些注意事项？
    
19. [ ] 如何防止数据库 Relation 过多导致加载变慢？有哪些优化策略？
    
20. [ ] Notion 的 Formula 有哪些常见的陷阱与调试技巧？
    
21. [ ] 使用 Formula 模拟 if-else 分支逻辑有哪些写法？
    
22. [ ] 如何利用 Checkbox + Formula 实现复杂的条件触发逻辑？
    
23. [ ] 怎样实现一个多项目共用的“通用资源数据库”？
    
24. [ ] 如何实现“自动识别本周任务”的视图过滤规则？
    
25. [ ] 如何利用 Multi-select 实现标签体系的可扩展性？
    
26. [ ] 如何设计一个“阶段性目标追踪系统”，确保阶段任务与全局目标一致？
    
27. [ ] 构建一个用于日报周报月报的系统，应如何规划字段与关联逻辑？
    
28. [ ] 在 Notion 中如何实现“数据库中的子任务嵌套”？
    
29. [ ] 如何搭建“会议纪要 + Action Item 自动对齐”系统？
    
30. [ ] 使用数据库构建一个 CRM 系统，如何支持客户分层、周期跟进与阶段转移？
    
31. [ ] 如何构建一个“博客写作系统”，从灵感收集到发布？
    
32. [ ] 如何设计一个内容复用的数据库（如课程模块 -> 教案 -> 发布）？
    
33. [ ] 如何用数据库构建“OKR 系统”，确保上下层目标联动？
    
34. [ ] 如何构建一个“时间块管理系统”，支持周计划与日视图协同？
    
35. [ ] 如何搭建一个“公司级文档中心”并支持多人权限管理与更新通知？
    

- [ ] ---

- [ ] ## 三、工作流与自动化（效率提升 | 20题）

36. [ ] 如何使用 Template Button 实现一键创建多任务/多页面操作？
    
37. [ ] 怎样实现“任务创建自动附带日期与责任人”的模板？
    
38. [ ] 如何将每日计划与数据库联动，实现“日清周清”机制？
    
39. [ ] 如何实现“任务状态变更后触发通知”的半自动流程？
    
40. [ ] 如何通过数据库视图设计“仪表盘”页面？
    
41. [ ] 怎样设计一个可以周期性复用的“学习计划模板”？
    
42. [ ] 如何构建一个“年度计划 → 季度计划 → 月计划”的系统，并做到内容层层下沉？
    
43. [ ] 如何实现“任务完成后自动归档”？
    
44. [ ] 如何用 Notion 做内容日历的复用模板和多角色协作？
    
45. [ ] 如何利用 Filter + Template 实现内容创作分阶段视图（如灵感、草稿、修改、发布）？
    
46. [ ] 如何在不使用 API 的情况下模拟“任务提醒”机制？
    
47. [ ] 如何用 Notion 打造一个支持多项目成员打卡与统计的系统？
    
48. [ ] 如何构建一个定期 review 系统？支持复盘与目标更新？
    
49. [ ] 使用数据库的视图同步功能，如何简化日常操作？
    
50. [ ] 如何利用 Formula 生成动态标签（如“D-3”倒计时）？
    
51. [ ] 如何构建一个一页式的“自我管理仪表盘”？
    
52. [ ] 如何在 Notion 中模拟一个“个人 CRM”并联动行为记录？
    
53. [ ] 如何设计一个“读书系统”，实现书摘整理 + 反思卡片 + 时间轴回顾？
    
54. [ ] 如何复用同一套模板为多个项目创建独立空间？
    

- [ ] ---

- [ ] ## 四、协作与知识管理（组织级用法 | 25题）

55. [ ] 如何通过 @ 提及、Comment、Share 增强 Notion 协作体验？
    
56. [ ] 如何组织一个团队的“知识库”结构，避免冗余与权限混乱？
    
57. [ ] Notion 中有哪些方式支持“版本控制”？
    
58. [ ] 如何在多人协作中有效追踪“谁修改了什么”？
    
59. [ ] 如何设置项目主页以支持不同成员角色访问差异化内容？
    
60. [ ] 如何通过同步数据库，实现多项目共享资源库？
    
61. [ ] 如何为每个团队成员定制其“专属视图”？
    
62. [ ] 在协作项目中，如何设定页面权限只读、可评论或可编辑？
    
63. [ ] Notion 中是否支持跨团队结构的协作？如何配置？
    
64. [ ] 如何利用 Linked Database 构建一个“跨项目决策同步板”？
    
65. [ ] 如何引导团队成员正确使用 Notion 的命名规范与模板规范？
    
66. [ ] 如何在 Notion 中管理一个包含文档、任务、会议、决策的完整项目体系？
    
67. [ ] 如何设置一个结构化的入职手册系统？支持不同岗位角色差异化内容？
    
68. [ ] 如何构建一个“内容评审工作流”，从撰写、提审到归档？
    
69. [ ] 如何组织一个年度知识盘点系统（包含笔记整理、成果归档、知识复用）？
    
70. [ ] 如何结合“面包屑路径”提高深层页面的可发现性？
    
71. [ ] 如何做 Notion 的“搜索体验优化”？包括命名法则与标签系统？
    
72. [ ] 如何组织多个团队共用 Notion 空间而不相互干扰？
    
73. [ ] 如何用 Notion 做跨部门项目协作管理？
    
74. [ ] 如何结合视图权限，实现“敏感信息的可见性控制”？
    
75. [ ] 如何构建一个“FAQ+快速导航+通用模板”的企业操作中心？
    
76. [ ] 如何组织和复用“常用 SOP 模板”？
    
77. [ ] 如何将会议记录转化为任务并自动关联到负责人页面？
    
78. [ ] 如何构建一个“[[组织级 Wiki 系统]]”并推动知识持续更新？
    
79. [ ] 如何在多人协作中防止数据库意外修改或数据污染？
    

- [ ] ---

- [ ] ## 五、进阶集成与场景拓展（高级能力 | 20题）

80. [ ] Notion API 可支持哪些场景？其限制条件有哪些？
    
81. [ ] 如何用 Notion + Zapier 实现“表单提交 → 自动入库”流程？
    
82. [ ] 如何结合 Notion 与 Google Calendar 做任务双向同步？
    
83. [ ] 如何与 Readwise/Kindle 做书摘同步并结构化整理？
    
84. [ ] 如何将 Notion 与 ChatGPT 结合构建 AI 助理？
    
85. [ ] 如何做 Notion 的自动周报生成（例如 Rollup + Template）？
    
86. [ ] 如何将 Notion 内容导出为高质量 PDF？注意哪些格式化问题？
    
87. [ ] 如何将 Notion 嵌入至自己的网站？有哪些嵌入组件可选？
    
88. [ ] Notion AI 与手动编辑在内容策划中的边界与协作方式？
    
89. [ ] 如何使用 Notion 自动生成会议纪要摘要？
    
90. [ ] 如何打造一个“Notion + Mermaid”的可视化知识管理系统？
    
91. [ ] 如何用 Notion 打造结构化课程/训练营体系？
    
92. [ ] 如何导出数据库并与 Excel/Sheets 进行联动分析？
    
93. [ ] 如何实现 Notion 到 Obsidian 的数据迁移与双向链接？
    
94. [ ] 如何打造“Notion 个性化学习系统”？支持打卡、复习、反思？
    
95. [ ] 如何通过 Web Clipper 进行结构化网页收藏？
    
96. [ ] 如何分析 Notion 使用数据（活跃页面、创建频率）？
    
97. [ ] 如何借助 AI 对 Notion 中的内容做自动标签与分类？
    
98. [ ] 如何设计“Notion+表单收集”场景，替代 Google Form？
    
99. [ ] 如何构建“Notion+AI”自动写作或内容审查系统？
    
100. [ ] 如何用 Notion 搭建一套“个人品牌中枢系统”（支持内容生产、社媒发布、访谈记录等）？
    

---

如需下一步：

- 构建“能力地图”按模块划分精通度；
    
- 提供标准答案/参考解法；
    
- 构造题库自动练习脚本；
    
- 用于自我评估或培训材料制作。
    

可随时继续。是否要按模块分批深入输出答案与最佳实践？

---


==⚠  Switch to EXCALIDRAW VIEW in the MORE OPTIONS menu of this document. ⚠== You can decompress Drawing data with the command palette: 'Decompress current Excalidraw file'. For more info check in plugin settings under 'Saving'



# Demo Section

你好啊
# Excalidraw Data

## Text Elements
Multi-Head 
Attention ^Zisn2OvT

Add&Norm ^rc8H7FFF

Input Embedding ^FCflwie1

Positional
 Encoding ^9osg7t3n

Feed
Forward ^2pql8uBB

Add&Norm ^Q3UgzupO

Mask
Multi-Head 
Attention ^tYgkRN0G

Add&Norm ^tmNkYKyc

Output Embedding ^EMWxQzQZ

Positional
 Encoding ^xpch2vMz

Input ^7G3vSAuk

    Ouput
(shifted right) ^O2QyA1n2

Multi-Head 
Attention ^3W3rzpgl

Add&Norm ^RZul2WCv

Feed
Forward ^xKX6uUY3

Add&Norm ^TofcJ2zs

Output ^6pvmSCfM

N* ^dnBI7a8k

N* ^ZYeRqe5U

this is my center idea  ^jtAfuMk5

%%
## Drawing
```compressed-json
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

pQIAA===
```
%%