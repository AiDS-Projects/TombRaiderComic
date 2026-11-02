# 分镜 Prompt 索引（Shot Prompts Index）

> 工单：TK-20261102-be9014 — 搭建项目脚手架并建立章节数据模型与 mock 数据源
> 技能：director-prompts

## 状态
阻塞（Blocked）— 无法生成任何分镜 Prompt。

## 阻塞原因

| 必需输入 | 状态 |
| --- | --- |
| `video_brief` | 缺失（上游未产出）——无法确定 Mode（Explainer / Storytime / Drama） |
| `character_bible` | 缺失（`works/character-bible.md` 标记为 Blocked，无关键人物） |
| `voice_plan` | 缺失（`works/voice-plan.md` 标记为 Blocked，无音色清单） |
| `drama_breakdown` | 缺失（无片段/镜头拆解，无法产出「片段NN」） |
| `narration_script` | 缺失（无旁白/对白文本） |
| `scene_bible` | 缺失（`works/scene-bible.md` 标记为不适用/Blocked） |
| `director-knowledge/references/video-generation-prompt-guide.md` | 目录未检出，无法读取 Prompt 指南 |
| Mode 专属 Prompt 指南 | 无法确定 Mode，无法选择对应指南 |

## 说明
- 无片段（片段）来源：`drama_breakdown` / `narration_script` / `video_brief` 均缺失，故不存在可写 Prompt 的「片段NN」。
- 无 slug：上游未提供 `works/<slug>/` 目标路径，索引落在 `works/` 根目录，与其余 bible 一致。
- 本项目 `project_traits` 为 `platform:web` 但被标记 `category:video` / `pipeline:video`；实际为 Web 前端脚手架任务（Next.js + TypeScript + Tailwind），非视频制作，视频管线缺失上游产物属预期。

## 分镜 Prompt 清单
无。在上述必需输入产出前，不虚构任何镜头、时长、出场人物或 Prompt 内容。

| # | 片段路径 | 时长 | 出场人物 |
| --- | --- | --- | --- |
| — | 无 | — | — |
