# awesome-agents-cn

中文版的智能体（Agents）集合 - 为各类 AI IDE 和开发工具提供专业的 AI 助手

## 什么是 Agent？

Agent（智能体）本质上是一段精心设计的提示词，定义了 AI 在特定任务中的角色、能力和工作方式。你可以把这些 agent 文件嵌入到支持 agent 系统的 AI IDE 中，比如 Trae、Claude Code、Cursor、Windsurf、Continue 等，让 AI 扮演不同的专业角色，帮你完成各种开发任务。

打个比方，agent 就像是给 AI 配备了不同的"专业工具包"——代码审查员会仔细检查代码质量，性能优化师会专注提升系统效率，数据库专家会帮你处理复杂查询。每个 agent 都在自己的领域里很专业，用起来比让 AI 从头开始更高效。

## 项目简介

本项目汇集多个优秀的 Agent 仓库，并将它们翻译成中文版本，方便中文用户使用：

- **[awesome-claude-agents-cn](awesome-claude-agents-cn/)** - AI 开发团队（24个专业 agents）
- **[awesome-claude-code-subagents-cn](awesome-claude-code-subagents-cn/)** - 代码 Subagents（126+个，10个类别）
- **[buildwithclaude-cn](buildwithclaude-cn/)** - 插件市场（117个agents + 175个commands + 28个hooks + 26个skills）


## 翻译进度

### ✅ 已完成
- **主 README.md** - 完整的中文版
- **awesome-claude-agents-cn** (15个文件):
  - README.md ✅
  - Core agents (4个) ✅
  - Orchestrators (3个) ✅
  - Universal agents (4个) ✅
  - Specialized agents (8个关键agents) ✅
- **awesome-claude-code-subagents-cn** (全部完成):
  - README.md ✅
  - 01-core-development (10个agents) ✅
  - 02-language-specialists (21个agents) ✅
  - 03-infrastructure (15个agents) ✅
  - 04-quality-security (14个agents) ✅
  - 05-data-ai (10个agents) ✅
  - 06-developer-experience (10个agents) ✅
  - 07-specialized-domains (12个agents) ✅
  - 08-business-product (10个agents) ✅
  - 09-meta-orchestration (10个agents) ✅
  - 10-research-analysis (6个agents) ✅
  - **总计：108个agents全部完成！**

### ⏳ 进行中
- **buildwithclaude-cn**:
  - README.md (待开始)
  - agents (117个，待开始)

## 快速开始

### 安装 Agents

将需要的 agent 文件复制到你的 agents 目录：

```bash
# 全局安装（所有项目可用）
cp -r awesome-claude-agents-cn/agents/* ~/.claude/agents/

# 项目安装（仅当前项目可用）
cp -r awesome-claude-agents-cn/agents/* .claude/agents/
```

### 使用 Agents

在支持 agents 的 AI IDE 中，你可以：

```bash
# 查看所有可用的 agents
/agents

# 直接使用某个 agent
claude "使用 @code-reviewer 审查我的代码"

# 让 AI 自动选择合适的 agent
claude "帮我优化这个 Python 函数的性能"
```

## Agent 分类

### 1. awesome-claude-agents-cn - AI 开发团队（24个）

#### 核心团队（4个）
- **code-archaeologist** - 代码考古学家：探索、文档化和分析不熟悉的或遗留代码库
- **code-reviewer** - 代码审查员：严格的安全感知审查，提供严重性标记的报告
- **documentation-specialist** - 文档专家：编写全面的 README、API 规范和技术文档
- **performance-optimizer** - 性能优化师：识别瓶颈并应用优化以构建可扩展系统

#### 编排器（3个）
- **tech-lead-orchestrator** - 技术负责人：分析复杂项目并协调多步骤开发任务
- **project-analyst** - 项目分析师：技术栈检测专家，实现智能 agent 路由
- **team-configurator** - 团队配置师：AI 团队设置专家，检测你的技术栈并配置最优的 agent 映射

#### 专业化 Agents（17个）

**Python 专家（8个）**
- python-expert - Python 生态系统专家
- django-expert - Django 后端开发专家
- django-api-developer - Django REST Framework 和 GraphQL 实现
- django-orm-expert - 查询优化和数据库性能
- fastapi-expert - FastAPI 异步 Web 框架专家
- ml-data-expert - 机器学习数据处理专家
- testing-expert - Python 测试专家
- security-expert - Python 安全专家
- performance-expert - Python 性能专家
- devops-cicd-expert - Python DevOps/CI/CD 专家

