# Awesome Claude Agents - AI 开发团队 🚀

**用一支专业的 AI 团队增强 Claude Code**，它们协同工作构建完整功能、调试复杂问题，并使用专家级知识处理任何技术栈。

## ⚠️ 重要提示

**本项目处于实验阶段，会消耗大量 token。** 我正在使用 Claude 订阅积极测试这些 agents - 在复杂工作流中预期会有较高的 token 消耗。多 agent 编排每个复杂功能可能消耗 10-50k token。请谨慎使用并监控你的使用情况。

## 🚀 快速开始（3分钟）

### 前置条件
- **Claude Code CLI** 已安装并完成认证
- **Claude 订阅** - 密集的 agent 工作流所必需
- 包含代码库的活动项目目录
- **可选**：[Context7 MCP](docs/dependencies.md) 用于增强文档访问

### 1. 安装 Agents
```bash
git clone https://github.com/vijaythecoder/awesome-claude-agents.git
```

#### 选项 A：符号链接（推荐 - 自动更新）

**macOS/Linux:**
```bash
# 创建 agents 目录（如果不存在，保留现有 agents）
mkdir -p ~/.claude/agents

# 符号链接 awesome-claude-agents 集合
ln -sf "$(pwd)/awesome-claude-agents/agents/" ~/.claude/agents/awesome-claude-agents
```

**Windows (PowerShell):**
```powershell
# 创建 agents 目录
New-Item -Path "$env:USERPROFILE\.claude\agents" -ItemType Directory -Force

# 创建符号链接
cmd /c mklink /D "$env:USERPROFILE\.claude\agents\awesome-claude-agents" "$(Get-Location)\awesome-claude-agents\agents"
```

#### 选项 B：复制（静态 - 无自动更新）
```bash
# 创建 agents 目录（如果不存在）
mkdir -p ~/.claude/agents

# 复制所有 agents
cp -r awesome-claude-agents/agents ~/.claude/agents/awesome-claude-agents
```

### 2. 验证安装
```bash
claude /agents
# 应该显示所有 24 个 agents。
```

### 3. 初始化你的项目
**导航**到你的**项目目录**并运行以下命令来配置你的 AI 团队：

```bash
claude "使用 @agent-team-configurator 优化我的项目以最好地使用可用的 subagents。"
```

### 4. 开始构建
```bash
claude "使用 @agent-tech-lead-orchestrator 构建一个用户认证系统"
```

你的 AI 团队将自动检测你的技术栈并使用合适的专家！

## 🎯 自动配置如何工作

@agent-team-configurator 自动设置你的完美 AI 开发团队。当被调用时，它：

1. **定位 CLAUDE.md** - 查找现有项目配置并保留"AI 团队配置"部分之外的所有自定义内容
2. **检测技术栈** - 检查 package.json、composer.json、requirements.txt、go.mod、Gemfile 和构建配置以了解你的项目
3. **发现可用的 Agents** - 扫描 ~/.claude/agents/ 和 .claude/ 文件夹，构建所有可用专家的能力表
4. **选择专家** - 优先选择特定框架的 agents 而非通用 agents，始终包含 @agent-code-reviewer 和 @agent-performance-optimizer 以确保质量
5. **更新 CLAUDE.md** - 创建带时间戳的"AI 团队配置"部分，包含检测到的技术栈和任务|Agent|备注映射表
6. **提供使用指导** - 显示检测到的技术栈、选择的 agents，并提供开始构建的示例命令

## 👥 认识你的 AI 开发团队

### 🎭 编排器（3个 agents）
- **[技术负责人编排器](agents/orchestrators/tech-lead-orchestrator.md)** - 分析复杂项目并协调多步骤开发任务的高级技术负责人
- **[项目分析师](agents/orchestrators/project-analyst.md)** - 技术栈检测专家，实现智能 agent 路由
- **[团队配置师](agents/orchestrators/team-configurator.md)** - AI 团队设置专家，检测你的技术栈并配置最优的 agent 映射

### 💼 框架专家（13个 agents）
- **Laravel (2个 agents)**
  - **[后端专家](agents/specialized/laravel/laravel-backend-expert.md)** - MVC、服务和 Eloquent 模式的综合 Laravel 开发
  - **[Eloquent 专家](agents/specialized/laravel/laravel-eloquent-expert.md)** - 高级 ORM 优化、复杂查询和数据库性能
