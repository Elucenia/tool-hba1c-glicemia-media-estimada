<!-- ELUCENIA technical documentation · hba1c-glicemia-media-estimada · en · no clinical/professional/rights approval -->

# HbA1c and estimated average glucose (ADAG)

[conditions, sources and permissions](https://elucenia.org/en/tools/hba1c-glicemia-media-estimada)

## How to use

Use the tool in the portal or open index.html through a local HTTP server. Select the language, complete the fields and calculate.

## Inputs and units

### HbA1c

`hba1c`

% · optional · range: 3–20

### or mean blood glucose (if HbA1c is not entered)

`gme`

mg/dL · optional · range: 40–600

## Method edition

ADAG/Nathan 2008: eAG mg/dL 28.7 HbA1c−46.7; mmol/L 1.59 HbA1c−2.59

## Documented formula

Estimated average glucose (mg/dL) = 28.7 × HbA1c (%) − 46.7.

In mmol/L = 1.59 × HbA1c (%) − 2.59.

Inverse: HbA1c (%) = (average glucose + 46.7) ÷ 28.7.

## Limits and population

The ADAG 2008 regression was studied over three months in participants with relatively stable glycemia. Children, pregnant women and people with erythrocyte conditions were excluded; anemia, altered erythrocyte turnover and hemoglobinopathies may affect interpretation of HbA1c. Estimated average glucose is not a direct measurement, and the algebraic inverse is not an independent diagnostic test. The unit and coefficient variant must be preserved.

## References

- [Nathan DM et al. Translating the A1C assay into estimated average glucose values. Diabetes Care, 2008.](https://doi.org/10.2337/dc08-0545)

- [American Diabetes Association Professional Practice Committee. 2. Diagnosis and Classification of Diabetes: Standards of Care in Diabetes—2025. Diabetes Care, 2025.](https://doi.org/10.2337/dc25-S002)

## Reproduce the technical tests

Run node test.cjs in the root directory of this repository to repeat the recorded synthetic cases. Original inputs, expectations and tolerances are preserved. Technical tests do not constitute clinical validation.

```sh
node test.cjs
```

tool.json contains sources, edition and review scope. examples.json retains synthetic inputs and expectations; results.json records the obtained results.

[Record and references](../tool.json) · [JavaScript code](../calculator.js) · [Reference cases](../examples.json) · [results.json](../results.json)

## Review and conditions of use

Independent clinical review has not been performed.

This interface is an authorial translation, not an official or certified edition. Independent clinical review, professional language review and instrument rights clearance have not been performed.

Formula or classification result. Interpretation, care and applicability depend on professional assessment and the selected source.

## License and attribution

Apache-2.0 applies only to ELUCENIA code. Rights to instruments, publications, translations and data remain with their respective holders. Preserve LICENSE and NOTICE.

ELUCENIA · Felipe Guedes · Copyright © 2026
