# 文章の設定をする

文章の設定は、
`remarkrc.yml` で変更できます。

（`remarkrc.yml` の詳細は、
[wooorm/remark]リポジトリを参照してください。）

[wooorm/remark]: https://github.com/wooorm/remark/tree/master/packages/remark-cli

`documentInfo` 内の情報が
テンプレートに反映されます。

```yaml
settings:
  latex:
    documentInfo:
      title:
        ja: 論文タイトル
      authors:
        - name:
            ja: 山田 太郎
```
