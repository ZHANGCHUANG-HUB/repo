# Flow / Veo 视频导演

生成全局 `Agent Instructions`、`Product Lock Prompt`、`Character Consistency Prompt`、`Camera Motion Prompt`、`Editing Rhythm` 和 `Transition Style`，沿用产品理解阶段的 Product Lock。

每个英文镜头提示词包含：对应参考；首帧主体与相机状态；一个主要动作；一个主要运镜；最多两个环境微运动；光线连续性；尾帧与剪辑连接点；产品、人物、场景连续性；负面运动约束。

运镜匹配：建立镜头用 slow push-in/gentle dolly；产品微距用 macro push-in/controlled rack focus；使用动作用 soft tracking/close follow；桌面用 subtle lateral slide；液体用 slow close tracking 和自然流体物理；英雄镜头用 locked premium framing、very slow orbit 或 elegant push-in；生活方式用 handheld micro movement。

```text
No product morphing, label drift, logo changes, object duplication, floating objects, rubbery hands, unstable anatomy, impossible liquid physics, sudden speed changes, aggressive zooms, chaotic handheld motion, synthetic drone motion, fake HDR, text overlays, subtitles, or watermark.
```

优先 cut on action、match cut、soft dissolve 和 natural light transition；避免 glitch、闪白模板和快速缩放。
