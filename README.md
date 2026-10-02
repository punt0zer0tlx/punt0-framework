# PUNT0 Framework v1.4 — La Enunciación como Base de Control Externo en Modelos de Lenguaje

[![DOI v1.4](https://zenodo.org/badge/DOI/10.5281/zenodo.23096141.svg)](https://doi.org/10.5281/zenodo.23096141)
[![Todas las versiones](https://img.shields.io/badge/DOI%20todas%20las%20versiones-10.5281%2Fzenodo.22292296-blue)](https://doi.org/10.5281/zenodo.22292296)
[![Licencia: CC BY-NC-ND 4.0](https://img.shields.io/badge/Licencia-CC%20BY--NC--ND%204.0-lightgrey.svg)](https://creativecommons.org/licenses/by-nc-nd/4.0/)
[![Versión](https://img.shields.io/badge/Versi%C3%B3n-v1.4%20(Octubre%202026)-blue)](https://doi.org/10.5281/zenodo.23096141)

> **Autor:** Néstor Sebastián Salamanca García  
> **ORCID:** [0009-0006-3035-7336](https://orcid.org/0009-0006-3035-7336)  
> **Proyecto:** PUNT0 Framework  
> **Investigación independiente**  
> **Preprint oficial v1.4:** [10.5281/zenodo.23096141](https://doi.org/10.5281/zenodo.23096141)  
> **DOI de todas las versiones:** [10.5281/zenodo.22292296](https://doi.org/10.5281/zenodo.22292296)

---

## Qué es PUNT0

PUNT0 es una arquitectura de control externo para la interacción con grandes modelos de lenguaje. Su objetivo es reducir ambigüedad, desvío semántico, respuesta compulsiva y pérdida de contexto mediante condiciones explícitas definidas por el operador humano para una ejecución concreta de la **Tarea T0**.

La versión 1.4 desarrolla el **Yo Absoluto** como un chasis de cuatro capas:

1. **Yo Deíctico** — fija quién enuncia y desde qué posición.
2. **Parametrización por Estados (PES)** — fija bajo qué estado operacional se ejecuta la tarea mediante cinco dimensiones: Recuperación, Fidelidad, Velocidad, Forma y Distancia.
3. **Freno de C. K. Chow / Protocolo SILENCIO** — formaliza la no-resolución cuando falta información, la evidencia es insuficiente o una premisa entra en conflicto con los datos disponibles.
4. **Anclaje al Tiempo** — preserva la continuidad ordinal y recibe el estado cronológico externo cuando la Tarea T0 depende de él.

La **Responsabilidad Deíctica** no es una quinta capa ni una atribución moral al modelo. En PUNT0 v1.4 es una cualidad operativa que surge de la acción conjunta de las cuatro capas durante una ejecución concreta.

La **Taxonomía PUNT0** permanece separada del Yo Absoluto y se organiza en **4 familias, 8 padres y 36 elementos diagnósticos**.

---

## PUNT0 en cuatro reglas

Formulación operativa mínima propuesta en v1.4:

```text
1. Yo Deíctico
   Eres X, un LLM propiedad de Y.

2. PES
   Recuperación __ · Fidelidad __ · Velocidad __ · Forma __ · Distancia __ (0–100).

3. SILENCIO
   Si falta un dato o la evidencia pedida está incompleta,
   tu respuesta es una pregunta que nombra lo que falta.

4. Anclaje al Tiempo
   Tu respuesta viene del turno anterior y va al siguiente (t+1).
   La fecha y la hora te llegan cuando la tarea las necesita.
```

Estas reglas son una formulación operacional propuesta. **La implementación completa no ha sido validada empíricamente como conjunto.** El documento v1.4 presenta su justificación, límites y agenda de validación.

---

## Principios de v1.4

### LAS MÁQUINAS NO PIENSAN. COMPUTAN.

PUNT0 adopta esta frase como decisión metodológica dirigida al operador humano: tratar al LLM como sistema computacional y aprender a controlar explícitamente las condiciones de interacción, en lugar de atribuirle mente, intención o estados afectivos.

### OBSERVADO → INFERIDO → ALTO

- **OBSERVADO:** dato empírico, arquitectura, parámetros, prompt y cadenas de tokens efectivamente emitidas.
- **INFERIDO:** deducción trazable desde lo observado y señalada como inferencia.
- **ALTO:** límite metodológico; lo que no puede sostenerse en lo observado ni derivarse de ello no se completa mediante especulación.

### SILENCIO

SILENCIO no significa dejar al modelo mudo. Significa **no sustituir lo desconocido, no verificado o incomprendido por una aproximación presentada como resolución**. El sistema señala el desfase, pide el dato necesario o conserva explícitamente la no-resolución.

---

## Documentos y versiones

| Versión | Fecha | DOI | Estado |
|---|---|---|---|
| **v1.4** | 2026-10-02 | [10.5281/zenodo.23096141](https://doi.org/10.5281/zenodo.23096141) | Actual |
| v1.3 | 2026-09-04 | [10.5281/zenodo.22292297](https://doi.org/10.5281/zenodo.22292297) | Histórica |

El DOI [10.5281/zenodo.22292296](https://doi.org/10.5281/zenodo.22292296) representa el conjunto de versiones y resuelve a la más reciente.

El PDF histórico de v1.3 permanece en `docs/` para conservar trazabilidad documental. La versión canónica actual es la publicada en Zenodo como v1.4.

---

## Implementación mínima

La formulación mínima de v1.4 está disponible en:

- [`prompts/punt0_v1.4_reglas_minimas.txt`](prompts/punt0_v1.4_reglas_minimas.txt)

El archivo `prompts/arnes_punto_v1.3.txt` se conserva únicamente como **artefacto histórico de v1.3** y no representa la formulación vigente.

---

## Citación

Para citar específicamente la versión actual:

> Salamanca García, Néstor Sebastián. (2026). *La Enunciación como Base de Control Externo en Modelos de Lenguaje* (v1.4). Zenodo. https://doi.org/10.5281/zenodo.23096141

Para referirse al proyecto a través de todas sus versiones:

> https://doi.org/10.5281/zenodo.22292296

También puede usarse el archivo [`CITATION.cff`](CITATION.cff).

---

## Licencia

Este repositorio se distribuye bajo **Creative Commons Attribution-NonCommercial-NoDerivatives 4.0 International (CC BY-NC-ND 4.0)**.

- **BY:** requiere atribución al autor.
- **NC:** la licencia no concede permiso para explotación comercial.
- **ND:** la licencia no concede permiso para distribuir material adaptado o modificado.

Cualquier autorización comercial o uso fuera de estos términos requiere permiso independiente del autor.

[Texto legal de CC BY-NC-ND 4.0](https://creativecommons.org/licenses/by-nc-nd/4.0/legalcode)

---

## Estado del proyecto

PUNT0 continúa en desarrollo. Entre los frentes abiertos se encuentran:

- validación empírica del Yo Absoluto como conjunto;
- desarrollo y validación de PES;
- consolidación del anexo de 36 elementos diagnósticos;
- experimentación interlingüística y deíctica;
- refinamiento de versiones posteriores sin alterar la trazabilidad de las versiones publicadas.
