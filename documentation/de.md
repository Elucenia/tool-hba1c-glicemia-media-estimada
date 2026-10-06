<!-- ELUCENIA technical documentation · hba1c-glicemia-media-estimada · de · no clinical/professional/rights approval -->

# HbA1c und geschätzter mittlerer Blutzucker (ADAG)

[Bedingungen, Quellen und Berechtigungen](https://elucenia.org/de/werkzeuge/hba1c-glicemia-media-estimada)

## Verwendung

Verwenden Sie das Werkzeug im Portal oder öffnen Sie index.html über einen lokalen HTTP-Server. Wählen Sie die Sprache, füllen Sie die Felder aus und berechnen Sie das Ergebnis.

## Eingaben und Einheiten

### HbA1c

`hba1c`

% · optional · Bereich: 3–20

### oder mittlerer Blutzucker (wenn HbA1c nicht angegeben wird)

`gme`

mg/dL · optional · Bereich: 40–600

## Fassung der Methode

ADAG/Nathan 2008: eAG mg/dL 28,7 HbA1c−46,7; mmol/L 1,59 HbA1c−2,59

## Dokumentierte Formel

Geschätzte mittlere Glukose (mg/dL) = 28,7 × HbA1c (%) − 46,7.

In mmol/L = 1,59 × HbA1c (%) − 2,59.

Umkehrung: HbA1c (%) = (mittlere Glukose + 46,7) ÷ 28,7.

## Grenzen und Population

Die ADAG-Regression von 2008 wurde über drei Monate bei Teilnehmenden mit relativ stabiler Glykämie untersucht. Kinder, Schwangere und Personen mit Erythrozytenerkrankungen wurden ausgeschlossen; Anämie, Veränderungen des Erythrozytenumsatzes und Hämoglobinopathien können die Interpretation des HbA1c beeinflussen. Die geschätzte mittlere Glukose ist keine direkte Messung, und die algebraische Umkehrung ist kein eigenständiger diagnostischer Test. Einheit und Koeffizientenvariante müssen beibehalten werden.

## Referenzen

- [Nathan DM et al. Translating the A1C assay into estimated average glucose values. Diabetes Care, 2008.](https://doi.org/10.2337/dc08-0545)

- [American Diabetes Association Professional Practice Committee. 2. Diagnosis and Classification of Diabetes: Standards of Care in Diabetes—2025. Diabetes Care, 2025.](https://doi.org/10.2337/dc25-S002)

## Technische Tests reproduzieren

Führen Sie node test.cjs im Stammverzeichnis dieses Repositorys aus, um die dokumentierten synthetischen Fälle zu wiederholen. Ursprüngliche Eingaben, erwartete Ergebnisse und Toleranzen bleiben erhalten. Technische Tests stellen keine klinische Validierung dar.

```sh
node test.cjs
```

tool.json enthält Quellen, Ausgabe und Umfang der Überprüfung. examples.json bewahrt die synthetischen Eingaben und erwarteten Ergebnisse; results.json dokumentiert die tatsächlich erhaltenen Ergebnisse.

[Eintrag und Referenzen](../tool.json) · [JavaScript-Code](../calculator.js) · [Referenzfälle](../examples.json) · [results.json](../results.json)

## Überprüfung und Nutzungsbedingungen

Eine unabhängige klinische Prüfung wurde nicht durchgeführt.

Diese Benutzeroberfläche ist eine selbst erstellte Übersetzung und keine offizielle oder zertifizierte Ausgabe. Eine unabhängige klinische Überprüfung, eine professionelle sprachliche Prüfung und eine Klärung der Rechte an den Instrumenten wurden nicht durchgeführt.

Ergebnis der Formel oder Klassifikation. Interpretation, Vorgehen und Anwendbarkeit hängen von der fachlichen Beurteilung und der ausgewählten Quelle ab.

## Lizenz und Urheberangaben

Apache-2.0 gilt nur für den ELUCENIA-Code. Die Rechte an Instrumenten, Veröffentlichungen, Übersetzungen und Daten verbleiben bei den jeweiligen Rechteinhabern. Bewahren Sie LICENSE und NOTICE auf.

ELUCENIA · Felipe Guedes · Copyright © 2026

## Dokumentierte Ergebnisse

Die folgenden Angaben bewahren die Ausgaben der Methode für synthetische Beispiele. Sie stellen keine unabhängige klinische Validierung dar.

### 1

HbA1c im Diabetesbereich (≥ 6,5 %)

| Ergebnisdetails | |
| --- | --- |
| Geschätzter mittlerer Blutzucker | 8,6 mmol/L |
| Gemeldete HbA1c | 7,0% |


### 2

HbA1c im Prädiabetes-Bereich (5,7 bis 6,4 %)

| Ergebnisdetails | |
| --- | --- |
| Geschätzter mittlerer Blutzucker | 7,0 mmol/L |
| Gemeldete HbA1c | 6,0% |


### 3

HbA1c im Prädiabetes-Bereich (5,7 bis 6,4 %)

| Ergebnisdetails | |
| --- | --- |
| Geschätzter mittlerer Blutzucker | 6,5 mmol/L |
| Gemeldete HbA1c | 5,7% |


### 4

HbA1c im Normbereich (< 5,7 %)

| Ergebnisdetails | |
| --- | --- |
| Geschätzter mittlerer Blutzucker | 5,4 mmol/L |
| Gemeldete HbA1c | 5,0% |


### 5

HbA1c im Diabetesbereich (≥ 6,5 %)

| Ergebnisdetails | |
| --- | --- |
| Geschätzter mittlerer Blutzucker | 8,6 mmol/L |
| Gemeldete mittlere Glukose | 154 mg/dL |

