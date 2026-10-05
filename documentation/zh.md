<!-- ELUCENIA technical documentation · hba1c-glicemia-media-estimada · zh · no clinical/professional/rights approval -->

# HbA1c 与估算平均血糖（ADAG）

[条件、来源与许可](https://elucenia.org/zh/tools/hba1c-glicemia-media-estimada)

## 使用方法

在门户中使用工具，或通过本地 HTTP 服务器打开 index.html。选择语言，填写各字段，然后计算。

## 输入与单位

### HbA1c

`hba1c`

% · 选填 · 范围: 3–20

### 或平均血糖（未输入 HbA1c 时）

`gme`

mg/dL · 选填 · 范围: 40–600

## 方法版本

ADAG/Nathan 2008：eAG mg/dL 28.7 HbA1c−46.7；mmol/L 1.59 HbA1c−2.59

## 已记录的公式

估算平均血糖（mg/dL） = 28.7 × HbA1c (%) − 46.7.

mmol/L单位 = 1.59 × HbA1c (%) − 2.59.

逆算: HbA1c (%) = (平均血糖 + 46.7) ÷ 28.7.

## 限制与适用人群

ADAG 2008回归模型在血糖相对稳定的参与者中研究了三个月。研究排除了儿童、孕妇和存在红细胞相关状况的人；贫血、红细胞更新速度改变和血红蛋白病可能影响HbA1c的解读。估算平均血糖并非直接测量，其代数逆运算也不是独立的诊断试验。必须保持单位及所用系数版本一致。

## 参考文献

- [Nathan DM et al. Translating the A1C assay into estimated average glucose values. Diabetes Care, 2008.](https://doi.org/10.2337/dc08-0545)

- [American Diabetes Association Professional Practice Committee. 2. Diagnosis and Classification of Diabetes: Standards of Care in Diabetes—2025. Diabetes Care, 2025.](https://doi.org/10.2337/dc25-S002)

## 复现技术测试

在此仓库的根目录中运行 node test.cjs，以重复已记录的合成案例。原始输入、预期结果和容差保持不变。技术测试不构成临床验证。

```sh
node test.cjs
```

tool.json 包含来源、版本和审查范围。examples.json 保留合成输入与预期结果；results.json 记录实际得到的结果。

[记录与参考文献](../tool.json) · [JavaScript代码](../calculator.js) · [参考案例](../examples.json) · [results.json](../results.json)

## 审查与使用条件

尚未开展独立临床审查。

此界面为自主编写的翻译，并非官方或认证版本。尚未完成独立临床审查、专业语言审查或工具权利授权。

公式或分类结果。解释、处理及适用性须结合专业评估和所选来源。

## 许可与署名

Apache-2.0 仅适用于 ELUCENIA 代码。工具、出版物、翻译和数据的权利仍归各自权利人所有。请保留 LICENSE 和 NOTICE。

ELUCENIA · Felipe Guedes · Copyright © 2026
