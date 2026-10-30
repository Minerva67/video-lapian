# 拉片输出模板（Output Template）

This is the exact structure every 拉片 report must follow. It is modeled on a
gold-standard teardown of Google's "Welcome to the Gemini Era". Match this
depth and these sections. Default language: **中文**（除非用户要求英文）。

The report has two parts: **(1) 逐秒镜头表** and **(2) 十个分析章节**.

---

## Header block (always first)

```
# <品牌> "<视频标题>" — 商业视频拉片分析
> 视频: <url>
> 时长: <s>秒 | 发布: <date> | 频道: <channel> | 观看量: <views>
> 描述: <official description, trimmed>
> 分析日期: <today>
> 类型: <一句话定性，如 "B2B 硅片规格发布片" / "C 端功能广告" / "品牌情绪大片">
> ⚠️ 音频说明: <抽帧无法转写，注明音频为推断 + 置信度>
```

The **类型定性** matters — it sets the analytical lens. A functional demo, a
spec launch, an emotional brand film, and a consumer feature ad each get read
differently (see method-notes.md "按类型调整分析视角").

---

## 一、逐秒镜头表

Group rows into **幕 (acts)** with a scene title + time range. Each row is one
beat. Use a 6-column table. For films ≤60s aim for ~per-second/per-0.5s rows;
for 2-3 min films use per-shot/per-beat rows (every 1.5-3s where things change).

```
### 第X幕：<幕名 + 策略概括> (M:SS - M:SS)
| 时间 | 画面内容 | 景别/角度 | 视觉元素 | 音频 | 分析 |
|------|---------|----------|----------|------|------|
| 0:03 | <what's on screen> | <全屏UI / 特写 / 手持实拍 / 3D…> | <logo, 文字, 商品, UI 元素, 色块…> | <音乐/人声/AI语音/音效> | **<粗体点出策略意图>** + 展开 |
```

Rules that make the table good:
- The **分析** column is the value — say *why* this beat exists, not just what it shows. Bold the one-line takeaway.
- Read exact on-screen text (product names, spec numbers, UI labels, slogans) verbatim — zoom into individual frames when montage cells are too small.
- Note transitions and color/tone flips where they happen (they're structural).
- Keep the **音频** column honest: label it as inference unless you truly heard it.

---

## 二、产品展示策略分析
出场顺序与逻辑表（序号 | 产品/功能 | 时间 | 展示方式 | 策略意图），再用一段话总结**展示逻辑主线**（如 "从熟悉→有趣→实用→情感→前沿"）。

## 三、视觉设计语言分析
- **核心手法**：一句话点出这支片最独特的视觉引擎（如 "排版即演示" / "拟人化痛点" / "逐级放大" / "真实商品当排版元素"）。
- **色彩系统**表（色彩层 | 用途 | 色值/风格）。
- **色调切换节奏**：用缩进代码块画出色调/场景的切换流。
- **动态图形/MG 风格**：招牌转场与动效。

## 四、节奏与信息密度分析
节拍分布表（时间段 | 时长 | 镜头数 | 平均每镜头 | 信息密度 | 节奏感），再总结均速（几秒/镜头）+ **避免眩晕/维持注意的手段**。

## 五、场景与人物（多样性）
人物分布表（出现时间 | 人物描述 | 场景 | 族裔·年龄 | 功能）。点出**代入策略**（有无主角、去人物化/拟人化、多样性覆盖）。若无真人，说明"硬件/图标即主角"或"只有一只手做第一人称代入"。

## 六、音乐与声音设计
音乐选择 + 声音层次表（时间 | 声音层 | 内容）。⚠️ 明确标注推断与置信度。分析音乐/人声/AI语音/旁白的**有无与作用**（如 "歌词即文案" / "声画同源" / "无旁白，全靠屏幕文字"）。

## 七、文案与旁白策略
关键文案表（位置 | 文案 | 策略）。点出文案家族（如 **对仗式 slogan** / **动词祈使句** / **参数冷+形容词热双轨** / **零参数全感受**）。

## 八、转场与视觉连贯性
主要转场手法表（转场类型 | 使用位置 | 效果），再用缩进代码块画出**视觉逻辑线**（一句话一层的叙事流）。

## 九、情绪曲线
用 ASCII 画一条情绪/信心/愉悦曲线（横轴时间），标出 5-7 个**情绪节点**（时间 + 事件 + 性质）。注意不同类型片的曲线不同：情绪片=多小高潮+终极高潮+急刹；技术片=焦虑(痛点)→释然→信心；功能广告=愉悦→惊喜→兴奋。

## 十、对<受众>视频生成技术的可参考模板
- **提炼的脚本结构模板**：用缩进代码块写出 Phase 1..N（每 Phase 的时长 + 目的 + 手法）。
- **关键制作要素清单**表（要素 | 本片的做法 | 可参考方向），覆盖 音乐/节奏/文案/人物/转场/色彩/收束/时长。
- 结尾一句 **"最大启发"**：这支片最值得偷师的一招。

---

## 质量准则
- 忠于所见：所有画面描述来自实际抽帧，不臆造。看不清就 zoom 单帧确认。
- 屏幕文字（产品名、参数、slogan、UI 标签）逐字准确 —— 这是可信度的地基。
- 音频诚实：无法转写就标注为推断 + 置信度，不假装听写。
- 每个分析都回答 "**为什么**"，而不只是 "是什么"。
- 报告服务于目标：多数拉片是为**竞品分析 / 给自己产品做参考**，第十节的可复用模板往往是用户最想要的。
