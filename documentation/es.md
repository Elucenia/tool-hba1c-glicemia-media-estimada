<!-- ELUCENIA technical documentation · hba1c-glicemia-media-estimada · es · no clinical/professional/rights approval -->

# HbA1c y glucemia media estimada (ADAG)

[condiciones, fuentes y permisos](https://elucenia.org/es/herramientas/hba1c-glicemia-media-estimada)

## Cómo usar

Utilice la herramienta en el portal o abra index.html mediante un servidor HTTP local. Seleccione el idioma, complete los campos y calcule.

## Entradas y unidades

### HbA1c

`hba1c`

% · opcional · intervalo: 3–20

### o glucemia media (si no introduce HbA1c)

`gme`

mg/dL · opcional · intervalo: 40–600

## Edición del método

ADAG/Nathan 2008: eAG mg/dL 28,7 HbA1c−46,7; mmol/L 1,59 HbA1c−2,59

## Fórmula documentada

Glucemia media estimada (mg/dL) = 28,7 × HbA1c (%) − 46,7.

En mmol/L = 1,59 × HbA1c (%) − 2,59.

Inversa: HbA1c (%) = (glucemia media + 46,7) ÷ 28,7.

## Límites y población

La regresión ADAG 2008 se estudió durante tres meses en participantes con glucemia relativamente estable. Se excluyeron niños, embarazadas y personas con alteraciones eritrocitarias; la anemia, los cambios en el recambio eritrocitario y las hemoglobinopatías pueden afectar la interpretación de la HbA1c. La glucemia media estimada no es una medición directa, y la inversa algebraica no constituye una prueba diagnóstica independiente. Deben conservarse la unidad y la variante de los coeficientes.

## Referencias

- [Nathan DM et al. Translating the A1C assay into estimated average glucose values. Diabetes Care, 2008.](https://doi.org/10.2337/dc08-0545)

- [American Diabetes Association Professional Practice Committee. 2. Diagnosis and Classification of Diabetes: Standards of Care in Diabetes—2025. Diabetes Care, 2025.](https://doi.org/10.2337/dc25-S002)

## Reproducir las pruebas técnicas

Ejecute node test.cjs en el directorio raíz de este repositorio para repetir los casos sintéticos registrados. Se conservan las entradas, los resultados esperados y las tolerancias originales. Las pruebas técnicas no constituyen validación clínica.

```sh
node test.cjs
```

tool.json contiene las fuentes, la edición y el alcance de la revisión. examples.json conserva las entradas y los resultados esperados de los casos sintéticos; results.json registra los resultados obtenidos.

[Ficha y referencias](../tool.json) · [Código JavaScript](../calculator.js) · [Casos de referencia](../examples.json) · [results.json](../results.json)

## Revisión y condiciones de uso

No se ha realizado una revisión clínica independiente.

Esta interfaz es una traducción de elaboración propia, no una edición oficial o certificada. No se han realizado la revisión clínica independiente, la revisión lingüística profesional ni la autorización de derechos de los instrumentos.

Resultado de la fórmula o clasificación. La interpretación, la conducta y la aplicabilidad dependen de la evaluación profesional y de la fuente seleccionada.

## Licencia y atribución

Apache-2.0 se aplica únicamente al código de ELUCENIA. Los derechos de los instrumentos, publicaciones, traducciones y datos permanecen en manos de sus respectivos titulares. Conserve LICENSE y NOTICE.

ELUCENIA · Felipe Guedes · Copyright © 2026
