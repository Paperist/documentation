# 文章を書く

文章データは `src` フォルダに入っています。
メインとなるファイルは、
`index.md` になります。

文章は **Markdown 記法**で記述します。
Markdown 記法については、
http://commonmark.org/help/ を参照してください。

ここでは、
Paperist 独自の仕様について説明します。
詳細については、
https://github.com/Paperist/remark-latex#syntax を参照してください。

## Table caption

Table caption 記法で、
表にキャプションをつけることができます。

```markdown
| left | center | right |
| :--- | :----: | ----: |
| <--  |  >--<  |   --> |

Table: キャプション
```

## Label

Label 記法を使うと、
文章中で CrossReference 記法で参照することができます。

Label 記法が使えるシンタックスは、
Headings / Image / Table / Math です。

各シンタックスと記法の対応は以下のとおりです。

|     Headings     |      Image       |      Table       |      Math       |
| :--------------: | :--------------: | :--------------: | :-------------: |
| `{#sec:<label>}` | `{#fig:<label>}` | `{#tbl:<label>}` | `{#eq:<label>}` |

```markdown
# はじめに {#sec:first}

![キャプション](../assets/figure.png) {#fig:image}

| left | center | right |
| :--- | :----: | ----: |
| <--  |  >--<  |   --> |

Table: キャプション {#tbl:table}
```

### Image config

Image への Label 記法では、
画像の設定も記述できます。

（LaTeX の `\includegraphics` への設定になります。）

設定中の `\` はエスケープシーケンスとなります。
バックスラッシュを入力するには `\\` と書きます。

```markdown
![キャプション](../assets/figure.png){#fig:image width=0.9\\linewidth,height=0.25\\paperheight}
```

## CrossReference

### Section / Figure etc.

ラベルを指定することで、
図や章節を参照することができます。

```markdown
図[@fig:image]は，
[@sec:first]章において重要なシステム概略図である．
```

記法は、`[@<type>:<label>]`のようになります。

### Cites

文献情報のラベルを指定することで、
文献番号を挿入することができます。

```markdown
宮代らによって，
これらの効果は薄いという報告がなされている[@miyashiro2000]．
```

記法は、`[@<bibtex-label>]`のようになります。
複数指定する場合は、`;`で区切ります。

```markdown
このような事象については，
多くの報告がなされている[@hoge2015;@fuga2000]．
```
