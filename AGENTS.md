# Agent 团队配置

## 📍 位置
`/root/.openclaw/workspace/projects/agent-team/`

## 🎯 团队角色

| 角色 | Agent 名称 | 职责 |
|------|-----------|------|
| 产品经理 | `product_manager` | 需求分析、PRD 编写、用户故事 |
| 项目经理 | `project_manager` | 任务分配、进度跟踪、WBS 分解 |
| 高级开发 | `senior_developer` | 架构设计、代码实现、Code Review |
| QA 测试 | `qa_tester` | 测试用例、Bug 报告、质量验收 |

## 📁 目录结构

```
agent-team/
├── AGENTS.md              # 本文件
├── agents/                # 各 Agent 配置文件
│   ├── product_manager.md
│   ├── project_manager.md
│   ├── senior_developer.md
│   └── qa_tester.md
├── memory/                # 团队工作记忆
│   └── session-logs.md
└── workflows/             # 工作流定义
    └── dev-cycle.md
```

## 🔄 工作流程

```
需求 → 产品经理 → 项目经理 → 高级开发 → QA 测试 → 验收
              ↓           ↓          ↓         ↓
           PRD 文档    任务分解    代码实现   测试报告
```

## 📌 使用说明

1. **创建子 Agent 会话**：参考各 Agent 配置文件中的指令
2. **协调工作**：由主 Agent（我）担任"协调员"角色
3. **工作记录**：所有会话记录存入 `memory/session-logs.md`

---
*创建时间：2026-03-23*
