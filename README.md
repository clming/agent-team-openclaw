# Agent Team 项目

**多 Agent 协作开发系统**

[![Projects](https://img.shields.io/badge/projects-2-blue)](./projects/README.md)
[![Agents](https://img.shields.io/badge/agents-4-green)](./agents/)

---

## 🎯 已完成项目

| 项目 | 状态 | GitHub | Agent 分工记录 |
|------|------|--------|---------------|
| **WeChat Login** | ✅ 完成 | [GitHub](https://github.com/clming/wechat-login) | [协作记录](./projects/WECHAT-LOGIN.md) |
| **Agent Team Framework** | ✅ 完成 | [GitHub](https://github.com/clming/agent-team-openclaw) | [自引用](./projects/README.md) |

📋 **查看完整项目列表**: [projects/README.md](./projects/README.md)

---

## 📁 项目结构

```
agent-team/
├── agents/                 # Agent 角色定义
│   ├── product_manager.md  # 产品经理 Agent
│   ├── project_manager.md  # 项目经理 Agent
│   ├── senior_developer.md # 高级开发 Agent
│   └── qa_tester.md        # 测试工程师 Agent
├── docs/                   # 项目文档
│   ├── PRD.md             # 产品需求文档
│   └── WBS.md             # 工作分解结构
├── workflows/              # 工作流程
│   └── dev-cycle.md       # 开发周期流程
├── memory/                 # 记忆和日志
│   └── session-logs.md    # 会话日志
└── AGENTS.md              # Agent 配置说明
```

---

## 🤖 Agent 角色

### 1. 产品经理 (Product Manager)
**职责**:
- 需求分析和文档编写
- 用户故事定义
- 功能优先级排序
- 产品路线图规划

### 2. 项目经理 (Project Manager)
**职责**:
- 项目计划制定 (WBS)
- 进度跟踪和管理
- 资源分配
- 风险管理

### 3. 高级开发 (Senior Developer)
**职责**:
- 系统架构设计
- 核心功能开发
- 代码审查
- 技术难题攻关

### 4. 测试工程师 (QA Tester)
**职责**:
- 测试计划制定
- 测试用例编写
- 执行测试
- Bug 跟踪和验证

---

## 📋 工作流程

### 开发周期 (dev-cycle.md)

1. **需求分析** → 产品经理
2. **任务分解** → 项目经理
3. **开发实现** → 高级开发
4. **测试验证** → 测试工程师
5. **迭代优化** → 全体 Agent

---

## 📄 文档列表

| 文档 | 说明 |
|------|------|
| PRD.md | 产品需求文档 |
| WBS.md | 工作分解结构 |
| dev-cycle.md | 开发周期流程 |
| AGENTS.md | Agent 配置说明 |

---

## 🚀 使用方式

Agent 团队通过协调器 (Coordinator) 进行任务分配和进度跟踪。

每个 Agent 都有明确的职责范围和输出标准，确保协作高效。

---

## 📝 状态

- ✅ Agent 角色定义完成
- ✅ 工作流程设计完成
- ✅ 文档模板创建
- 🔄 持续优化中