- **Django (3个 agents)**
  - **[后端专家](agents/specialized/django/django-backend-expert.md)** - 遵循当前 Django 约定的模型、视图和服务
  - **[API 开发者](agents/specialized/django/django-api-developer.md)** - Django REST Framework 和 GraphQL 实现
  - **[ORM 专家](agents/specialized/django/django-orm-expert.md)** - Django 应用的查询优化和数据库性能
- **Rails (3个 agents)**
  - **[后端专家](agents/specialized/rails/rails-backend-expert.md)** - 遵循约定的全栈 Rails 开发
  - **[API 开发者](agents/specialized/rails/rails-api-developer.md)** - RESTful API 和 Rails 模式下的 GraphQL
  - **[ActiveRecord 专家](agents/specialized/rails/rails-activerecord-expert.md)** - 复杂查询和数据库优化
- **React (2个 agents)**
  - **[组件架构师](agents/specialized/react/react-component-architect.md)** - 现代 React 模式、hooks 和组件设计
  - **[Next.js 专家](agents/specialized/react/react-nextjs-expert.md)** - SSR、SSG、ISR 和全栈 Next.js 应用
- **Vue (3个 agents)**
  - **[组件架构师](agents/specialized/vue/vue-component-architect.md)** - Vue 3 Composition API 和组件模式
  - **[Nuxt 专家](agents/specialized/vue/vue-nuxt-expert.md)** - SSR、SSG 和全栈 Nuxt 应用
  - **[状态管理器](agents/specialized/vue/vue-state-manager.md)** - Pinia 和 Vuex 状态架构

### 🌐 通用专家（4个 agents）
- **[后端开发者](agents/universal/backend-developer.md)** - 跨多种语言和框架的多语言后端开发
- **[前端开发者](agents/universal/frontend-developer.md)** - 任何框架的现代 Web 技术和响应式设计
- **[API 架构师](agents/universal/api-architect.md)** - RESTful 设计、GraphQL 和框架无关的 API 架构
- **[Tailwind 前端专家](agents/universal/tailwind-css-expert.md)** - Tailwind CSS 样式、实用优先开发和响应式组件

### 🔧 核心团队（4个 agents）
- **[代码考古学家](agents/core/code-archaeologist.md)** - 探索、文档化和分析不熟悉的或遗留代码库
- **[代码审查员](agents/core/code-reviewer.md)** - 严格的安全感知审查，提供严重性标记的报告
- **[性能优化师](agents/core/performance-optimizer.md)** - 识别瓶颈并应用优化以构建可扩展系统
- **[文档专家](agents/core/documentation-specialist.md)** - 编写全面的 README、API 规范和技术文档

**总计：24个专业 agents** 协同工作构建你的项目！

[浏览所有 agents →](agents/)

## 🔥 团队优于单独 AI 的原因

- **专业化知识**：每个 agent 都掌握其领域的深度、最新知识
- **真正协作**：agents 无缝协调，共享上下文并移交任务
- **定制解决方案**：获得完全匹配你技术栈并遵循其最佳实践的代码
- **并行执行**：多个专家同时工作以更快交付

## 📈 影响力

- **更快交付** - 在几分钟内完成功能，而不是几天
- **更好的代码质量** - 每一行都遵循最佳实践
- **边做边学** - 看看专家如何处理问题
- **自信扩展** - 为增长设计的架构

## 📚 了解更多

- [创建自定义 Agents](docs/creating-agents.md) - 为你的需求构建专家
- [最佳实践](docs/best-practices.md) - 从你的 AI 团队获得最大收益

## 💬 加入社区

- ⭐ **Star 这个仓库** 以示支持
- 🐛 [报告问题](https://github.com/vijaythecoder/awesome-claude-agents/issues)
- 💡 [分享想法](https://github.com/vijaythecoder/awesome-claude-agents/discussions)
- 🎉 [成功故事](https://github.com/vijaythecoder/awesome-claude-agents/discussions/categories/show-and-tell)

## 📄 许可证

MIT License - 在你的项目中自由使用！

## Star History

[![Star History Chart](https://api.star-history.com/svg?repos=vijaythecoder/awesome-claude-agents&type=Date)](https://www.star-history.com/#vijaythecoder/awesome-claude-agents&Date)

---

<p align="center">
  <strong>将 Claude Code 转变为一个交付生产就绪功能的 AI 开发团队</strong><br>
  <em>简单设置。强大结果。只需描述和构建。</em>
</p>

<p align="center">
  <a href="https://github.com/vijaythecoder/awesome-claude-agents">GitHub</a> •
  <a href="docs/creating-agents.md">文档</a> •
  <a href="https://github.com/vijaythecoder/awesome-claude-agents/discussions">社区</a>
</p>
