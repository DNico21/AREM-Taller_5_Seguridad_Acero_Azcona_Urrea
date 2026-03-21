# 📄 Informe Técnico del Taller

## 🔖 Nombre del Taller
_Taller 5 - Evaluación de Seguridad con STRIDE_

## 👥 Integrantes del equipo
- Deivid Nicolás Urrea Lara
- Samuel Acero Garcia
- Andres Felipe Azcona Gomez

## 🧠 Descripción general del trabajo
El objetivo del taller fue analizar los riesgos de seguridad en un sistema mediante el uso del modelo STRIDE, identificando amenazas como suplantación de identidad, manipulación de datos, exposición de información y escalamiento de privilegios. La actividad se desarrolló en dos partes: primero aplicando STRIDE al caso base EdukIT y luego adaptando el análisis a un cliente real, en este caso Cemedica IPS, enfocándose en el proceso de generación, validación y envío de RIPS en formato JSON hacia SISPRO.

## 🔧 Proceso de desarrollo
El trabajo se realizó identificando primero un flujo crítico del sistema del cliente, en este caso el proceso de generación y envío de RIPS. Posteriormente se definieron los componentes involucrados como el sistema legacy, la API de RIPS, la base de datos y el sistema de autenticación. Se utilizó la plantilla proporcionada para clasificar las amenazas según STRIDE y se evaluaron impactos, probabilidades y controles existentes. Finalmente, se propusieron medidas de mitigación alineadas con buenas prácticas de seguridad como MFA, cifrado y control de accesos.

## 🧩 Análisis del modelo propuesto
- El modelo se estructura a partir de una tabla STRIDE que relaciona amenazas con componentes del sistema, activos afectados y controles de seguridad.
- Representa las necesidades del cliente al enfocarse en un proceso crítico que maneja datos sensibles y cumplimiento normativo, como lo es el envío de RIPS a SISPRO.
- Se asumió que el sistema actual carece de mecanismos avanzados de seguridad, como autenticación multifactor, cifrado robusto y trazabilidad completa, lo que permite identificar riesgos potenciales.

## 📈 Diagrama final entregado
> Tabla STRIDE aplicada al flujo de generación, validación y envío de RIPS JSON a SISPRO (ver archivo tabla-stride-cliente.xlsx en el repositorio)

## 📋 Tabla de actores, entidades o componentes (si aplica)

| Nombre del elemento           | Tipo        | Descripción                                                        | Responsable              |
|------------------------------|-------------|--------------------------------------------------------------------|--------------------------|
| Sistema de autenticación     | Componente  | Gestiona el acceso de usuarios al sistema                          | Equipo de Seguridad      |
| API de generación de RIPS    | Componente  | Genera los archivos RIPS en formato JSON                           | Backend                  |
| Módulo de validación RIPS    | Componente  | Valida la estructura y contenido de los RIPS                       | Backend / QA             |
| Servicio de envío a SISPRO   | Componente  | Envía los archivos RIPS al sistema externo SISPRO                  | Infraestructura / Backend|
| Base de datos clínica        | Componente  | Almacena información de pacientes y registros clínicos             | Arquitectura / DB Admin  |
| Usuarios (médicos/admin)     | Actor       | Interactúan con el sistema para generar y gestionar información    | Cliente                  |

## 🔍 Investigación complementaria
### Tema investigado:
Principios de seguridad STRIDE y buenas prácticas en protección de datos en el sector salud

### Resumen:
El modelo STRIDE es un marco de referencia ampliamente utilizado para identificar amenazas de seguridad en sistemas de información. Clasifica los riesgos en seis categorías: Spoofing, Tampering, Repudiation, Information Disclosure, Denial of Service y Elevation of Privilege, permitiendo analizar de forma estructurada las vulnerabilidades en cada componente del sistema.

En el contexto del sector salud, la seguridad de la información es crítica debido a la sensibilidad de los datos clínicos. Normativas como las relacionadas con protección de datos personales (Habeas Data) y estándares internacionales como ISO 27001 recomiendan implementar controles como cifrado de datos, autenticación robusta, control de accesos y monitoreo continuo. Estas prácticas se relacionan directamente con el taller al permitir proponer mitigaciones adecuadas para los riesgos identificados en Cemedica IPS.
---

_Este documento hace parte de la entrega del taller 5 del curso AREM (Arquitectura Empresarial) - Universidad de La Sabana._