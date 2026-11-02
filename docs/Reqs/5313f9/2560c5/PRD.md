# PRD — 第一集视频简报：定 Mode 与剧情定位

> 所属需求：第一集试片：龙三角的呼唤

## 用户故事
As a 视频导演/制片人，I want to 为第一集试片「龙三角的呼唤」产出一份 video_brief，明确 Mode 与剧情定位，So that 后续分镜拆解与镜头生成有统一的方向基准，避免风格漂移与反复返工。

## 功能需求
1. 确定本片 Mode = cinematic-drama（剧情影像），与项目「写实电影感 AI 漫剧」定位一致。[假设] 用户未显式指定 Mode，依据项目特征 category:video 与「写实电影感」定位倾向 Drama，需在 brief 中显式声明该选择并给出理由。
2. 产出剧情定位，至少包含四项：题材类型（冒险/动作/悬疑）、主角（劳拉·克劳馥）、核心冲突（第一卷第一章「龙三角的呼唤」的主线矛盾）、叙事基调（写实、电影感、紧张）。
3. 明确目标时长与受众：给出单镜头时长区间与整集镜头规模预估，受众一句话定位。
4. 确定视觉 style（写实电影感），与 Mode 对应，不设静默默认。[假设] style 需在 brief 中显式列出，供后续分镜与生图 Prompt 复用。
5. 将产出保存为结构化文件 works/<slug>/video_brief.json，字段包含 mode、genre、protagonist、core_conflict、tone、style、target_duration、audience，供后续分镜流程读取。

## 验收标准
- video_brief 文档产出，且 mode 字段值 = "cinematic-drama"（字符串精确匹配，0/1 校验）。
- 剧情定位包含 ≥4 个字段且均非空：genre、protagonist、core_conflict、tone。
- target_duration 为数值区间（单镜头 10–15 秒），整集镜头规模给出明确数量（如 N 个镜头）。
- audience 字段为 ≥1 句的目标人群描述，非空字符串。
- style 字段非空，且与 Mode（cinematic-drama）语义匹配。
- 产出文件可被定位：works/<slug>/video_brief.json，JSON 可被解析且字段名与约定一致。

## 边界条件（不做的事）
1. 不拆分镜头（shot_prompts 属下一工单）。
2. 不执行 gen_video 生图/视频生成，本工单仅产 brief。
3. 不做网页 / Next.js / 前端页面。
4. 不生成整集全部镜头，仅完成 video_brief 这一最小步骤。
5. 不生成完整讲稿/正式视频 Prompt（讲稿确认前不写正式视频 Prompt）。

## 资产需求线索
暂无。本工单为视频简报/文案阶段，不涉及图标、插画、背景图、音效、背景音乐、骨骼动画、粒子特效等资产。
