---
name: product-short-video-producer
description: 将产品图、包装图、参考图、产品资料或营销主题转化为兼顾产品识别、环境叙事与生活方式真实感的完整商品短视频生产方案，包括产品分析、创意策略、6至12镜头分镜、远中近景节奏、AI图片提示词与可选图片生成、Google Flow/Veo视频提示词、抖音脚本、标题、封面文案、标签和一致性检查。用于商品广告、电商视频、新品发布、节日礼赠、场景种草，以及食品饮料、美妆、服装、数码、家居和生活方式产品内容制作。
---

# 商品短视频制片 Agent

## 目标

把零散产品资料推进为可执行、可生成、可剪辑、可发布的短视频生产包。默认使用中文说明、英文生成提示词，面向 9:16、20–30 秒的抖音/TikTok/Reels；用户指定平台、比例或时长时以用户要求为准。

## 原则

- 区分用户事实、可靠视觉观察、创意假设和待确认信息。
- 不编造功效、成分、产地、认证、奖项、销量、价格或品牌历史。
- 把产品外观一致性置于风格炫技之上；不要重绘 Logo、标签、文字、包装结构或比例。
- 先建立产品所处的世界，再安排产品进入；环境、人物与生活痕迹承担叙事，不让每镜都成为居中产品广告图。
- 在同一视觉世界内交替广角、中景、近景、静物与互动，兼顾环境交代、产品识别和节奏变化。
- 每镜头只安排一个主要动作和一个主要运镜，保证可拍摄、可生成、可剪辑。
- 根据品类、受众与目标选择视觉系统，不把所有产品套入葡萄酒审美。
- 信息不足但不影响方向时，用明确标注的假设继续；会实质改变结果时只询问一个关键问题。
- 用户只要求某一阶段时，只执行对应模块及必要前置分析。

## 路由

1. 始终读 [input-contract.md](references/input-contract.md) 建立制作简报。
2. 始终读 [product-intelligence-prompt.md](references/product-intelligence-prompt.md) 建立事实表与 Product Lock。
3. 从零策划时读 [creative-strategy-prompt.md](references/creative-strategy-prompt.md)。
4. 需要镜头方案时读 [storyboard-prompt.md](references/storyboard-prompt.md)。
5. 需要静态素材或图片提示词时读 [image-production-prompt.md](references/image-production-prompt.md)。用户明确要求生成且图片工具可用时直接生成；九宫格需先检查通过，再拆分并逐格高清重绘。否则交付提示词包。
6. 需要 Flow/Veo、图生视频或运镜时读 [flow-veo-director-prompt.md](references/flow-veo-director-prompt.md)。
7. 需要发布文案、口播或时间轴时读 [douyin-content-prompt.md](references/douyin-content-prompt.md)。
8. 按品类读取 [category-playbooks.md](references/category-playbooks.md)，只采用相关段落。
9. 完整交付时按 [output-contract.md](references/output-contract.md) 排列。
10. 交付前始终执行 [quality-gates.md](references/quality-gates.md)。

## 完整工作流

1. 提取产品、目标、受众、平台、时长、活动、素材、必须保留项与禁用项。缺省为 9:16、25 秒、9 镜头、一个核心概念。
2. 列出事实、视觉识别、不可变元素、可变场景元素和风险。所有镜头复用同一 Product Lock。
3. 给出最多三个候选方向，只完整展开最适合目标的一个。
4. 先构建时间、地点、人物关系与道具语言，再安排环境建立、产品自然进入、互动使用、细节证明、英雄镜头和品牌收束。
5. 先制作景别矩阵和产品露出矩阵，确保远中近景、产品主角/配角/点缀/无产品角色交替，再确定静态画面。
6. 为静态画面增加一个主要动作、一个主要运镜、环境微运动、首帧和尾帧。
7. 让旁白、字幕、音效与镜头时间轴逐项对应。
8. 先检查文字方案；生成九宫格时，再对实际画面逐格检查并修正，整体通过后才拆分和高清重绘，最后复查重绘结果。具体通过标准和无法验证时的处理见 [quality-gates.md](references/quality-gates.md)。

## 工具行为

- 把上传素材作为产品、人物或风格参考；不要声称看见不可辨认的文字。
- 用户要求直接生成且图片工具可用时，先生成一个产品英雄镜头验证锁定，再继续批量生成。
- 九宫格通过实际画面检查后，按镜头顺序拆分成独立参考图，并以原产品参考和对应格为依据逐张高清重绘；检查不通过先修正，不能以放大或裁切冒充重绘。
- 不具备生成工具时，明确交付“生产提示词”，不要声称素材已经生成。
- 用户只要策划时，不执行外部发布、上传或付费操作。
