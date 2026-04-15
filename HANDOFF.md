# Handoff Notes

本项目由用户和 `GPT/Codex` 协作整理。

## 项目目标

把用户拍摄的纸质量子化学培训资料逐页整理为一份连续的 `LaTeX` 文档，并生成 PDF。

## 强约束

- 只写资料里已有内容，不额外补课。
- 忽略页眉页脚、页码、水印、版权、网址、作者单位、手写痕迹。
- 文档应是连续讲义，不是 PPT 截图转录。
- 简单示意图可以重画；复杂图可跳过，只保留必要信息。
- 不要把对话里的解释直接塞进讲义。

## 已形成的工作习惯

- 入口文件：`main.tex`
- 主章节：
  - `chapters/01-quantum-mechanics-overview.tex`
  - `chapters/02-theoretical-foundations.tex`
- 每次编辑后使用：

```bash
latexmk -xelatex -interaction=nonstopmode -halt-on-error main.tex
```

## 当前断点

第二章已写到 `1.2 半经验方法` 标题，下一步应从这里继续。

