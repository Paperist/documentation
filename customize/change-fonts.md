# フォントを変える

`paperist.config.yml` の設定を変えることで、任意のフォントに変更できます。

これらは [PXchfon] という LaTeX パッケージによって実現されています。

[PXchfon]: https://github.com/zr-tex8r/PXchfon

必要なフォントファイルを `fonts/` に置くか、
対応するテンプレートをインストールすることで利用できます。

Paperist 公式で用意しているものは次のとおりです。

- `ipaex`
  - 標準で利用できます
- `sourcehan-otc`
  - **TeX Live 2017 以降**が必要です
  - [Paperist/template-sourcehan-fonts] テンプレートが必要です
    - `paperist template install paperist/template-sourcehan-fonts`

```yaml
documentInfo:
  # default
  fontpreset: ipaex
  # with Paperist/template-sourcehan-fonts
  fontpreset: sourcehan-otc
```

[Paperist/template-sourcehan-fonts]: https://github.com/Paperist/template-sourcehan-fonts
