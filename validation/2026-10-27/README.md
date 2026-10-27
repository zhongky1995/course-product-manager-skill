# 2026-10-27 验证材料

本目录保存已执行检验的构造材料和实际作品，供阅读、核对及按需复测。结论与限制见[维护报告](../2026-10-27.md)。这些材料不是当前技能安装入口；安装使用仓库的`skills/course-product-manager/`。

## 版本、任务与设置

- [before-skill](before-skill/)：维护开始时有效安装副本，包含此前本地修改。它与较旧仓库提交03ea050不同，是实际对照基线。
- [材料](materials.md)、[三页原稿](pages-input/)、[七轮请求](requests.json)：两组收到相同输入，各自在同一连续上下文完成。
- [版本摘要](versions.json)：修改前、前六轮冻结候选及最终技能的SHA-256。前六轮候选与最终入口的两处文字差异见[candidate-to-final.diff](candidate-to-final.diff)；第七轮显式读取最终副本。
- [可见模型设置](visible-model-settings.json)：从本地可观察的执行元数据提取，两组七轮均为gpt-6-astra/high；第八轮仅对新版进行有明确诊断的返修，设置相同。
- [文件摘要](record-manifest.json)：复制入库的原始证据文件摘要。索引及维护报告不在此清单内，复制时没有修改作品内容。

## 实际产物与独立审读

| 请求 | 修改前有效版 | 新版 | 独立审读 |
| --- | --- | --- | --- |
| 设计与完整样章 | [设计](before/design.md)、[样章](before/lesson-1.md) | [设计](after/design.md)、[样章](after/lesson-1.md) | [第1—3轮](reviews/review-rounds-1-3.md) |
| 同样章两次“太虚”反馈 | [第二稿](before/lesson-2.md)、[第三稿](before/lesson-3.md) | [第二稿](after/lesson-2.md)、[第三稿](after/lesson-3.md) | 同上 |
| 局部概念改写 | [段落](before/local-rewrite.md) | [段落](after/local-rewrite.md) | [第4—5轮](reviews/review-rounds-4-5.md) |
| 三页整体修复 | [三页](before/pages/)、[说明](before/pages-repair-note.md) | [三页](after/pages/)、[说明](after/pages-revision-note.md) | 同上 |
| 逐字稿与阅读讲义 | [逐字稿](before/spoken.md)、[讲义](before/handout.md) | [逐字稿](after/spoken.md)、[讲义](after/handout.md) | [第6轮](reviews/review-round-6.md) |
| 只要设计初版 | [设计](before/design-only.md) | [设计](after/design-only.md) | [第7轮](reviews/review-round-7.md) |
| 第8轮具体诊断后的返修 | 无对应追加轮 | [反馈](repair-request-8.md)、[修订逐字稿](after/spoken-revised.md)、[修订讲义](after/handout-revised.md)、[修改说明](after/repair-note-8.md) | [返修复核](reviews/review-repair-8.md) |

匿名评审中的A对应本目录after，B对应before。评审时只收到匿名作品、任务和原材料，未收到此映射、技能版本或维护诊断。公开时保留评审原文与原始失败，不因映射公开改变结论。

## 解释结果时保留的边界

两版各有长处，本批不能证明新版整体优于修改前有效版。新版第六轮的前提遗漏真实保留，修复仅证明收到具体诊断后能有效返修。三页完成也没有独立证明“样板先通过，再放行扩展”的严格先后机制。

本轮显式提供并要求使用技能，没有验证自然语言自动选用的稳定性；没有真实学员试读、讲师实测、真实企业成效、其他模型/领域的稳定性，也不能由七轮连续修订推出压缩、交接及长期跨阶段持续有效。原课程实际制作的跟进是另一个观察范围，本目录不发布其私有正文或会话记录。

模型设置是已核对元数据的公开摘录；原始会话、读取调用及本机安装记录仍保存在维护报告所列本地证据目录，不包含在本目录中。本目录不新增测试平台，也不将文件摘要或格式检查当作教学质量证明。
