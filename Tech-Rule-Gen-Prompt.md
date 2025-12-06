# 技术规则文档生成请求

## 目标
为 **[主题/技术名称]** 创建一份开发规则文档

## 输出要求
- **受众**: AI Agent（机器可读优先）
- **风格**: 规则驱动、极简主义、Token 高效
- **语言**: 纯英文
- **用途**: Vibe Coding 快速参考

## 模板与路径
- **使用模板**: `@agent_docs/_templates/tech_rule.md`
- **输出位置**: `项目根目录/agent_docs/tech_guidance/`
- **文件命名**: 使用 kebab-case，能准确反映内容（例如：`spring-boot-rest-api-rules.md`）

## 文档结构（必须包含）
1. **Axioms** - 核心不可变原则
2. **Mapping Rules** - 禁止 vs 必须的对照表
3. **Critical Snippets** - 最小可用代码范式
4. **Verification** - 可执行的检查清单

## 优化原则
- ❌ 避免冗长解释和理论背景
- ✅ 优先使用表格、代码片段、清单
- ✅ 每条规则必须可操作、可验证
- ✅ 代码示例仅保留"正确范式"（Good Pattern）
