# 年間計画
教科書: [実教出版『高校 社会と情報』](https://amazon.jp/dp/4407202262)

<!-- workaround for bug of cutemarked -->
<script> mermaid.ganttConfig = { numberSectionStyles:2 }; </script>

## 上半期
- 4月: [セキュリティ](security/README.md) (個人情報、マルウェア)
- 5月上旬: [知的財産](intellectualproperty/README.md) (著作権)
- 5月中旬: [情報とは](information/README.md) (情報の定義・特徴、情報の分類)
- 6月上旬-中旬: [コミュニケーション](communication/README.md) (コミュニケーション、メディア)
- 6月下旬: [デザイン](design/README.md)
- 7月-11月上旬: [メディア・リテラシー](medialiteracy/README.md) (レポート、プレゼンテーション)

```mermaid
gantt
	title 授業計画(上半期)
	dateFormat YYYY-MM-DD

section セキュリティ
	個人情報			:s1, 2016-04-27, 1w
	マルウェア			:s2, after s1, 1w
section 知的財産
	知的財産			:l1, after s2, 1w
	著作権			:l2, after l1, 1w
section 情報
	情報の定義・特徴	:i1, after l2, 1w
	情報の分類			:i2, after i1, 1w
section コミュニケーション
	コミュニケーション		:c1, after i2, 1w
	メディア			:c2, after c1, 1w
section デザイン
	デザイン			:d1, after c2, 1w
section メディア・リテラシー
	メディア・リテラシー		:m1, after d1, 1w
	レポート			:m2, after m1, 1w
	アウトライン作成		:m3, after m2, 1w
```

## 下半期
- 7月-11月上旬: [メディア・リテラシー](medialiteracy/README.md) (レポート、プレゼンテーション)
- 12月-2月: [プログラミング](programming/README.md) (Scratch、Excel、VBA、Scratch)

```mermaid
gantt
	title 授業計画(下半期)
	dateFormat YYYY-MM-DD

section メディア・リテラシー
	相互レビュー		:m4, 2016-09-10, 1w
section プレゼンテーション
	プレゼンテーション		:p1, after m4, 1w
	アウトライン作成		:p2, after p1, 1w
	スライド作成			:p3, after p2, 2w
	リハーサル			:p4, after p3, 1w
	プレゼン実施		:p5, after p4, 2w
section プログラミング
	Scratch実習		:c1, after p5, 1w
	表計算			:c2, after c1, 2w
	VBA				:c3, 2017-01-01, 2w
	シミュレーション		:c4, after c3, 1w
	自由制作			:c5, after c4, 2w
```

## 単元の関連性・位置づけ
```mermaid
graph TB
	情報-->コミュニケーション
	コミュニケーション-->メディアリテラシー
	メディアリテラシー-->プレゼンテーション
	コミュニケーション-->デザイン
	情報-->プログラミング
	コミュニケーション-->プログラミング
	デザイン-->プレゼンテーション
	情報-->セキュリティ
	情報-->知的財産
```
