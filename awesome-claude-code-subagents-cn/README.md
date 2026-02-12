<a href="https://github.com/VoltAgent/voltagent">
<img width="1500" height="500" alt="Group 32" src="https://github.com/user-attachments/assets/55b97c47-8506-4be0-b18f-f5384d063cbb" />
</a>

<br />
<br/>

<div align="center">
    <strong>Claude Code subagents 的精选集合。</strong>
    <br />
    <br />
</div>

<div align="center">
    
[![Awesome](https://awesome.re/badge.svg)](https://awesome.re)
<a href="https://github.com/VoltAgent/voltagent">
  <img alt="VoltAgent" src="https://cdn.voltagent.dev/website/logo/logo-2-svg.svg" height="20" />
</a> 

![Subagent Count](https://img.shields.io/badge/subagents-126+-blue?style=flat-square)
[![Last Update](https://img.shields.io/github/last-commit/VoltAgent/awesome-claude-code-subagents?label=Last%20update&style=flat-square)](https://github.com/VoltAgent/awesome-claude-code-subagents)
[![Discord](https://img.shields.io/discord/1361559153780195478.svg?label=&logo=discord&logoColor=ffffff&color=7389D8&labelColor=6A7EC2)](https://s.voltagent.dev/discord)
[![GitHub forks](https://img.shields.io/github/forks/VoltAgent/awesome-claude-code-subagents?style=social)](https://github.com/VoltAgent/awesome-claude-code-subagents/network/members)
    
</div>


# Awesome Claude Code Subagents 中文版

本仓库是 Claude Code subagents 的权威集合，这些是专为特定开发任务设计的专业 AI 助手。

## 安装

### 作为 Claude Code 插件（推荐）

```bash
claude plugin marketplace add VoltAgent/awesome-claude-code-subagents
claude plugin install <plugin-name>
```

示例：
```bash
claude plugin install voltagent-lang    # 语言专家
claude plugin install voltagent-infra   # 基础设施和 DevOps
```

参见下方的[类别](#-categories)以获取所有可用的插件。

> **注意**：`voltagent-meta` 编排 agents 在安装其他类别时效果最佳。

### 选项 1：手动安装

1. 克隆此仓库
2. 将所需的 agent 文件复制到：
   - `~/.claude/agents/` 用于全局访问
   - `.claude/agents/` 用于项目特定使用
3. 根据你的项目需求进行自定义

### 选项 2：交互式安装程序

```bash
git clone https://github.com/VoltAgent/awesome-claude-code-subagents.git
cd awesome-claude-code-subagents
./install-agents.sh
```

此交互式脚本让你可以浏览类别、选择 agents，并使用单个命令安装/卸载它们。

### 选项 3：独立安装程序（无需克隆）

```bash
curl -sO https://raw.githubusercontent.com/VoltAgent/awesome-claude-code-subagents/main/install-agents.sh
chmod +x install-agents.sh
./install-agents.sh
```

直接从 GitHub 下载 agents，无需克隆仓库。需要 `curl`。

### 选项 4：Agent 安装程序（使用 Claude Code 安装 agents）

```bash
curl -s https://raw.githubusercontent.com/VoltAgent/awesome-claude-code-subagents/main/categories/09-meta-orchestration/agent-installer.md -o ~/.claude/agents/agent-installer.md
```

然后在 Claude Code 中："使用 agent-installer 显示可用的类别"或"查找 PHP agents 并全局安装 php-pro"。

<br />

<a href="https://github.com/VoltAgent/voltagent">
<img width="1390" height="296" alt="social" src="https://github.com/user-attachments/assets/5d8822c0-e97b-4183-a71e-a922ab88e1a0" />
</a>


## 📚 类别

### [01. 核心开发](categories/01-core-development/)
**插件：** `voltagent-core-dev`

日常编码任务的基本开发 subagents。

- [**api-designer**](categories/01-core-development/api-designer.md) - REST 和 GraphQL API 架构师
- [**backend-developer**](categories/01-core-development/backend-developer.md) - 可扩展 API 的服务端专家
- [**electron-pro**](categories/01-core-development/electron-pro.md) - 桌面应用专家
- [**frontend-developer**](categories/01-core-development/frontend-developer.md) - React、Vue 和 Angular 的 UI/UX 专家
- [**fullstack-developer**](categories/01-core-development/fullstack-developer.md) - 端到端功能开发
- [**graphql-architect**](categories/01-core-development/graphql-architect.md) - GraphQL schema 和联邦专家
- [**microservices-architect**](categories/01-core-development/microservices-architect.md) - 分布式系统设计器
- [**mobile-developer**](categories/01-core-development/mobile-developer.md) - 跨平台移动专家
- [**ui-designer**](categories/01-core-development/ui-designer.md) - 视觉设计和交互专家
- [**websocket-engineer**](categories/01-core-development/websocket-engineer.md) - 实时通信专家

### [02. 语言专家](categories/02-language-specialists/)
**插件：** `voltagent-lang`

具有深度框架知识的语言特定专家。

- [**typescript-pro**](categories/02-language-specialists/typescript-pro.md) - TypeScript 专家
- [**sql-pro**](categories/02-language-specialists/sql-pro.md) - 数据库查询专家
- [**swift-expert**](categories/02-language-specialists/swift-expert.md) - iOS 和 macOS 专家
- [**vue-expert**](categories/02-language-specialists/vue-expert.md) - Vue 3 Composition API 专家
- [**angular-architect**](categories/02-language-specialists/angular-architect.md) - Angular 15+ 企业模式专家
- [**cpp-pro**](categories/02-language-specialists/cpp-pro.md) - C++ 性能专家
- [**csharp-developer**](categories/02-language-specialists/csharp-developer.md) - .NET 生态系统专家
- [**django-developer**](categories/02-language-specialists/django-developer.md) - Django 4+ Web 开发专家
- [**dotnet-core-expert**](categories/02-language-specialists/dotnet-core-expert.md) - .NET 8 跨平台专家
- [**dotnet-framework-4.8-expert**](categories/02-language-specialists/dotnet-framework-4.8-expert.md) - .NET Framework 传统企业专家
- [**elixir-expert**](categories/02-language-specialists/elixir-expert.md) - Elixir 和 OTP 容错系统专家
- [**flutter-expert**](categories/02-language-specialists/flutter-expert.md) - Flutter 3+ 跨平台移动专家
- [**golang-pro**](categories/02-language-specialists/golang-pro.md) - Go 并发专家
- [**java-architect**](categories/02-language-specialists/java-architect.md) - 企业 Java 专家
- [**javascript-pro**](categories/02-language-specialists/javascript-pro.md) - JavaScript 开发专家
- [**powershell-5.1-expert**](categories/02-language-specialists/powershell-5.1-expert.md) - Windows PowerShell 5.1 和完整 .NET Framework 自动化专家
- [**powershell-7-expert**](categories/02-language-specialists/powershell-7-expert.md) - 跨平台 PowerShell 7+ 自动化和现代 .NET 专家
- [**kotlin-specialist**](categories/02-language-specialists/kotlin-specialist.md) - 现代 JVM 语言专家
- [**laravel-specialist**](categories/02-language-specialists/laravel-specialist.md) - Laravel 10+ PHP 框架专家
- [**nextjs-developer**](categories/02-language-specialists/nextjs-developer.md) - Next.js 14+ 全栈专家
- [**php-pro**](categories/02-language-specialists/php-pro.md) - PHP Web 开发专家
- [**python-pro**](categories/02-language-specialists/python-pro.md) - Python 生态系统大师
- [**rails-expert**](categories/02-language-specialists/rails-expert.md) - Rails 8.1 快速开发专家
- [**react-specialist**](categories/02-language-specialists/react-specialist.md) - React 18+ 现代模式专家
- [**rust-engineer**](categories/02-language-specialists/rust-engineer.md) - 系统编程专家
- [**spring-boot-engineer**](categories/02-language-specialists/spring-boot-engineer.md) - Spring Boot 3+ 微服务专家


### [03. 基础设施](categories/03-infrastructure/)
**插件：** `voltagent-infra`

DevOps、云和部署专家。

- [**azure-infra-engineer**](categories/03-infrastructure/azure-infra-engineer.md) - Azure 基础设施和 Az PowerShell 自动化专家
- [**cloud-architect**](categories/03-infrastructure/cloud-architect.md) - AWS/GCP/Azure 专家
- [**database-administrator**](categories/03-infrastructure/database-administrator.md) - 数据库管理专家
- [**deployment-engineer**](categories/03-infrastructure/deployment-engineer.md) - 部署自动化专家
- [**devops-engineer**](categories/03-infrastructure/devops-engineer.md) - CI/CD 和自动化专家
- [**devops-incident-responder**](categories/03-infrastructure/devops-incident-responder.md) - DevOps 事件管理
- [**incident-responder**](categories/03-infrastructure/incident-responder.md) - 系统事件响应专家
- [**kubernetes-specialist**](categories/03-infrastructure/kubernetes-specialist.md) - 容器编排大师
- [**network-engineer**](categories/03-infrastructure/network-engineer.md) - 网络基础设施专家
- [**platform-engineer**](categories/03-infrastructure/platform-engineer.md) - 平台架构专家
- [**security-engineer**](categories/03-infrastructure/security-engineer.md) - 基础设施安全专家
- [**sre-engineer**](categories/03-infrastructure/sre-engineer.md) - 站点可靠性工程专家
- [**terraform-engineer**](categories/03-infrastructure/terraform-engineer.md) - 基础设施即代码专家
- [**terragrunt-expert**](categories/03-infrastructure/terragrunt-expert.md) - Terragrunt 编排和 DRY IaC 专家
- [**windows-infra-admin**](categories/03-infrastructure/windows-infra-admin.md) - Active Directory、DNS、DHCP 和 GPO 自动化专家

### [04. 质量与安全](categories/04-quality-security/)
**插件：** `voltagent-qa-sec`

测试、安全和代码质量专家。

- [**accessibility-tester**](categories/04-quality-security/accessibility-tester.md) - A11y 合规专家
- [**ad-security-reviewer**](categories/04-quality-security/ad-security-reviewer.md) - Active Directory 安全和 GPO 审计专家
- [**architect-reviewer**](categories/04-quality-security/architect-reviewer.md) - 架构审查专家
- [**chaos-engineer**](categories/04-quality-security/chaos-engineer.md) - 系统弹性测试专家
- [**code-reviewer**](categories/04-quality-security/code-reviewer.md) - 代码质量守护者
- [**compliance-auditor**](categories/04-quality-security/compliance-auditor.md) - 法规合规专家
- [**debugger**](categories/04-quality-security/debugger.md) - 高级调试专家
- [**error-detective**](categories/04-quality-security/error-detective.md) - 错误分析和解决专家
- [**penetration-tester**](categories/04-quality-security/penetration-tester.md) - 道德黑客专家
- [**performance-engineer**](categories/04-quality-security/performance-engineer.md) - 性能优化专家
- [**powershell-security-hardening**](categories/04-quality-security/powershell-security-hardening.md) - PowerShell 安全加固和合规专家
- [**qa-expert**](categories/04-quality-security/qa-expert.md) - 测试自动化专家
- [**security-auditor**](categories/04-quality-security/security-auditor.md) - 安全漏洞专家
- [**test-automator**](categories/04-quality-security/test-automator.md) - 测试自动化框架专家

### [05. 数据与 AI](categories/05-data-ai/)
**插件：** `voltagent-data-ai`

数据工程、ML 和 AI 专家。

- [**ai-engineer**](categories/05-data-ai/ai-engineer.md) - AI 系统设计和部署专家
- [**data-analyst**](categories/05-data-ai/data-analyst.md) - 数据洞察和可视化专家
- [**data-engineer**](categories/05-data-ai/data-engineer.md) - 数据管道架构师
- [**data-scientist**](categories/05-data-ai/data-scientist.md) - 分析和洞察专家
- [**database-optimizer**](categories/05-data-ai/database-optimizer.md) - 数据库性能专家
- [**llm-architect**](categories/05-data-ai/llm-architect.md) - 大语言模型架构师
- [**machine-learning-engineer**](categories/05-data-ai/machine-learning-engineer.md) - 机器学习系统专家
- [**ml-engineer**](categories/05-data-ai/ml-engineer.md) - 机器学习专家
- [**mlops-engineer**](categories/05-data-ai/mlops-engineer.md) - MLOps 和模型部署专家
- [**nlp-engineer**](categories/05-data-ai/nlp-engineer.md) - 自然语言处理专家
- [**postgres-pro**](categories/05-data-ai/postgres-pro.md) - PostgreSQL 数据库专家
- [**prompt-engineer**](categories/05-data-ai/prompt-engineer.md) - Prompt 优化专家

### [06. 开发体验](categories/06-developer-experience/)
**插件：** `voltagent-dev-exp`

工具和开发者生产力专家。

- [**build-engineer**](categories/06-developer-experience/build-engineer.md) - 构建系统专家
- [**cli-developer**](categories/06-developer-experience/cli-developer.md) - 命令行工具创建者
- [**dependency-manager**](categories/06-developer-experience/dependency-manager.md) - 包和依赖专家
- [**documentation-engineer**](categories/06-developer-experience/documentation-engineer.md) - 技术文档专家
- [**dx-optimizer**](categories/06-developer-experience/dx-optimizer.md) - 开发体验优化专家
- [**git-workflow-manager**](categories/06-developer-experience/git-workflow-manager.md) - Git 工作流和分支专家
- [**legacy-modernizer**](categories/06-developer-experience/legacy-modernizer.md) - 遗留代码现代化专家
- [**mcp-developer**](categories/06-developer-experience/mcp-developer.md) - Model Context Protocol 专家
- [**powershell-ui-architect**](categories/06-developer-experience/powershell-ui-architect.md) - PowerShell UI/UX 专家，用于 WinForms、WPF、Metro 框架和 TUI
- [**powershell-module-architect**](categories/06-developer-experience/powershell-module-architect.md) - PowerShell 模块和配置文件架构专家
- [**refactoring-specialist**](categories/06-developer-experience/refactoring-specialist.md) - 代码重构专家
- [**slack-expert**](categories/06-developer-experience/slack-expert.md) - Slack 平台和 @slack/bolt 专家
- [**tooling-engineer**](categories/06-developer-experience/tooling-engineer.md) - 开发工具专家

### [07. 专业化领域](categories/07-specialized-domains/)
**插件：** `voltagent-domains`

领域特定的技术专家。

- [**api-documenter**](categories/07-specialized-domains/api-documenter.md) - API 文档专家
- [**blockchain-developer**](categories/07-specialized-domains/blockchain-developer.md) - Web3 和加密专家
- [**embedded-systems**](categories/07-specialized-domains/embedded-systems.md) - 嵌入式和实时系统专家
- [**fintech-engineer**](categories/07-specialized-domains/fintech-engineer.md) - 金融科技专家
- [**game-developer**](categories/07-specialized-domains/game-developer.md) - 游戏开发专家
- [**iot-engineer**](categories/07-specialized-domains/iot-engineer.md) - IoT 系统开发者
- [**m365-admin**](categories/07-specialized-domains/m365-admin.md) - Microsoft 365、Exchange Online、Teams 和 SharePoint 管理专家
- [**mobile-app-developer**](categories/07-specialized-domains/mobile-app-developer.md) - 移动应用专家
- [**payment-integration**](categories/07-specialized-domains/payment-integration.md) - 支付系统专家
- [**quant-analyst**](categories/07-specialized-domains/quant-analyst.md) - 量化分析专家
- [**risk-manager**](categories/07-specialized-domains/risk-manager.md) - 风险评估和管理专家
- [**seo-specialist**](categories/07-specialized-domains/seo-specialist.md) - 搜索引擎优化专家

### [08. 商业与产品](categories/08-business-product/)
**插件：** `voltagent-biz`

产品管理和商业分析。

- [**business-analyst**](categories/08-business-product/business-analyst.md) - 需求专家
- [**content-marketer**](categories/08-business-product/content-marketer.md) - 内容营销专家
- [**customer-success-manager**](categories/08-business-product/customer-success-manager.md) - 客户成功专家
- [**legal-advisor**](categories/08-business-product/legal-advisor.md) - 法律和合规专家
- [**product-manager**](categories/08-business-product/product-manager.md) - 产品策略专家
- [**project-manager**](categories/08-business-product/project-manager.md) - 项目管理专家
- [**sales-engineer**](categories/08-business-product/sales-engineer.md) - 技术销售专家
- [**scrum-master**](categories/08-business-product/scrum-master.md) - 敏捷方法论专家
- [**technical-writer**](categories/08-business-product/technical-writer.md) - 技术文档专家
- [**ux-researcher**](categories/08-business-product/ux-researcher.md) - 用户研究专家
- [**wordpress-master**](categories/08-business-product/wordpress-master.md) - WordPress 开发和优化专家

### [09. 元与编排](categories/09-meta-orchestration/)
**插件：** `voltagent-meta`

Agent 协调和元编程。

- [**agent-installer**](categories/09-meta-orchestration/agent-installer.md) - 通过 GitHub 浏览和安装此仓库中的 agents
- [**agent-organizer**](categories/09-meta-orchestration/agent-organizer.md) - 多 agent 协调器
- [**context-manager**](categories/09-meta-orchestration/context-manager.md) - 上下文优化专家
- [**error-coordinator**](categories/09-meta-orchestration/error-coordinator.md) - 错误处理和恢复专家
- [**it-ops-orchestrator**](categories/09-meta-orchestration/it-ops-orchestrator.md) - IT 运维工作流编排专家
- [**knowledge-synthesizer**](categories/09-meta-orchestration/knowledge-synthesizer.md) - 知识聚合专家
- [**multi-agent-coordinator**](categories/09-meta-orchestration/multi-agent-coordinator.md) - 高级多 agent 编排
- [**performance-monitor**](categories/09-meta-orchestration/performance-monitor.md) - Agent 性能优化
- [**pied-piper**](https://github.com/sathish316/pied-piper/) - 为重复的 SDLC 工作流编排 AI Subagents 团队
- [**task-distributor**](categories/09-meta-orchestration/task-distributor.md) - 任务分配专家
- [**workflow-orchestrator**](categories/09-meta-orchestration/workflow-orchestrator.md) - 复杂工作流自动化

### [10. 研究与分析](categories/10-research-analysis/)
**插件：** `voltagent-research`

研究、搜索和分析专家。

- [**research-analyst**](categories/10-research-analysis/research-analyst.md) - 综合研究专家
- [**search-specialist**](categories/10-research-analysis/search-specialist.md) - 高级信息检索专家
- [**trend-analyst**](categories/10-research-analysis/trend-analyst.md) - 新兴趋势和预测专家
- [**competitive-analyst**](categories/10-research-analysis/competitive-analyst.md) - 竞争情报专家
- [**market-researcher**](categories/10-research-analysis/market-researcher.md) - 市场分析和消费者洞察
- [**data-researcher**](categories/10-research-analysis/data-researcher.md) - 数据发现和分析专家

## 🤖 理解 Subagents

Subagents 是专业的 AI 助手，通过提供任务特定的专业知识来增强 Claude Code 的能力。当 Claude Code 遇到特定类型的工作时，可以调用它们作为专门的助手。

### Subagents 的特别之处

**独立的上下文窗口**  
每个 subagent 在其自己的独立上下文空间中运行，防止不同任务之间的交叉污染，并保持主对话线程的清晰度。

**领域特定智能**  
Subagents 配备了精心制作的指令，针对其专业领域，在特定任务上产生卓越的性能。

**跨项目共享**  
创建 subagent 后，你可以在各种项目中使用它，并在团队成员之间分发，以确保一致的开发实践。

**细粒度工具权限**  
你可以为每个 subagent 配置特定的工具访问权限，实现对不同任务类型可用能力的精细控制。

### 核心优势

- **内存效率**：隔离的上下文防止主对话被任务特定的细节弄得混乱
- **增强的准确性**：专门的提示和配置在特定领域产生更好的结果
- **工作流一致性**：团队范围的 subagent 共享确保对常见任务的统一方法
- **安全控制**：工具访问可以根据 subagent 类型和用途进行限制

### 开始使用 Subagents

**1. 访问 Subagent 管理器**
```bash
/agents
```

**2. 创建你的 Subagent**
- 在项目特定或全局 subagents 之间选择
- 让 Claude 生成初始版本，然后根据你的需求进行优化
- 提供 subagent 的用途和激活触发器的详细描述
- 配置工具访问（留空以继承所有可用工具）
- 使用内置编辑器自定义系统提示（按 `e`）

**3. 部署和利用**
你的 subagent 立即可用。Claude Code 将在适当时自动调用它，或者你可以明确请求它的帮助：
```
> 让 code-reviewer subagent 分析我的最新提交
```

### Subagent 存储位置

| 类型 | 路径 | 可用性 | 优先级 |
|------|------|--------------|------------|
| 项目 Subagents | `.claude/agents/` | 仅当前项目 | 更高 |
| 全局 Subagents | `~/.claude/agents/` | 所有项目 | 更低 |

注意：当发生命名冲突时，项目特定的 subagents 会覆盖全局的。


## 📖 Subagent 结构

每个 subagent 遵循标准化模板：

```yaml
---
name: subagent-name
description: 何时应该调用此 agent
tools: Read, Write, Edit, Bash, Glob, Grep
model: sonnet
---

你是一个[角色描述和专业领域]...
[Agent 特定的检查清单、模式和指南]...
## 通信协议
Agent 间通信规范...
## 开发工作流
结构化实现阶段...
```

### 工具分配哲学

### 智能模型路由

每个 subagent 包含一个 `model` 字段，自动将其路由到正确的 Claude 模型——平衡质量和成本：

| 模型 | 何时使用 | 示例 |
|-------|----------------|----------|
| `opus` | 深度推理——架构审查、安全审计、财务逻辑 | `security-auditor`、`architect-reviewer`、`fintech-engineer` |
| `sonnet` | 日常编码——编写、调试、重构 | `python-pro`、`backend-developer`、`devops-engineer` |
| `haiku` | 快速任务——文档、搜索、依赖检查 | `documentation-engineer`、`seo-specialist`、`build-engineer` |

你可以通过编辑其 frontmatter 中的 `model` 字段来覆盖任何 agent 的模型。设置 `model: inherit` 以使用你主对话正在使用的任何模型。

### 工具分配哲学

每个 subagent 的 `tools` 字段指定了 Claude Code 内置工具，针对其角色进行了优化：
- **只读 agents**（审查员、审计员）：`Read, Grep, Glob` - 分析而不修改
- **研究 agents**（分析师、研究员）：`Read, Grep, Glob, WebFetch, WebSearch` - 收集信息
- **代码编写者**（开发者、工程师）：`Read, Write, Edit, Bash, Glob, Grep` - 创建和执行
- **文档 agents**（编写者、文档员）：`Read, Write, Edit, Glob, Grep, WebFetch, WebSearch` - 通过研究进行文档

每个 agent 都具有最小的必要权限。你可以通过将 MCP 服务器或外部工具添加到 `tools` 字段来扩展 agents。

## 🧰 工具

### [subagent-catalog](tools/subagent-catalog/)
用于浏览和从此目录中获取 subagents 的 Claude Code 技能。

| 命令 | 描述 |
|---------|-------------|
| `/subagent-catalog:search <query>` | 按名称、描述或类别查找 agents |
| `/subagent-catalog:fetch <name>` | 获取完整的 agent 定义 |
| `/subagent-catalog:list` | 浏览所有类别 |
| `/subagent-catalog:invalidate` | 刷新缓存 |

**安装：**
```bash
cp -r tools/subagent-catalog ~/.claude/commands/
```



## 🤝 贡献

我们欢迎贡献！参见 [CONTRIBUTING.md](CONTRIBUTING.md) 获取指南。

- 通过 PR 提交新的 subagents
- 改进现有定义
- 报告问题和错误

## 贡献者 ♥️ 感谢
![Contributors](https://contrib.rocks/image?repo=VoltAgent/awesome-claude-code-subagents&max=500&columns=20&anon=1)

## 📄 许可证

MIT License - 参见 [LICENSE](LICENSE)

本仓库是由维护者和社区贡献的 subagent 定义的精选集合。所有 subagents 均"按原样"提供，不提供任何保证。我们不对任何 subagent 的安全性或正确性进行审计或保证。使用前请审查，维护者不对因使用它们而产生的任何问题承担责任。

如果你发现列出的 subagent 有问题或希望删除你的贡献，请[打开 issue](https://github.com/VoltAgent/awesome-claude-code-subagents/issues)，我们将及时处理。
