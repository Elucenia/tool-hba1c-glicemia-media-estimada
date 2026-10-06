<!-- ELUCENIA technical documentation · hba1c-glicemia-media-estimada · fr · no clinical/professional/rights approval -->

# HbA1c et glycémie moyenne estimée (ADAG)

[conditions, sources et autorisations](https://elucenia.org/fr/outils/hba1c-glicemia-media-estimada)

## Mode d’emploi

Utilisez l’outil sur le portail ou ouvrez index.html via un serveur HTTP local. Sélectionnez la langue, remplissez les champs et lancez le calcul.

## Données d’entrée et unités

### HbA1c

`hba1c`

% · facultatif · intervalle: 3–20

### ou glycémie moyenne (si HbA1c non renseignée)

`gme`

mg/dL · facultatif · intervalle: 40–600

## Édition de la méthode

ADAG/Nathan 2008 : eAG mg/dL 28,7 HbA1c−46,7 ; mmol/L 1,59 HbA1c−2,59

## Formule documentée

Glycémie moyenne estimée (mg/dL) = 28,7 × HbA1c (%) − 46,7.

En mmol/L = 1,59 × HbA1c (%) − 2,59.

Inverse: HbA1c (%) = (glycémie moyenne + 46,7) ÷ 28,7.

## Limites et population

La régression ADAG 2008 a été étudiée pendant trois mois chez des participants ayant une glycémie relativement stable. Les enfants, les femmes enceintes et les personnes présentant des anomalies érythrocytaires ont été exclus ; l’anémie, les modifications du renouvellement érythrocytaire et les hémoglobinopathies peuvent affecter l’interprétation de l’HbA1c. La glycémie moyenne estimée n’est pas une mesure directe, et l’inverse algébrique ne constitue pas un test diagnostique indépendant. L’unité et la variante des coefficients doivent être conservées.

## Références

- [Nathan DM et al. Translating the A1C assay into estimated average glucose values. Diabetes Care, 2008.](https://doi.org/10.2337/dc08-0545)

- [American Diabetes Association Professional Practice Committee. 2. Diagnosis and Classification of Diabetes: Standards of Care in Diabetes—2025. Diabetes Care, 2025.](https://doi.org/10.2337/dc25-S002)

## Reproduire les tests techniques

Exécutez node test.cjs dans le répertoire racine de ce dépôt pour reproduire les cas synthétiques enregistrés. Les données d’entrée, les résultats attendus et les tolérances d’origine sont conservés. Les tests techniques ne constituent pas une validation clinique.

```sh
node test.cjs
```

tool.json contient les sources, l’édition et le périmètre de la revue. examples.json conserve les données d’entrée et les résultats attendus des cas synthétiques ; results.json consigne les résultats obtenus.

[Fiche et références](../tool.json) · [Code JavaScript](../calculator.js) · [Cas de référence](../examples.json) · [results.json](../results.json)

## Revue et conditions d’utilisation

Aucune révision clinique indépendante n’a été effectuée.

Cette interface est une traduction réalisée par nos soins, et non une édition officielle ou certifiée. La revue clinique indépendante, la révision linguistique professionnelle et l’autorisation des droits sur les instruments n’ont pas été réalisées.

Résultat de la formule ou de la classification. L’interprétation, la conduite et l’applicabilité dépendent de l’évaluation professionnelle et de la source sélectionnée.

## Licence et attribution

Apache-2.0 s’applique uniquement au code d’ELUCENIA. Les droits sur les instruments, publications, traductions et données restent ceux de leurs titulaires respectifs. Conservez LICENSE et NOTICE.

ELUCENIA · Felipe Guedes · Copyright © 2026

## Résultats documentés

Les informations ci-dessous conservent les sorties de la méthode pour des exemples synthétiques. Elles ne constituent pas une validation clinique indépendante.

### 1

HbA1c dans l’intervalle du diabète (≥ 6,5 %)

| Détails du résultat | |
| --- | --- |
| Glycémie moyenne estimée | 8,6 mmol/L |
| HbA1c rapportée | 7,0% |


### 2

HbA1c dans l’intervalle de prédiabète (5,7 à 6,4 %)

| Détails du résultat | |
| --- | --- |
| Glycémie moyenne estimée | 7,0 mmol/L |
| HbA1c rapportée | 6,0% |


### 3

HbA1c dans l’intervalle de prédiabète (5,7 à 6,4 %)

| Détails du résultat | |
| --- | --- |
| Glycémie moyenne estimée | 6,5 mmol/L |
| HbA1c rapportée | 5,7% |


### 4

HbA1c dans l’intervalle normal (< 5,7 %)

| Détails du résultat | |
| --- | --- |
| Glycémie moyenne estimée | 5,4 mmol/L |
| HbA1c rapportée | 5,0% |


### 5

HbA1c dans l’intervalle du diabète (≥ 6,5 %)

| Détails du résultat | |
| --- | --- |
| Glycémie moyenne estimée | 8,6 mmol/L |
| Glycémie moyenne rapportée | 154 mg/dL |

