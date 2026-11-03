# 图片素材生产

逐镜头英文提示词按以下顺序写：主体与精确产品身份；动作；场景、表面、道具与背景层次；构图、景别与角度；光线、色彩与氛围；镜头语言与景深；材质、阴影与反射；Product Lock 摘要；比例与干净画面；负面提示词。

## 组图节奏

先为整组素材写一个共享视觉控制块：地点家族、时间段、光线方向、低饱和色板、表面与材质、人物造型、道具家族、摄影真实感。每个提示词完整重复必要控制，但改变叙事任务、景别和角度。

- 环境建立镜头：用 24–35mm 广角或等效视感，描述空间布局、前中后景、天气、人物尺度和负空间；产品不出现或只作点缀。
- 生活方式镜头：用 35–50mm 中景，产品自然处于桌边、手边或活动路径中，不强制居中或正面。
- 互动镜头：明确一个简单可信的手部/人物动作，并保留足够环境信息。
- 英雄镜头：用 50–85mm，确保产品清晰可识别；只在必要镜头采用正面居中构图。
- 细节镜头：用 85–100mm 微距，强调材质、标签、质地或可见过程。
- 收束镜头：回响开场的光线、颜色或环境物件，保留呼吸感和文字安全区。

不要在每个提示词中都要求 `centered product`, `full bottle visible`, `label facing camera` 或极浅景深。只有品牌识别、英雄和标签镜头需要这些约束。环境镜头应让背景可读，使用中等或深景深；生活方式镜头让产品像真实生活中的一部分，而不是贴入广告背景。

通用负面提示词：

```text
warped product, altered packaging, changed logo, invented label text, mirrored typography, duplicate product, incorrect proportions, floating objects, deformed hands, extra fingers, plastic skin, fake HDR, oversaturation, artificial reflections, inconsistent shadows, cluttered composition, text overlay, subtitle, watermark, low resolution, cheap e-commerce styling, fake luxury styling, overly staged commercial poster look
```

用户要求直接生成且工具可用时，先生成产品英雄镜头，检查轮廓、比例、结构、主色、Logo 区域和材质；锁定合格描述后再生成其余镜头。文字无法稳定生成时保留真实标签结构并建议后期合成，不虚构文字。

生成九宫格时，以通过方案检查的镜头表为依据，确保每格独立、顺序清晰且主体不跨格。生成后按 [quality-gates.md](quality-gates.md) 实际检查并修正；通过前不得拆分或重绘。通过后拆出各格作为参考，结合原始产品参考逐格高清重绘，再检查重绘结果。缺少生成、图像查看或必要参考时如实说明限制，不把提示词、裁切图或放大图说成已完成的高清重绘。
