<!-- ELUCENIA technical documentation · hba1c-glicemia-media-estimada · it · no clinical/professional/rights approval -->

# HbA1c e glicemia media stimata (ADAG)

[condizioni, fonti e autorizzazioni](https://elucenia.org/it/strumenti/hba1c-glicemia-media-estimada)

## Come usare

Usi lo strumento nel portale oppure apra index.html tramite un server HTTP locale. Selezioni la lingua, compili i campi ed esegua il calcolo.

## Dati di ingresso e unità

### HbA1c

`hba1c`

% · facoltativo · intervallo: 3–20

### o glicemia media (se non viene inserita HbA1c)

`gme`

mg/dL · facoltativo · intervallo: 40–600

## Edizione del metodo

ADAG/Nathan 2008: eAG mg/dL 28,7 HbA1c−46,7; mmol/L 1,59 HbA1c−2,59

## Formula documentata

Glicemia media stimata (mg/dL) = 28,7 × HbA1c (%) − 46,7.

In mmol/L = 1,59 × HbA1c (%) − 2,59.

Inversa: HbA1c (%) = (glicemia media + 46,7) ÷ 28,7.

## Limiti e popolazione

La regressione ADAG 2008 è stata studiata per tre mesi in partecipanti con glicemia relativamente stabile. Sono stati esclusi bambini, donne in gravidanza e persone con condizioni eritrocitarie; anemia, alterazioni del ricambio eritrocitario ed emoglobinopatie possono influenzare l’interpretazione dell’HbA1c. La glicemia media stimata non è una misurazione diretta e l’inversa algebrica non costituisce un test diagnostico indipendente. Devono essere mantenute l’unità e la variante dei coefficienti.

## Riferimenti

- [Nathan DM et al. Translating the A1C assay into estimated average glucose values. Diabetes Care, 2008.](https://doi.org/10.2337/dc08-0545)

- [American Diabetes Association Professional Practice Committee. 2. Diagnosis and Classification of Diabetes: Standards of Care in Diabetes—2025. Diabetes Care, 2025.](https://doi.org/10.2337/dc25-S002)

## Riprodurre i test tecnici

Esegua node test.cjs nella cartella principale di questo repository per ripetere i casi sintetici registrati. Gli input, i risultati attesi e le tolleranze originali sono conservati. I test tecnici non costituiscono validazione clinica.

```sh
node test.cjs
```

tool.json contiene le fonti, l’edizione e l’ambito della revisione. examples.json conserva gli input e i risultati attesi dei casi sintetici; results.json registra i risultati ottenuti.

[Scheda e riferimenti](../tool.json) · [Codice JavaScript](../calculator.js) · [Casi di riferimento](../examples.json) · [results.json](../results.json)

## Revisione e condizioni d’uso

Non è stata effettuata una revisione clinica indipendente.

Questa interfaccia è una traduzione realizzata dagli autori, non un’edizione ufficiale o certificata. Non sono state eseguite la revisione clinica indipendente, la revisione linguistica professionale né la verifica delle autorizzazioni relative ai diritti sugli strumenti.

Risultato della formula o classificazione. Interpretazione, condotta e applicabilità dipendono dalla valutazione professionale e dalla fonte selezionata.

## Licenza e attribuzione

Apache-2.0 si applica solo al codice di ELUCENIA. I diritti su strumenti, pubblicazioni, traduzioni e dati restano ai rispettivi titolari. Conservi LICENSE e NOTICE.

ELUCENIA · Felipe Guedes · Copyright © 2026
