# video-lapian

- Produce a deep shot-by-shot teardown (拉片 / 逐秒镜头表 + 十节分析) of a commercial, ad, or product-launch video — the kind of competitive/creative analysis where you break the film into per-beat shots and analyze visual language, pacing, copy, music, transitions, emotion curve, and a reusable script template. Use this WHENEVER the user gives a video URL (YouTube etc.) or local video file and asks to 拉片 / 拉这个片 / 逐帧或逐秒分析 / 分镜分析 / "break down this ad" / "shot-by-shot" / "分析这支广告/宣传片/发布视频" / teardown / competitive video analysis — even if they don't say the word "拉片". Also triggers when they want to study a reference video to inform their own product/marketing video. Downloads the video, extracts frames, and writes the full structured report. Default output language 中文.

一个 Claude Code skill。来自合集 [claude-skills](https://github.com/Minerva67/claude-skills)。

## 安装

```bash
git clone https://github.com/Minerva67/video-lapian.git ~/.claude/skills/video-lapian
```

装好后在 Claude Code 里输入 `/video-lapian`，或者直接描述任务，符合条件时会自动触发。

## 文件

```
SKILL.md
references/method-notes.md
scripts/extract_frames.py
scripts/get_video.sh
```
