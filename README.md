# Agent Team - 多 Agent 协作框架

**Workspace 层面的 Agent 协作系统** - 用于管理所有项目的开发

[![Projects](https://img.shields.io/badge/projects-2-blue)](./projects/README.md)
[![Agents](https://img.shields.io/badge/agents-4-green)](./agents/)

---

## 🎯 定位说明

**Agent Team 不是独立项目**，而是 **Workspace 层面的协作框架**，用于：

1. **管理所有项目**: Edu-AITest, WeChat Login, App Project 等
2. **分配 Agent 任务**: Product Manager, Senior Developer, QA Tester 等
3. **记录协作过程**: 每个项目的 Agent 分工和交付物
4. **标准化流程**: 统一的开发工作流

---

## 🤖 Agent 角色

| Agent | 职责 | 配置文件 |
|-------|------|---------|
| **Product Manager** | 需求分析、产品设计、API 规范 | `agents/product_manager.md` |
| **Project Manager** | 任务分解、进度跟踪、WBS | `agents/project_manager.md` |
| **Senior Developer** | 架构设计、代码实现、Code Review | `agents/senior_developer.md` |
| **QA Tester** | 测试计划、质量验收、Bug 跟踪 | `agents/qa_tester.md` |

---

## 📁 目录结构

```
/root/.openclaw/workspace/
├── agent-team/                    # ← Agent 协作框架 (本目录)
│   ├── agents/                    # Agent 角色定义
│   ├── workflows/                 # 工作流程
│   ├── projects/                  # 项目协作记录
│   │   ├── README.md              # 项目列表
│   │   └── WECHAT-LOGIN.md        # WeChat Login 协作记录
│   └── README.md                  # 本文件
│
├── projects/                      # ← 实际项目代码
│   ├── edu-aitest/                # 教育 AI 测试平台
│   ├── wechat-login/              # 微信登录服务
│   └── app-project/               # 移动前端项目 (规划中)
│
└── skills/                        # ← 技能模块
```

---

## 🔄 工作流程

```
新需求
  │
  ▼
Product Manager (需求分析)
  │
  ▼
PRD 文档 + 用户故事
  │
  ▼
Project Manager (任务分解)
  │
  ▼
WBS 任务清单
  │
  ▼
Senior Developer (代码实现)
  │
  ▼
可运行代码 + 单元测试
  │
  ▼
QA Tester (测试验证)
  │
  ▼
测试报告 → 有 Bug? → 返回开发修复
  │
  无 Bug
  │
  ▼
验收通过 → 提交 GitHub
```

详细流程：[workflows/dev-cycle.md](./workflows/dev-cycle.md)

---

## 📋 管理的项目

| 项目 | 位置 | GitHub | 状态 | Agent 分工记录 |
|------|------|--------|------|---------------|
| **WeChat Login** | `projects/wechat-login/` | [GitHub](https://github.com/clming/wechat-login) | ✅ 完成 | [查看](./projects/WECHAT-LOGIN.md) |
| **Edu-AITest** | `projects/edu-aitest/` | [GitHub](https://github.com/clming/edu-aitest) | ✅ 完成 | 待补充 |
| **App Project** | `projects/app-project/` | 待创建 | 📄 规划中 | - |

📊 **完整项目列表**: [projects/README.md](./projects/README.md)

---

## 📝 如何为新项目分配 Agent

### 步骤 1: 创建项目协作记录

```bash
cd /root/.openclaw/workspace/agent-team/projects
touch NEW-PROJECT.md
```

### 步骤 2: 记录 Agent 分工

参考 `WECHAT-LOGIN.md` 格式:
- 阶段 1: Product Manager - 需求分析
- 阶段 2: Senior Developer - 架构设计
- 阶段 3: Senior Developer - 代码实现
- 阶段 4: QA Tester - 测试计划

### 步骤 3: 在项目中添加引用

在项目 README 中添加:
```markdown
🤖 本项目由 Agent Team 协作完成
[查看协作记录](../agent-team/projects/NEW-PROJECT.md)
```

### 步骤 4: 跟踪进度

更新 `projects/NEW-PROJECT.md` 中的完成状态

---

## 🔗 项目关联

### Agent Team → 项目代码
- `projects/WECHAT-LOGIN.md` → `../projects/wechat-login/`
- 记录每个阶段的 Agent 和交付物

### 项目代码 → Agent Team
- 项目 README 顶部添加 Agent Team 标识
- 链接回协作记录

---

## 📊 统计信息

| 指标 | 数值 |
|------|------|
| 管理项目数 | 2 |
| 已完成项目 | 2 |
| Agent 角色 | 4 个 |
| 总代码量 | ~6700+ 行 |
| 总文档量 | ~315KB |

---

## 📚 相关文档

- [Agent 角色定义](./agents/)
- [工作流程](./workflows/dev-cycle.md)
- [项目列表](./projects/README.md)
- [WeChat Login 协作记录](./projects/WECHAT-LOGIN.md)
- [项目关联说明](../PROJECT-RELATIONSHIP.md)

---

*最后更新：2026-03-24*
