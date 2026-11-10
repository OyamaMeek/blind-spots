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

## [2026-11-05 10:15] 归档导数定义与可导性学习总结

- **需求/问题描述**：
  > 整理用户提供的导数定义、含绝对值函数的可导性、极限与导数、左右导数及夹逼定理学习总结。

- **实际实现的功能与改动**：
  - 按现有模板新增四条 `open` 疑问，保留待本人复述的“我的理解”；区分明确疑惑与总结中的推测。
  - 新增夹逼定理知识笔记，保留原题和推导，注明掌握情况未经验证。
  - 补充有限导数、邻域及夹逼条件，注明 $x^2|x|=|x|^3$；没有原始个人错误过程，不创建错题或虚构错因。
  - 验证：Ruby 标准库检查五份记录的 YAML、日期、标签、状态、章节、公式块及 12 个内部链接通过；六个正负邻近点的差商与夹逼上界交叉检查通过。数学依据写入正文，采样不作为极限证明。
  - `git diff --check` 通过；未执行复习流程或视觉验证。检查脚本位于已忽略的 `.agent/work/`。

- **涉及文件**：
  - `questions/2026-11-05-含绝对值函数的可导性.md`
  - `questions/2026-11-05-函数极限与导数的区别.md`
  - `questions/2026-11-05-导数定义与差商极限.md`
  - `questions/2026-11-05-左右导数与可导性.md`
  - `math/analysis/2026-11-05-夹逼定理在导数定义中的应用.md`
  - `memory/agents.md`、`memory/plan.md`、`memory/progress.md`、`memory/verify.md`
  - `docs/CHANGELOG.md`

- **Git 提交**：`f905c14f0aa03b8aecd126a1c7b09ad18df32fdd docs: archive derivative definition and differentiability notes`，已推送至 `origin/main`。自动审批曾拒绝推送；用户了解目标为公开仓库并明确确认后，普通推送成功。实际提交哈希由后续文档提交补记。

---

## [2026-11-07 11:28] 归档 C 条件表达式的两条疑问

- **需求/问题描述**：
  > 整理第（5）题的条件真假判断和第（6）题的嵌套条件表达式。

- **实际实现的功能与改动**：
  - 分别归档两条 `open` 疑问，保留原表达式和给定数值，补充示例与分支求值过程。
  - 验证：两个 C17 示例在 Apple Clang 17.0.0 下无警告编译，运行结果与文档一致。YAML、模板章节、三个内部链接及 `git diff --check` 检查通过。

- **涉及文件**：
  - `questions/2026-11-07-C条件表达式的真假判断.md`
  - `questions/2026-11-07-C嵌套条件表达式的结合性.md`
  - `memory/agents.md`、`memory/plan.md`、`memory/progress.md`、`memory/verify.md`
  - `docs/CHANGELOG.md`

- **Git 提交**：`818f4f62ce29f719730b8328c27c08a4f267fc3d docs: archive C conditional expression questions`，已推送至 `origin/main`。

---

## [2026-11-07 11:36] 归档 C++ 1003 最大连续区间和复习清单

- **需求/问题描述**：
  > 将 1003 最大连续区间和的复习清单写入仓库，归为 C++。

- **实际实现的功能与改动**：
  - 保存三条已提出的疑问、五条待自测项和逐元素手算练习，说明相同区间和时的更新行为。
  - Ruby 标准库核对 YAML 和清单结构通过，`git diff --check` 通过。材料未附 C++ 源代码，未运行程序。

- **涉及文件**：
  - `programming/cpp/2026-11-07-1003-最大连续区间和.md`
  - `memory/agents.md`、`memory/plan.md`、`memory/progress.md`、`memory/verify.md`
  - `docs/CHANGELOG.md`

- **Git 提交**：`1801d093a2323c9177f18f5ea7299551d9f9dbda docs: archive C++ problem 1003 review checklist`，已推送至 `origin/main`。

---

## [2026-11-07 13:07] 按需创建归档目录的规则

- **需求/问题描述**：
  > 将按需创建文件夹并写入对应目录的规则写入 AGENTS.md。

- **实际实现的功能与改动**：
  - 疑问、错题和知识笔记按科目与主题归档，优先复用目录，缺少合适目录时按需创建文件夹。
  - 更新疑问命名、处理和期末复盘约定，同步 `CLAUDE.md`；`questions/` 保留现有历史记录。
  - 验证：`cmp AGENTS.md CLAUDE.md` 和 `git diff --check` 通过；已检查差异范围，仅修改归档规则及协作记录，未迁移现有疑问。