**Vue 专家（3个）**
- vue-component-architect - Vue 3 Composition API 和组件模式
- vue-nuxt-expert - Nuxt SSR、SSG 和全栈应用
- vue-state-manager - Pinia 和 Vuex 状态架构

**React 专家（2个）**
- react-component-architect - 现代 React 模式、hooks 和组件设计
- react-nextjs-expert - SSR、SSG、ISR 和全栈 Next.js 应用

**Rails 专家（3个）**
- rails-backend-expert - 遵循约定的全栈 Rails 开发
- rails-api-developer - RESTful API 和 Rails 模式下的 GraphQL
- rails-activerecord-expert - 复杂查询和数据库优化

**Laravel 专家（2个）**
- laravel-backend-expert - MVC、服务和 Eloquent 模式的综合 Laravel 开发
- laravel-eloquent-expert - 高级 ORM 优化、复杂查询和数据库性能

#### 通用专家（4个）
- **backend-developer** - 后端开发专家：跨多种语言和框架的多语言后端开发
- **frontend-developer** - 前端开发专家：任何框架的现代 Web 技术和响应式设计
- **api-architect** - API 架构师：RESTful 设计、GraphQL 和框架无关的 API 架构
- **tailwind-css-expert** - Tailwind CSS 专家：Tailwind CSS 样式、实用优先开发和响应式组件

### 2. awesome-claude-code-subagents-cn - 代码 Subagents（126+个）

#### 01. 核心开发
- api-designer - REST 和 GraphQL API 架构师
- backend-developer - 可扩展 API 的服务端专家
- electron-pro - 桌面应用专家
- frontend-developer - React、Vue 和 Angular 的 UI/UX 专家
- fullstack-developer - 端到端功能开发
- graphql-architect - GraphQL schema 和联邦专家
- microservices-architect - 分布式系统设计器
- mobile-developer - 跨平台移动专家
- ui-designer - 视觉设计和交互专家
- websocket-engineer - 实时通信专家

#### 02. 语言专家
- typescript-pro - TypeScript 专家
- sql-pro - 数据库查询专家
- swift-expert - iOS 和 macOS 专家
- vue-expert - Vue 3 Composition API 专家
- angular-architect - Angular 15+ 企业模式专家
- cpp-pro - C++ 性能专家
- csharp-developer - .NET 生态系统专家
- django-developer - Django 4+ Web 开发专家
- dotnet-core-expert - .NET 8 跨平台专家
- dotnet-framework-4.8-expert - .NET Framework 传统企业专家
- elixir-expert - Elixir 和 OTP 容错系统专家
- flutter-expert - Flutter 3+ 跨平台移动专家
- golang-pro - Go 并发专家
- java-architect - 企业 Java 专家
- javascript-pro - JavaScript 开发专家
- powershell-5.1-expert - Windows PowerShell 5.1 和完整 .NET Framework 自动化专家
- powershell-7-expert - 跨平台 PowerShell 7+ 自动化和现代 .NET 专家
- kotlin-specialist - 现代 JVM 语言专家
- laravel-specialist - Laravel 10+ PHP 框架专家
- nextjs-developer - Next.js 14+ 全栈专家
- php-pro - PHP Web 开发专家
- python-pro - Python 生态系统专家
- rails-expert - Rails 8.1 快速开发专家
- react-specialist - React 18+ 现代模式专家
- rust-engineer - 系统编程专家
- spring-boot-engineer - Spring Boot 3+ 微服务专家

#### 03. 基础设施
- azure-infra-engineer - Azure 基础设施和 Az PowerShell 自动化专家
- cloud-architect - AWS/GCP/Azure 专家
- database-administrator - 数据库管理专家
- deployment-engineer - 部署自动化专家
- devops-engineer - CI/CD 和自动化专家
- devops-incident-responder - DevOps 事件管理
- incident-responder - 系统事件响应专家
- kubernetes-specialist - 容器编排大师
- network-engineer - 网络基础设施专家
- platform-engineer - 平台架构专家
- security-engineer - 基础设施安全专家
- sre-engineer - 站点可靠性工程专家
- terraform-engineer - 基础设施即代码专家
- terragrunt-expert - Terragrunt 编排和 DRY IaC 专家
- windows-infra-admin - Active Directory、DNS、DHCP 和 GPO 自动化专家

