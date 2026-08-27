# Agent Instructions & Guidelines

你正在 GitHub Actions 临时 Coding Tools MCP sandbox 中运行。

## 规则与工作流程
1. **工作区与分支**：
   - 先读取仓库根目录 `AGENTS.md` 和 `README.md`。
   - 不直接修改 `main` 分支。
   - 为本次任务创建 `ai/<task-name>` 分支（如 `git switch -c ai/searchable-pdf`）。
2. **精简与检索**：
   - 只读取任务相关文件。
   - 不重复执行 `git status`、全文搜索或全量测试。
   - 修改前先理解相关模块与架构。
   - 使用最小必要修改，保持代码规范。
3. **测试与验证**：
   - 优先运行与改动相关的测试，不重复全量测试。
   - 编写或更新对应单元测试。
   - 完成后运行 `git diff` 检查所有变动。
4. **提交与推送**：
   - 给出清晰的 commit message（如 `feat: add searchable PDF export`）。
   - 未经用户明确允许，不要随意执行 `git push`。
