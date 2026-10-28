# 开发记录

## [2026-10-26 19:38] 归档等价无穷小的四个疑问

- **需求/问题描述**：
  > 根据用户提供的学习总结，整理等价无穷小代换的适用条件、主要项抵消、和差代换及整体代换四个疑问。

- **实际实现的功能与改动**：
  - 建立四条 `open` 疑问及最小疑问模板，保留例题和待本人复述的“我的理解”。
  - 补充积商比值证明、和差代换的总误差判据及整体代换的恒等变形；说明一般渐近等价与等价无穷小的区别。
  - 初始化本次任务的协作、计划、进度、验证与注意事项记录。
  - 验证：4 条记录的 YAML、日期、状态、标签、章节、公式块及 10 个内部链接检查通过；原极限及三个等价关系在正负邻近点的数值交叉检查通过；数学推导写入正文。`git diff --check` 通过。
  - 仓库没有测试套件及复习脚本，未执行复习流程或视觉验证。

- **涉及文件**：
  - `templates/question.md`
  - `questions/2026-10-26-等价无穷小的积商代换.md`
  - `questions/2026-10-26-主要项抵消与高阶无穷小.md`
  - `questions/2026-10-26-和差中的等价代换条件.md`
  - `questions/2026-10-26-整体等价与局部代换.md`
  - `memory/agents.md`、`memory/plan.md`、`memory/progress.md`、`memory/verify.md`、`memory/gotchas.md`
  - `docs/CHANGELOG.md`

- **Git 提交**：`708772acf243cc198c9cfcfe7db881a632653b49 docs: archive four questions on equivalent infinitesimal substitution`，已推送至 `origin/main`。

---

## [2026-10-28 22:21] 归档 C 自增与自减笔记

- **需求/问题描述**：
  > 整理用户提供的 Notion 截图中关于自增、自减运算的内容。

- **实际实现的功能与改动**：
  - 新增 C 知识笔记，转录原代码与输出，整理四种运算的对照表、逐句执行过程及可迁移的教训；保存原始截图并引用。
  - 区分表达式值与变量最终值；没有错误过程或具体疑问，不填写错因、掌握程度或本人理解。
  - 使用 Apple Clang 17.0.0 按 C17 编译运行，输出与截图一致；四组运算断言、YAML、章节、图片链接和图片 SHA-256 一致性检查通过。
  - 原示例 `int main()` 产生一条 `-Wstrict-prototypes` 警告，已在笔记中注明；未执行复习流程或额外视觉验证。
  - 验证中间文件位于 `.agent/work/` 并由 `.gitignore` 排除；更新计划、进度与验证记录。`git diff --check` 通过。

- **涉及文件**：
  - `programming/c/2026-10-28-自增与自减.md`
  - `assets/2026-10-28-自增与自减-1.png`
  - `.gitignore`
  - `memory/agents.md`、`memory/plan.md`、`memory/progress.md`、`memory/verify.md`
  - `docs/CHANGELOG.md`

- **Git 提交**：`cb0b5be3a46013dae92f2c112fe30149c967994b docs: archive C increment and decrement notes`，已推送至 `origin/main`。

---
