# quantum_chemistry_notes

这是一份根据纸质量子化学培训资料逐页整理得到的 `LaTeX` 讲义工程，由用户提供拍摄图片，`GPT/Codex` 协助转写、排版、补图与编译。

当前产物：

- 源文件入口：`main.tex`
- 章节文件：`chapters/01-quantum-mechanics-overview.tex`
- 章节文件：`chapters/02-theoretical-foundations.tex`
- 当前 PDF：`main.pdf`

编译方式：

```bash
latexmk -xelatex -interaction=nonstopmode -halt-on-error main.tex
```

在 macOS 上继续工作时，建议先安装支持 `xelatex` 的 TeX 发行版，然后直接在本目录执行上面的命令。

## 整理原则

- 只整理纸质资料里出现的教学内容，不额外补充讲义外的新知识。
- 忽略页眉、页脚、页码、水印、版权信息、拍照阴影和手写标记。
- 不按 PPT 页一页页复刻，而是整理成连续、可读的讲义式文档。
- 可以为可读性调整排版和语句顺序，但不应改变原意。
- 重要公式可适当紧凑排版，必要时用黑框突出。
- 图片策略：
  - 简单图尽量用 `TikZ` 或 `LaTeX` 重画。
  - 复杂图不强行复现，优先保留其承载的文字结论。
- 用户在对话中单独提出的解释性说明，不自动写入讲义，除非用户明确要求。

## 当前进度

- 第一章“量子力学概要”已整理较完整。
- 第二章“量子化学的理论基础”已整理到：
  - Born-Oppenheimer 近似
  - 电子相关、交换相关、库仑相关
  - Hartree-Fock 方法
  - SCF 迭代流程
  - `1.2 半经验方法` 标题已起出，正文尚待继续

## 给下一台机器上的 Codex

- 继续新增内容时，优先编辑 `chapters/02-theoretical-foundations.tex`。
- 保持中文连续讲义风格，不要退回到逐页 PPT 式排版。
- 如果用户继续发新照片，先提取文字主干，再判断是否需要作图。
- 本工程目前已经能稳定编译，继续修改后重新运行 `latexmk -xelatex ...` 即可。

