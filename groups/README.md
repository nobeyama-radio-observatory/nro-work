# 業務グループごとの業務一覧

業務グループごとに `<業務グループ>.yaml` を置きます。項目の定義はハブの [work/README.md](https://github.com/nobeyama-radio-observatory/nro-context/blob/main/work/README.md) です。

書き方の例（架空の業務。実際のファイルではありません）：

```yaml
group: 例のグループ
as_of: 2026-12
source: worklog の月次マージ（2026-12）
tasks:
  - tag: "#例のグループ/例の業務"
    name: 例の装置の定期保守
    category: 装置
    frequency: 年1回
    timing: 夏
    docs: あり（所内）
    people: 2
    judges: 1
    learners: 1
    concentration: 中
    status: 現行
    assets: [nro45m]
```
