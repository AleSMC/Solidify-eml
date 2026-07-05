# Solidify-eml

Framework de auditoría y verificación formal acelerada de Smart Contracts en Solidity mediante Operadores Universales y guiado de pruebas en asistentes formales (Draft, Sketch, and Prove).

Este repositorio contendrá el prototipo del Producto Mínimo Viable (MVP) desarrollado durante la estancia de investigación en el centro de ciberseguridad GSEC Málaga, en el marco de la convocatoria de Premios de la Cátedra de Ciberseguridad UMA-VirusTotal / Google.

## Arquitectura del Proyecto

Solidify-eml implementa un pipeline de auditoría estructurado en tres capas:

1. **Traducción y Mapeo Lógico (src/)**: Procesamiento del AST de Solidity para homogeneizar las invariantes aritméticas y financieras mediante el Operador Binario Universal de Odrzywołek ($e^x - \ln(y)$).
2. **Intuición de Parches (Vibe Proving)**: Integración con APIs de modelos de lenguaje masivos para la conjetura de parches de seguridad y la inyección de comentarios lógicos en línea.
3. **Verificación Formal en Lean 4 (lean/)**: Ciclo de verificación y autorreparación cerrada sobre el demostrador formal Lean 4 mediante automatización táctica con el motor aesop.

## Estructura del Repositorio

* `src/`: Módulos de traducción de AST y parseo de Solidity.
* `lean/`: Especificaciones formales y demostraciones matemáticas en Lean 4.
* `tests/`: Casos de prueba de contratos vulnerables y parches certificados.
* `docs/`: Documentación del proyecto y memoria técnica.

## Licencia

Este proyecto está distribuido bajo los términos de la Licencia GNU General Public License v3.0 (GPL-3.0).
