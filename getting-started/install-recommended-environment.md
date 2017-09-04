# 付録 | 推奨環境のインストール

## Git

[Git 公式サイト](https://git-scm.com/) からダウンロードします。

## Node.js

[Node.js 公式サイト](https://nodejs.org/ja/) からダウンロードします。
推奨版・最新版のどちらでも構いません。

## LaTeX

Docker image を使う方法と TeX Live でインストールする方法があります。

### Whalebrew (Docker image)

Docker 環境がある場合は、
[Whalebrew](https://github.com/bfirsh/whalebrew) を使うと導入が簡単です。

macOS / Linux の場合は、
https://github.com/bfirsh/whalebrew#install を参考に
Whalebrew をインストールします。

Whalebrew 経由で `latexmk` を導入するには、
以下のコマンドを実行します。

```bash
whalebrew install paperist/latexmk
```

Whalebrew を使う場合は、
TeX Live の導入は不要です。

### TeX Live

LaTeX のインストールには、TeX Live を使います。

- For Windows
  - [TeX Live for Windows](http://mirror.ctan.org/systems/texlive/tlnet/install-tl-windows.exe)
- For macOS
  - [MacTeX](http://tug.org/cgi-bin/mactex-download/MacTeX.pkg) (`schema-full`)
  - [BasicTeX](http://tug.org/cgi-bin/mactex-download/BasicTeX.pkg) (`scheme-small`)

Windows 版 TeX Live および MacTeX は、
デフォルトで `schema-full` がインストールされます。
通常はこれで問題ありません。
（ただし、インストールにかなり時間がかかります。）

`schema-full` 以外をインストールした場合は、
以下のコレクションが必要になります。

- `collection-basic`
- `collection-latex`
- `collection-latexrecommended`
- `collection-latexextra`
- `collection-fontsrecommended`
- `collection-langjapanese`
- `latexmk`

詳しい情報は、[TeX Live - TeX Wiki](https://texwiki.texjp.org/?TeX%20Live)を参照してください。

