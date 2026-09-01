# Java 全栈工程师 Obsidian 知识库

> 配套：二本软件工程大三学生，2027 年秋招 Java 全栈/AI 应用岗

## 快速上手

### 1. 导入 Obsidian
1. 下载本文件夹所有内容
2. 在 Obsidian 中「打开本地仓库」，选择本文件夹
3. 设置 → 文件与链接 → 关闭「使用 Wiki 链接」（推荐用标准 Markdown 链接）

### 2. 安装插件（必须）
设置 → 第三方插件 → 关闭安全模式 → 浏览社区插件：
- **Templater**：高级模板（比自带模板好用）
  - 设置模板文件夹为 `99-Templates/`
  - 建议绑定快捷键：设置 → 快捷键 → 搜索「Templater: Open Insert Template Modal」→ 设为 `Alt+T`
- **Dataview**（可选但推荐）：自动查询汇总

### 3. 开始使用

#### 写概念卡片
1. 在对应文件夹（如 `03-Java-Core/04-JVM/`）新建笔记
2. 按 `Alt+T` → 选择 `T-Concept`
3. 填写内容，保存

#### 写算法题解
1. 在 `02-Algorithm/01-Array/` 新建笔记
2. 命名格式：`Array-0001-TwoSum.md`
3. 按 `Alt+T` → 选择 `T-Algorithm`
4. 填写内容，保存

#### 每日复盘
1. 在 `01-Daily/` 新建笔记
2. 命名格式：`2026-08-31.md`
3. 按 `Alt+T` → 选择 `T-Daily`

### 4. 核心习惯
- **写卡片时加 `[[链接]]`**：提到任何已有/待学的概念，都用双方括号链接
- **随手打 `#标签`**：如 `#java` `#interview` `#status/seed`
- **每周日看 Graph View**：按 `Ctrl/Cmd+G`，给孤岛笔记补链接
- **每周日看 Tags Pane**：右侧边栏「标签」，检查是否有重复标签

## 文件夹说明

| 文件夹 | 用途 |
|--------|------|
| `00-Inbox/` | 临时速记，还没整理 |
| `01-Daily/` | 每日学习日志 |
| `02-Algorithm/` | 算法题解，按题型分类 |
| `03-Java-Core/` | Java 核心：基础、集合、并发、JVM |
| `04-Framework/` | Spring 全家桶 |
| `05-Database/` | MySQL、Redis、ES |
| `06-Microservices/` | 微服务、分布式、消息队列、DevOps |
| `07-Frontend/` | Vue3、小程序、前端基础 |
| `08-SystemDesign/` | 系统设计、架构、场景题 |
| `09-Projects/` | 项目复盘（苍穹外卖、Campus AI） |
| `10-Interview/` | 八股文、面经、简历 |
| `11-Books/` | 读书笔记 |
| `99-Templates/` | 6 个模板文件 |
| `99-Assets/` | 图片、PDF 附件 |
| `99-MOCs/` | 知识地图（总览入口） |

## 命名规范

| 类型 | 格式 | 示例 |
|------|------|------|
| 概念卡片 | `技术域 - 概念名.md` | `JVM - 运行时数据区域.md` |
| 算法题解 | `题型-题号-题目英文名.md` | `Array-0001-TwoSum.md` |
| 项目文档 | `项目名 - 模块名.md` | `sky-takeout - Redis缓存设计.md` |
| 八股文 | `面试专题 - 具体问题.md` | `面试专题 - HashMap线程安全问题.md` |
| 每日复盘 | `YYYY-MM-DD.md` | `2026-08-31.md` |
| MOC | `📋 主题 MOC.md` | `📋 Java 并发 MOC.md` |

## 标签体系

### 状态标签
- `#status/seed` — 刚记录，还没整理
- `#status/sprout` — 已整理，但不完整
- `#status/tree` — 完整成熟，可输出
- `#status/evergreen` — 经典内容，定期复习

### 类型标签
- `#type/concept` `#type/algorithm` `#type/project` `#type/interview` `#type/book` `#type/moc` `#type/daily`

### 领域标签
- `#java` `#jvm` `#concurrency` `#spring` `#springboot` `#mysql` `#redis` `#vue` `#linux` `#docker`

## 每日工作流（参考）

```
上午：学知识点 → Inbox 速记 或 直接写概念卡片
下午：健身
傍晚：LeetCode 1 题 → 写题解卡片 → push 到 GitHub
晚上：整理 Inbox → 用模板转成正式卡片 → 加 [[链接]] 和 #标签
睡前：写 Daily 复盘 → 检查 GitHub 绿色方块
周末：更新 MOC → Graph View 补链接 → Tags Pane 检查标签
```

## 重要提醒

1. **先完成再完美**：卡片写得烂没关系，先存在
2. **不要调主题**：默认主题足够用，别浪费时间在 CSS 上
3. **每天必须有产出**：至少 1 张卡片或 1 道题解
4. **GitHub 必须绿**：每天至少 1 次 commit

---

> 计划再完美，不执行等于零。今天就开始。
