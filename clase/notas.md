# Bitácora de Sesión — Taller: Evaluación de Seguridad con STRIDE

---

## 📆 Fecha de la sesión

Clase 6 — 2025

---

## 👥 Integrantes presentes

- Deivid Nicolás Urrea Lara  
- Samuel Acero García  
- Andrés Felipe Azcona Gómez  

---

## 🧠 Actividades realizadas en clase

**¿Qué se discutió con el equipo?**

El equipo analizó los conceptos de seguridad arquitectónica, enfatizando los principios de confidencialidad, integridad y disponibilidad dentro del diseño de sistemas empresariales. A partir del caso base EdukIT, se identificaron los activos más sensibles del sistema, como los datos personales, información de pagos y registros académicos.

Se discutieron los posibles riesgos asociados a estos activos y la importancia de anticipar amenazas desde el diseño de la arquitectura, siguiendo el enfoque de “security by design”.

---

**¿Qué decisiones de modelado se tomaron?**

- Se seleccionó el flujo crítico **“Procesamiento de pagos con terceros”** como foco del análisis.
- Se decidió aplicar el modelo STRIDE evaluando cada categoría de amenaza sobre este flujo.
- Se estructuró el análisis en una tabla que incluye: componente, amenaza, escenario de ataque, impacto, probabilidad, controles existentes y mitigaciones.
- Se consideraron los actores involucrados en el flujo: estudiante, plataforma EdukIT y pasarela de pagos.
- Se priorizó el uso de amenazas realistas basadas en buenas prácticas de seguridad (MFA, cifrado, control de acceso, etc.).

---

**¿Qué herramientas se usaron?**

- Microsoft Excel para la elaboración de la tabla STRIDE.
- Markdown para la documentación de la bitácora.
- Diapositivas de clase sobre STRIDE como guía conceptual.
- Discusión colaborativa del equipo para identificar amenazas y mitigaciones.

---

**¿Qué parte del trabajo se alcanzó a desarrollar?**

Durante la sesión se logró:

- Identificar un flujo crítico del sistema EdukIT.
- Aplicar el modelo STRIDE de forma completa sobre dicho flujo.
- Definir escenarios de ataque realistas para cada tipo de amenaza.
- Estimar el impacto y la probabilidad de cada riesgo.
- Proponer controles de mitigación alineados con buenas prácticas de seguridad.

---

## 🔁 Tareas definidas para complementar el taller

| Tarea asignada | Responsable | Fecha estimada |
|---|---|---|
| Construcción final de la tabla STRIDE en Excel | Samuel Acero García | Clase 6 |
| Revisión de mitigaciones y nivel de riesgo | Andrés Felipe Azcona Gómez | Clase 6 |
| Documentación de la bitácora y organización del repositorio | Deivid Nicolás Urrea Lara | Clase 6 |

---

> Este documento resume el trabajo colaborativo realizado durante la sesión del Taller 5 en el curso AREM — Universidad de La Sabana.
