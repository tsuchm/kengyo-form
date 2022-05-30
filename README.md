# 使い方

1. 兼業等従事届の Excel 様式ファイルを適宜に編集して，定数部分を埋める．
2. 兼業等従事届の Excel 様式ファイルを PDF 形式に export する．
3. PDF の余白部分を削除する．

```
pdfcrop kengyo-form.pdf wallpaper.pdf
```

4. PDF ファイルを EPS 形式に変換する．

```
pdftops -eps wallpaper.pdf wallpaper.eps
```

5. sample.tex を処理して，適切な兼業等従事届が得られることを確認する．

```
latexmk sample.tex
```
