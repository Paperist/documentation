# テンプレートをインストールする

テンプレートをインストールすることで、
出力される PDF のデザインスタイルを変更できます。

```bash
paperist template install Paperist/template-example-japanese
```

`--with-example` or `-w` をつけることで、
サンプルをインストールできます（**サンプルで上書きすると元には戻せません**）。

## Paperist 提供のテンプレート

テンプレートは更新日時などをみて、
**現行のテンプレートと互換性があるか確認してから利用してください**。

- [Paperist/template-example-japanese]
  - サンプル文章の日本語版です
  - `paperist template install Paperist/template-example-japanese`
- [Paperist/template-sourcehan-fonts]
  - 本文のフォントを [源ノ角ゴシック] / [源ノ明朝] にします
  - `paperist template install Paperist/template-sourcehan-fonts`
- [Paperist/template-ipsj-techreport]
  - [情報処理学会]の研究報告用のテンプレートです
  - 情報処理学会主催 [インタラクション]にも対応しています
  - `paperist template install Paperist/template-ipsj-techreport`
- [Paperist/template-wiss]
  - [WISS]のテンプレートです
  - `paperist template install Paperist/template-wiss`

[源ノ角ゴシック]: https://typekit.com/fonts/source-han-sans-japanese
[源ノ明朝]: https://typekit.com/fonts/source-han-serif-japanese
[情報処理学会]: http://www.ipsj.or.jp/journal/submit/style.html
[インタラクション]: http://www.interaction-ipsj.org
[WISS]: http://www.wiss.org/

[Paperist/template-example-japanese]: https://github.com/Paperist/template-example-japanese
[Paperist/template-ipsj-techreport]: https://github.com/Paperist/template-ipsj-techreport
[Paperist/template-sourcehan-fonts]: https://github.com/Paperist/template-sourcehan-fonts
[Paperist/template-wiss]: https://github.com/Paperist/template-wiss
