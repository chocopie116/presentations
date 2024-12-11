# slides
- [公式ドキュメント](https://marpit.marp.app/markdown)
- [marp記法](https://qiita.com/takeshisakuma/items/5a61e6eac123d28602fb)


# 出力
## html出力
以下のコマンドでlocalで見れます
```sh
$ npm run server
```
またgithub pagesにhtml, PDF共に.mdに対応する形でdeployされています。

- 20241125_langchain-langgraph-study/index.md
- => https://chocopie116.github.io/presentations/20241125_langchain-langgraph-study/index.html
- => https://chocopie116.github.io/presentations/20241125_langchain-langgraph-study/index.pdf


## PDF出力
以下のコマンドでPDFを出力できます

```sh
$ npm run server
$ npm run pdf -- 20241211_ragaiagent/スライド.md -o ~/Desktop/20241211-勉強会スライド.pdf
```
