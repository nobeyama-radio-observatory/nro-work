# nro-work

国立天文台 野辺山宇宙電波観測所の**業務一覧**です。文脈基盤のハブ [nro-context](https://github.com/nobeyama-radio-observatory/nro-context) から参照されます（ハブの判断記録 [0008](https://github.com/nobeyama-radio-observatory/nro-context/blob/main/decisions/0008-業務一覧を月次マージから集計して公開する.md)）。

- **材料：** 所内の worklog（非公開）の月次マージ。業務単位に集計し、個人名と、誰がどの判断レベルかは書いていません。人数だけを書いています。
- **項目の定義と、書き出しの前の確認の項目の正本：** ハブの [work/README.md](https://github.com/nobeyama-radio-observatory/nro-context/blob/main/work/README.md)
- **作り方：** 月次マージの担当が、worklog のあるマシンで、worklog のスキルの月次マージの手順7「公開用の書き出し」に沿って作り、そのマシンからプルリクエストを出します。非公開の材料は、このリポジトリに置きません。

## 中身

| 場所 | 中身 |
|---|---|
| `groups/<業務グループ>.yaml` | 業務グループごとの業務一覧。業務グループは worklog のタグ辞書の第1階層 |

最初の書き出しは 2026-11 の月次マージから作りました。

## 読み方

- `judges` は単独で判断できる人の数（判断レベル L4 以上）。1以下の業務は、担い手が抜けると止まりうる業務です。
- `learners` は経験を積んでいる人の数（L2〜L3）。0 の業務は、後継が育っていません。
- `concentration`（属人度）が「高」で、`docs` が「なし」の業務は、引き継ぎで抜けやすい業務です。
- 手間の量は、当面は `frequency`（頻度）と `timing`（時期）で表しています（作業時間は記録していません）。

## 進め方

進め方の決まりの正本は、ハブの [CONTRIBUTING.md](https://github.com/nobeyama-radio-observatory/nro-context/blob/main/CONTRIBUTING.md) です。

担当：月次マージの担当（所長）

## 利用許諾

- コード：BSD 3-Clause License（[LICENSE](LICENSE)）
- 文書とデータ：クリエイティブ・コモンズ 表示 4.0 国際（CC BY 4.0、[LICENSE-docs](LICENSE-docs)）