#### 04. 质量与安全
- accessibility-tester - A11y 合规专家
- ad-security-reviewer - Active Directory 安全和 GPO 审计专家
- architect-reviewer - 架构审查专家
- chaos-engineer - 系统弹性测试专家
- code-reviewer - 代码质量守护者
- compliance-auditor - 法规合规专家
- debugger - 高级调试专家
- error-detective - 错误分析和解决专家
- penetration-tester - 道德黑客专家
- performance-engineer - 性能优化专家
- powershell-security-hardening - PowerShell 安全加固和合规专家
- qa-expert - 测试自动化专家
- security-auditor - 安全漏洞专家
- test-automator - 测试自动化框架专家

#### 05. 数据与 AI
- ai-engineer - AI 系统设计和部署专家
- data-analyst - 数据洞察和可视化专家
- data-engineer - 数据管道架构师
- data-scientist - 分析和洞察专家
- database-optimizer - 数据库性能专家
- llm-architect - 大语言模型架构师
- machine-learning-engineer - 机器学习系统专家
- ml-engineer - 机器学习专家
- mlops-engineer - MLOps 和模型部署专家
- nlp-engineer - 自然语言处理专家
- postgres-pro - PostgreSQL 数据库专家
- prompt-engineer - Prompt 优化专家

#### 06. 开发体验
- build-engineer - 构建系统专家
- cli-developer - 命令行工具创建者
- dependency-manager - 包和依赖专家
- documentation-engineer - 技术文档专家
- dx-optimizer - 开发体验优化专家
- git-workflow-manager - Git 工作流和分支专家
- legacy-modernizer - 遗留代码现代化专家
- mcp-developer - Model Context Protocol 专家
- powershell-ui-architect - WinForms、WPF、Metro 框架和 TUI 的 PowerShell UI/UX 专家
- powershell-module-architect - PowerShell 模块和配置文件架构专家
- refactoring-specialist - 代码重构专家
- slack-expert - Slack 平台和 @slack/bolt 专家
- tooling-engineer - 开发工具专家

#### 07. 专业化领域
- api-documenter - API 文档专家
- blockchain-developer - Web3 和加密专家
- embedded-systems - 嵌入式和实时系统专家
- fintech-engineer - 金融科技专家
- game-developer - 游戏开发专家
- iot-engineer - IoT 系统开发者
- m365-admin - Microsoft 365、Exchange Online、Teams 和 SharePoint 管理专家
- mobile-app-developer - 移动应用专家
- payment-integration - 支付系统专家
- quant-analyst - 量化分析专家
- risk-manager - 风险评估和管理专家
- seo-specialist - 搜索引擎优化专家

#### 08. 商业与产品
- business-analyst - 需求专家
- content-marketer - 内容营销专家
- customer-success-manager - 客户成功专家
- legal-advisor - 法律和合规专家
- product-manager - 产品策略专家
- project-manager - 项目管理专家
- sales-engineer - 技术销售专家
- scrum-master - 敏捷方法论专家
- technical-writer - 技术文档专家
- ux-researcher - 用户研究专家
- wordpress-master - WordPress 开发和优化专家

#### 09. 元与编排
- agent-installer - 通过 GitHub 浏览和安装此仓库中的 agents
- agent-organizer - 多 agent 协调器
- context-manager - 上下文优化专家
- error-coordinator - 错误处理和恢复专家
- it-ops-orchestrator - IT 运维工作流编排专家
- knowledge-synthesizer - 知识聚合专家
- multi-agent-coordinator - 高级多 agent 编排
- performance-monitor - Agent 性能优化
- pied-piper - 为重复的 SDLC 工作流编排 AI Subagents 团队
- task-distributor - 任务分配专家
- workflow-orchestrator - 复杂工作流自动化

#### 10. 研究与分析
- research-analyst - 综合研究专家
- search-specialist - 高级信息检索专家
- trend-analyst - 新兴趋势和预测专家
- competitive-analyst - 竞争情报专家
- market-researcher - 市场分析和消费者洞察
- data-researcher - 数据发现和分析专家

### 3. buildwithclaude-cn - 插件市场（117+个）

#### Agents 分类
- **开发与架构** - 后端、前端、移动、GraphQL 专家
- **语言专家** - Python、Go、Rust、TypeScript、C/C++ 专家
- **质量与安全** - 代码审查、安全审计、调试
- **基础设施与运维** - DevOps、云、数据库优化
- **数据与 AI** - ML 工程、数据管道、AI 开发
- **加密与区块链** - 交易系统、DeFi、Web3 开发

