# 計算理論 課題1a 解答・解説スライド

このリポジトリは「計算理論」の課題1aの解答・解説スライドを作成・管理するためのものです。

## 使い方

1. 各問題ごとにスライド（beamer形式のtexファイル）を作成します。
2. メインの `main.tex` から `\input{}` コマンドで各スライドファイルを挿入します。
3. `lualatex main.tex` で全体のスライドPDFを一括生成できます。

### 例

```tex
% main.tex の例
\documentclass[aspectratio=169]{beamer}
\usepackage{luatexja}
\usepackage{luatexja-fontspec}
\setmainjfont{IPAexGothic}
\usetheme[block=fill]{metropolis}

	itle{1a 解答}
\author{}
\date{}

\begin{document}

\input{../question2-1-4-slide.tex} % スライドファイルを挿入

\end{document}
```

---
スライドファイルを追加・修正したら `lualatex main.tex` でPDFを再生成してください。