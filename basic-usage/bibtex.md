# BibTex で参考文献を書く

Paperist では、
参考文献の記述として BibTeX を利用しています。

BibTeX では、`bibs/main.bib`ファイルに文献情報を書きます。

```bib
@inproceedings{bibtex-id,
  title = {サンプル引用論文},
  author = {山田太郎 and 鈴木花子},
  booktitle = {第99回コンピュータビジョン研究会予稿集},
  year = {2017},
  pages = {11--25}
}
```

引用するときは、
本文中で BibTeX の ID を記述します。

```md
山田らによって報告されている[@bibtex-id]．
```

論文を公開しているサイトや Google Scholar には、
BibTeX を表示するリンクがある場合がほとんどです。

また、Mendeley や JabRef のような文献管理ツールを使うと、
BibTeX ファイルを作成することができます。

Paperist では、
生成された BibTeX ファイルから
記述をコピーして使うことを推奨しています。

## Tips

### 日本人の姓名が逆に表示されてしまう

日本人名の姓名の間にスペースやカンマを入れてしまうと、
`名, 姓` と解釈されてしまいます。
逆順で入力するか、スペースをなくしてみてください。

### 英字が省略される

省略せずにそのままの状態で表示したい場合は、
その部分をさらに `{` `}` で囲んでください。

```bib
% John Smith をそのまま表示する
@misc{bibtex-id,
  title = {サンプル引用論文},
  author = {{John Smith} and 鈴木花子},
}
```

### URL を折り返す

URL は `\url{}` で囲うことを推奨しています。

```bib
@misc{example,
  title = {Example Domain},
  howpublished = {\url{http://example.com/}},
  note = {(Accessed on 09/07/2017)}
}
```
