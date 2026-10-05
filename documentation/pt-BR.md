<!-- ELUCENIA technical documentation · hba1c-glicemia-media-estimada · pt-BR · no clinical/professional/rights approval -->

# HbA1c e glicemia média estimada (ADAG)

[condições, fontes e permissões](https://elucenia.org/pt-br/ferramentas/hba1c-glicemia-media-estimada)

## Como usar

Use a ferramenta no portal ou abra index.html em um servidor HTTP local. Selecione o idioma, preencha os campos e calcule.

## Entradas e unidades

### HbA1c

`hba1c`

% · opcional · intervalo: 3–20

### ou glicemia média (se não informar a HbA1c)

`gme`

mg/dL · opcional · intervalo: 40–600

## Edição do método

ADAG/Nathan 2008:e AGmg/d L 28,7 Hb A 1 c−46,7; mmol/L 1,59 Hb A 1 c−2,59

## Fórmula documentada

Glicemia média estimada (mg/dL) = 28,7 × HbA1c (%) − 46,7.

Em mmol/L = 1,59 × HbA1c (%) − 2,59.

Inversa: HbA1c (%) = (glicemia média + 46,7) ÷ 28,7.

## Limites e população

A regressão ADAG 2008 foi estudada durante três meses em participantes com glicemia relativamente estável. Crianças, gestantes e pessoas com condições eritrocitárias foram excluídas; anemia, alterações do turnover eritrocitário e hemoglobinopatias podem afetar a interpretação da HbA1c. A glicemia média estimada não é uma medida direta, e a inversa algébrica não constitui teste diagnóstico independente. A unidade e a variante dos coeficientes devem ser preservadas.

## Referências

- [Nathan DM et al. Translating the A1C assay into estimated average glucose values. Diabetes Care, 2008.](https://doi.org/10.2337/dc08-0545)

- [American Diabetes Association Professional Practice Committee. 2. Diagnosis and Classification of Diabetes: Standards of Care in Diabetes—2025. Diabetes Care, 2025.](https://doi.org/10.2337/dc25-S002)

## Reproduzir os testes técnicos

Execute node test.cjs na pasta raiz deste repositório para repetir os casos sintéticos registrados. As entradas, expectativas e tolerâncias originais são preservadas. Testes técnicos não constituem validação clínica.

```sh
node test.cjs
```

tool.json contém fontes, edição e escopo de revisão. examples.json conserva as entradas e expectativas sintéticas; results.json registra os resultados obtidos.

[Ficha e referências](../tool.json) · [Código JavaScript](../calculator.js) · [Casos de referência](../examples.json) · [results.json](../results.json)

## Revisão e condições de uso

Revisão clínica independente não realizada.

Esta interface é uma tradução autoral, não uma edição oficial ou certificada. Revisão clínica independente, revisão linguística profissional e autorização de direitos de instrumentos não foram realizadas.

Resultado da fórmula ou classificação. Interpretação, conduta e aplicabilidade dependem da avaliação profissional e da fonte selecionada.

## Licença e atribuição

Apache-2.0 aplica-se somente ao código da ELUCENIA. Os instrumentos, publicações, traduções e dados mantêm os direitos dos respectivos titulares. Preserve LICENSE e NOTICE.

ELUCENIA · Felipe Guedes · Copyright © 2026