- **涉及文件**：
  - `AGENTS.md`、`CLAUDE.md`
  - `memory/gotchas.md`、`memory/progress.md`
  - `docs/CHANGELOG.md`

- **Git 提交**：`21bc2dcb71f43e13b29bcdfa3a96d7943b0efaeb docs: organize questions by subject directory`，已推送至 `origin/main`；实际提交哈希通过后续文档提交补记。

---

## [2026-11-09 00:12] 归档反对称矩阵乘积的充要条件错题

- **需求/问题描述**：
  > 根据第 8 题（3）的学习总结，整理矩阵因子消去、对称与反对称定义，以及充要条件证明中的问题；用户已确认题面。

- **实际实现的功能与改动**：
  - 新增线性代数错题，保留总结提供的错误步骤、错误归纳和复习顺序，状态为 `未掌握`，主错因为 `概念不清`。
  - 补全两种矩阵定义及完整等价证明，说明同侧可逆因子的消去规则、零矩阵边界；区分本次使用正确的乘积转置与需要巩固的符号规则。
  - 来源仅为所贴总结和用户确认的题面；没有原始手写或红笔修改，不补写缺失的修改过程，不确认本人已掌握。
  - 验证：Ruby 检查 YAML、必需章节和公式块通过；729 对三阶整数反对称矩阵及一对乘积非零的四阶反对称矩阵交叉检查通过，并验证可逆矩阵的异侧因子也不能直接消去。数学证明写入正文，样例不替代证明。
  - `git diff --check` 通过；检查脚本保存在已忽略的 `.agent/work/`。仓库没有测试套件及复习脚本，未执行复习调度或视觉验证。

- **涉及文件**：
  - `math/linear-algebra/2026-11-09-反对称矩阵乘积的充要条件.md`
  - `memory/agents.md`、`memory/plan.md`、`memory/progress.md`、`memory/verify.md`
  - `docs/CHANGELOG.md`

- **Git 提交**：`49a1e0ba93c1c8c01554d25cc242af308197da79 docs: archive skew-symmetric matrix product proof`，已推送至 `origin/main`；实际提交哈希通过后续文档提交补记。

---

## [2026-11-10 23:02] 归档第 236 题

- **需求/问题描述**
  > 整理第 236 题中识别幂指极限、构造第二个重要极限和凑导数差商的思路。

- **实际实现的功能与改动**
  - 依据学习总结复原题面，记录最初的思路卡点和后来独立完成的差商拆分。错因记为「思路卡住」。
  - 补齐底数为正、去心邻域内 $u\ne0$ 及左右两侧的推导，得到极限 $e^2$。
  - Ruby 检查 YAML、必需章节、公式块及四个正负邻近点的计算通过。`git diff --check` 通过。

- **涉及文件**
  - `math/analysis/2026-11-10-第236题-幂指极限与导数定义.md`
  - `memory/agents.md`、`memory/plan.md`、`memory/progress.md`、`memory/verify.md`
  - `docs/CHANGELOG.md`

- **Git 提交** `d4f8297398c939f4f58c5734f1e959632c04ea22 docs: archive problem 236 power limit`，已推送至 `origin/main`。

---

## [2026-11-10 23:06] 归档第 235 题

- **需求/问题描述**
  > 将题图中的第 235 题录入数学分析错题，记下第一次没有做出来。

- **实际实现的功能与改动**
  - 转录题面，附上去除元数据的题图，记为「思路卡住」与「未掌握」。
  - 根据比值极限和连续性求出 $f(x_0)=0$，再拆成两个导数差商，得到 $f'(x_0)=1/6$。
  - YAML、章节、公式、题图链接、图像像素与四个正负步长的差商检查通过。`git diff --check` 通过。

- **涉及文件**
  - `math/analysis/2026-11-10-第235题-等价无穷小与导数定义.md`
  - `assets/2026-11-10-第235题-等价无穷小与导数定义-1.png`
  - `memory/agents.md`、`memory/plan.md`、`memory/progress.md`、`memory/verify.md`
  - `docs/CHANGELOG.md`

- **Git 提交** `191710abfdda1995f3894d15baeb13696c85b115 docs: archive problem 235 derivative exercise`，已推送至 `origin/main`。

---