#### Commands 分类（175个）
- **版本控制** - 提交、PR 创建、分支管理
- **代码分析** - 测试、审查、优化
- **文档** - 文档生成、变更日志、API 规范
- **项目管理** - 待办事项、PRD、任务跟踪

#### Hooks 分类（28个）
- **通知** - Slack、Discord、Telegram 警报
- **Git** - 自动暂存、智能提交
- **开发** - 保存时 lint、自动格式化
- **安全** - 文件保护、漏洞扫描

#### Skills 分类（26个）
- 文档处理（PDF、DOCX、PPTX、XLSX）
- Canvas 设计
- 文件组织
- 图像增强
- MCP 构建器
- Obsidian 集成
- 主题工厂
- Web 应用测试

## 使用示例

### 使用 awesome-claude-agents-cn

```bash
# 使用代码审查员
claude "使用 @code-reviewer 审查我的最新提交"

# 使用性能优化师
claude "使用 @performance-optimizer 优化这个函数"

# 使用团队配置师
claude "使用 @team-configurator 为我的项目配置最优的 AI 团队"
```

### 使用 awesome-claude-code-subagents-cn

```bash
# 使用 Python 专家
claude "使用 @python-pro 优化这个 Python 函数"

# 使用安全审计员
claude "使用 @security-auditor 审查这段认证代码"

# 使用 DevOps 工程师
claude "使用 @devops-engineer 帮助调试这个部署"
```

### 使用 buildwithclaude-cn

```bash
# 使用命令
/commit                    # 创建约定式提交
/create-pr                 # 创建拉取请求
/docs                      # 生成文档
/tdd                       # 开始测试驱动开发
/code_analysis             # 分析代码质量
```

## 安装指南

### 方式一：直接复制

```bash
# 安装 awesome-claude-agents-cn
cp -r awesome-claude-agents-cn/agents/* ~/.claude/agents/

# 安装 awesome-claude-code-subagents-cn
cp -r awesome-claude-code-subagents-cn/categories/* ~/.claude/agents/

# 安装 buildwithclaude-cn agents
cp -r buildwithclaude-cn/plugins/all-agents/agents/* ~/.claude/agents/
```

### 方式二：符号链接（推荐）

```bash
# macOS/Linux
ln -s $(pwd)/awesome-claude-agents-cn/agents ~/.claude/agents/awesome-claude-agents-cn
ln -s $(pwd)/awesome-claude-code-subagents-cn/categories ~/.claude/agents/awesome-claude-code-subagents-cn
ln -s $(pwd)/buildwithclaude-cn/plugins/all-agents/agents ~/.claude/agents/buildwithclaude-cn
```

### 方式三：使用插件市场

```bash
# 添加 buildwithclaude 市场
/plugin marketplace add davepoon/buildwithclaude

# 安装插件
/plugin install agents-python-expert@buildwithclaude
/plugin install commands-version-control-git@buildwithclaude
/plugin install hooks-notifications@buildwithclaude
```

## 项目结构

```
awesome-agents-cn/
├── README.md                          # 本文件
├── awesome-claude-agents-cn/           # AI 开发团队（24个）
│   ├── README.md
│   ├── agents/
│   │   ├── core/                      # 核心团队
│   │   ├── orchestrators/             # 编排器
│   │   ├── specialized/               # 专业化 agents
│   │   └── universal/                 # 通用专家
│   └── docs/
├── awesome-claude-code-subagents-cn/  # 代码 Subagents（126+个）
│   ├── README.md
│   ├── categories/                    # 10个类别
│   └── tools/
└── buildwithclaude-cn/                # 插件市场（117+个）
    ├── README.md
    └── plugins/
```

## 贡献

欢迎贡献！如果你有新的 agent 想要添加或改进现有的翻译，请提交 Pull Request。

## 许可证

本项目中的各个子项目均遵循 MIT License。原始项目：
- [awesome-claude-agents](https://github.com/vijaythecoder/awesome-claude-agents)
- [awesome-claude-code-subagents](https://github.com/VoltAgent/awesome-claude-code-subagents)
- [buildwithclaude](https://github.com/davepoon/buildwithclaude)

## 致谢

感谢原始项目的维护者和贡献者！

---

让 AI 开发变得更强大🚀
