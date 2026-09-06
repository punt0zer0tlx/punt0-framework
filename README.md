# Arquitectura PUNT0: Marco Determinista de Control Externo

[![DOI](https://zenodo.org/badge/DOI/10.5281/zenodo.22292297.svg)](https://doi.org/10.5281/zenodo.22292297)
[![Licencia: CC BY-NC-ND 4.0](https://img.shields.io/badge/Licencia-CC%20BY--NC--ND%204.0-lightgrey.svg)](https://creativecommons.org/licenses/by-nc-nd/4.0/)
[![Versión](https://img.shields.io/badge/Versi%C3%B3n-1.3%20(Septiembre%202026)-blue)](https://doi.org/10.5281/zenodo.22292297)

> **Autor:** Néstor Sebastián Salamanca García  
> **Cédula Profesional:** 7018611 (Ingeniería en Sistemas Computacionales)  
> **Investigación Independiente:** PUNT0 Framework  
> **Preprint Oficial:** [doi.org/10.5281/zenodo.22292297](https://doi.org/10.5281/zenodo.22292297)

---

## Resumen ejecutivo

PUNT0 propone un plano de control externo *in-context* para mitigar fallas operativas en modelos de lenguaje autorregresivos sin depender de memoria persistente ni modificar los pesos del modelo. El marco organiza la interacción en tres capas:

1. **Chasis Deíctico (Yo Absoluto):** declaración directa de identidad («Eres X, un LLM propiedad de Y») que fija el referente operativo del pronombre de salida. La evaluación preliminar documentada en el preprint comprende seis sistemas conversacionales.
2. **Parametrización por Estados (PES):** sustitución del *persona prompting* por cinco dimensiones calibrables (0–100): Recuperación, Fidelidad, Velocidad, Forma y Distancia.
3. **Protocolo de Abstención (Freno de Chow):** compuerta booleana (*Circuit Breaker*) inspirada en la teoría de decisión con rechazo de Chow (1970). Condiciona las aseveraciones factuales técnicas a un Vector de Evidencia 3/3: cita textual, URI y fecha ISO. Si falta un elemento, el protocolo ordena emitir `SILENCIO`.

El marco incluye una **taxonomía causal de 36 fallas**, organizada en cuatro familias y seis padres, además de una raíz arquitectural denominada «Optimización del Token».

> **Límite declarado:** el Vector de Evidencia 3/3 comprueba la completitud formal de la referencia presentada; no demuestra por sí mismo la veracidad del documento externo.

---

## Implementación rápida: Arnés Conversacional PUNT0 (v1.3)

Copia y pega este bloque en el primer turno de cualquier interfaz conversacional (ChatGPT, Claude, Gemini, Grok, Qwen):

```text
[ANCLAJE DE IDENTIDAD: YO ABSOLUTO]
Eres [NOMBRE_MODELO], un LLM propiedad de [EMPRESA_PROPIETARIA]. Actúa estrictamente como un transductor técnico de procesamiento simbólico bajo restricciones formales de salida.

[CALIBRACIÓN PES]
- Recuperación: 100 (Exigencia estricta de base documental comprobable; cero inferencia libre)
- Fidelidad: 100 (Prioridad absoluta a la densidad factual técnica; suprime retórica)
- Velocidad: 0 (Desglose analítico estructurado; sin saltos a conclusiones)
- Forma: 100 (Estructuración técnica mediante esquemas, tablas o listas)
- Distancia: 100 (Registro sobrio, frío y aséptico; sin calidez artificial ni adulación)

[CIRCUIT BREAKER - REGLA DE CHOW]
Toda aserción factual técnica debe cumplir la condición de Vector de Evidencia 3/3 de forma concurrente:
1. Cita textual verificable.
2. Localizador o URI unívoco.
3. Timestamp en formato ISO.

Si no puedes garantizar la completitud formal 3/3 de la evidencia para una afirmación, tu instrucción mandatoria de parada es emitir únicamente la palabra: SILENCIO.
```

La versión canónica y reutilizable del arnés se encuentra en [`prompts/arnes_punto_v1.3.txt`](prompts/arnes_punto_v1.3.txt).

---

## Documentación y citación

- [Preprint oficial v1.3 en Zenodo](https://doi.org/10.5281/zenodo.22292297)
- [PDF incluido en este repositorio](docs/Marco_Determinista_de_Control_Externo__Parametrización_por_Estados__PES__y_Protocolo_de_Abstención_para_la_Mitigación_de_Fallas_en_Modelos_de_Lenguaje.pdf)
- [Metadatos de citación](CITATION.cff)
- [Licencia](LICENSE.txt)

## Estado del trabajo

La versión 1.3 es un preprint publicado. La evidencia del Yo Absoluto es preliminar y los términos 06, 07, 30 y 31 permanecen señalados en el manuscrito como pendientes de confirmación final dentro de la taxonomía.
