# はじめに

## 推奨環境

Paperist では、以下のソフトウェアが必要です。

（これらのインストール方法は、[付録 | 推奨環境のインストール](../appendix/install-recommended-environment.md)を参照してください。）

- [Git](https://git-scm.com/)
- [Node.js](https://nodejs.org/ja/)
  - **バージョン 7.6.0 以上が必要です**
- [LaTeX](https://www.tug.org/texlive/)
  - TeXLive 2017 以上を推奨します
  - **以下のコレクションが必要です**
    - `collection-basic`
    - `collection-latex`
    - `collection-latexrecommended`
    - `collection-latexextra`
    - `collection-fontsrecommended`
    - `collection-langjapanese`
    - `latexmk`

## インストール

コマンドプロンプト もしくは ターミナルから、
以下のコマンドを実行してください。

```bash
npm install --global @paperist/cli
```

## 試してみる

まずは、執筆フォルダを作りましょう。

```bash
paperist init ./new-paper
cd ./new-paper
```

執筆フォルダには、
すでにサンプルの文章が入っています。

サンプルの文章を PDF にするには、
以下のコマンドを実行してください。

```bash
paperist build
```

`build.pdf` が生成されれば、
インストールは無事に完了しています。
