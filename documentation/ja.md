<!-- ELUCENIA technical documentation · hba1c-glicemia-media-estimada · ja · no clinical/professional/rights approval -->

# HbA1c・推定平均血糖（ADAG）

[条件・出典・許諾](https://elucenia.org/ja/tools/hba1c-glicemia-media-estimada)

## 使い方

ポータルでツールを使用するか、ローカルHTTPサーバー経由でindex.htmlを開いてください。言語を選択し、項目を入力して計算してください。

## 入力項目と単位

### HbA1c

`hba1c`

% · 任意 · 範囲: 3–20

### または平均血糖（HbA1cを入力しない場合）

`gme`

mg/dL · 任意 · 範囲: 40–600

## 方法の版

ADAG/Nathan 2008：eAG mg/dL 28.7 HbA1c−46.7；mmol/L 1.59 HbA1c−2.59

## 記載された計算式

推定平均血糖（mg/dL） = 28.7 × HbA1c (%) − 46.7.

mmol/Lで = 1.59 × HbA1c (%) − 2.59.

逆算: HbA1c (%) = (平均血糖 + 46.7) ÷ 28.7.

## 限界・対象集団

ADAG 2008の回帰式は、血糖が比較的安定した参加者を対象に3か月間研究されました。小児、妊婦、赤血球に関連する病態のある人は除外されました。貧血、赤血球の代謝回転の変化、ヘモグロビン異常症はHbA1cの解釈に影響する可能性があります。推定平均血糖は直接測定値ではなく、代数的な逆算は独立した診断検査ではありません。単位と係数の版を維持する必要があります。

## 参考文献

- [Nathan DM et al. Translating the A1C assay into estimated average glucose values. Diabetes Care, 2008.](https://doi.org/10.2337/dc08-0545)

- [American Diabetes Association Professional Practice Committee. 2. Diagnosis and Classification of Diabetes: Standards of Care in Diabetes—2025. Diabetes Care, 2025.](https://doi.org/10.2337/dc25-S002)

## 技術テストの再現

このリポジトリのルートディレクトリでnode test.cjsを実行すると、記録された合成ケースを再実行できます。元の入力、期待結果、許容誤差は保持されています。技術テストは臨床的検証を意味しません。

```sh
node test.cjs
```

tool.jsonには出典、版、確認範囲が記録されています。examples.jsonには合成入力と期待結果が保持され、results.jsonには実際に得られた結果が記録されています。

[記録・参考文献](../tool.json) · [JavaScriptコード](../calculator.js) · [参照ケース](../examples.json) · [results.json](../results.json)

## 確認状況と使用条件

独立した臨床レビューは実施されていません。

このインターフェースは独自に作成した翻訳であり、公式版や認証済みの版ではありません。独立した臨床レビュー、専門家による言語レビュー、評価尺度等の権利許諾の確認は実施されていません。

式または分類の結果です。解釈、対応、適用可能性は専門家による評価と選択した出典に依存します。

## ライセンスと帰属表示

Apache-2.0はELUCENIAのコードにのみ適用されます。評価尺度等、出版物、翻訳、データの権利は、それぞれの権利者に帰属します。LICENSEとNOTICEを保持してください。

ELUCENIA · Felipe Guedes · Copyright © 2026
