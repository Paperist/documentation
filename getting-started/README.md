# はじめに

## 推奨環境

Paperist では、以下のソフトウェアが必要です。

（これらのインストール方法は、[付録 | 推奨環境のインストール](./install-recommended-environment.md)を参照してください。）

- [Git](https://git-scm.com/)
- [Node.js](https://nodejs.org/ja/)
  - **バージョン 6.11.2 以上が必要です**
- [LaTeX](https://www.tug.org/texlive/)
  - TeXLive 2017 以上を推奨します
  - **以下のコレクションが必要です**
    - `collection-basic`
    - `collection-latex`
    - `collection-latexrecommended`
    - `collection-fontsrecommended`
    - `collection-langjapanese`
    - `latexmk`
  - 以下のコレクションを推奨します
    - `collection-latexextra`

## インストール

スターターキットをダウンロードして、
必要なソフトウェアをインストールします。

コマンドプロンプト もしくは ターミナルから、
以下のコマンドを実行してください。

```bash
git clone --depth 1 https://github.com/Paperist/starter-kit.git
cd ./starter-kit
npm install
```

## 試してみる

スターターキットには、
すでにサンプルの文章が入っています。

サンプルの文章を PDF にするには、
以下のコマンドを実行してください。

```bash
npm run build
```

`main.pdf` が生成されれば、
インストールは無事に完了しています。

