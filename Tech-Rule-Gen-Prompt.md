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

## 使用场景
参考以下的风格，基于当前的项目背景，为当前技术规则文档输出一句简明扼要的“智能导航”式场景触发词： → 这是不属于**使用模板**的部分，请你另外输出，不要放到当前技术文档的最终输出产物中（例如：`spring-boot-rest-api-rules.md`）
```
- `edt-threading-rules.md`: 当你开发IntelliJ插件的 Swing UI 操作时或者需要执行耗时操作（如网络请求、文件 IO、AI 调用）时查阅该规则
- `intellij-psi-usage-rules.md`: 当你需要读取或修改IntelliJ插件开发SDK提供的的 Java/Kotlin 源代码的结构化表示（Program Structure Interface）时查阅，例如分析代码元素（类、方法、字段）、生成代码、执行代码重构等
- `intellij-swing-ui-rules.md`: 当你在IntelliJ插件开发中需要创建或修改Swing UI组件时查阅该规则，例如处理线程安全、组件创建、主题适配、对话框显示等UI操作
- `intellij-theme-adaptation-rules.md`: 当你在IntelliJ插件UI代码开发中需要确保自定义 UI 组件在浅色和深色主题下都能正确显示时查阅该规则
- `kotlin-idea-plugin-tdd-testing.md`: 当你开始实现一个新的后端功能时。当你需要在 src/test/kotlin 目录下创建或修改测试文件时查阅该规则
- `kotlin-mockk-testing-rules.md`: 当你的测试需要模拟（mock）IntelliJ 平台服务（如 Project, Editor, PsiFile）或其他依赖项、或需要隔离外部依赖（如数据库、网络请求、文件系统）、或使用JUnit 5 注解（如 `@Test`, `@BeforeEach`, `@AfterEach`）时查阅该规则
- `okhttp-proxy-auto-detection-rules.md`: 当你需要在Intellij插件构建新的 OkHttpClient 处理Intellij的代理时
- `nekoama-tab-extension-system-rules.md`: 当你需要为 Nekoama 工具窗口添加一个新的标签页时查阅该规则
```
