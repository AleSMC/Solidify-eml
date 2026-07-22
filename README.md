# Solidify-eml

Framework de auditoría y verificación formal acelerada de Smart Contracts en Solidity mediante Operadores Universales y guiado de pruebas en asistentes formales (Draft, Sketch, and Prove).

Este repositorio contiene el prototipo del Producto Mínimo Viable (MVP) para la auditoría y verificación formal acelerada de Smart Contracts, diseñado originalmente como propuesta de desarrollo para la convocatoria de Premios de la Cátedra de Ciberseguridad UMA-VirusTotal / Google.

## Arquitectura del Proyecto

Solidify-eml implementa un pipeline de auditoría estructurado en tres capas:

1. **Traducción y Mapeo Lógico (src/)**: Procesamiento del AST de Solidity para homogeneizar las invariantes aritméticas y financieras mediante el Operador Binario Universal de Odrzywołek ($e^x - \ln(y)$).
2. **Intuición de Parches (Vibe Proving)**: Integración con APIs de modelos de lenguaje masivos para la conjetura de parches de seguridad y la inyección de comentarios lógicos en línea.
3. **Verificación Formal en Lean 4 (lean_env/)**: Ciclo de verificación y autorreparación cerrada sobre el demostrador formal Lean 4 mediante automatización táctica con el motor aesop.

## Estructura del Repositorio

* `contracts/`: Banco de pruebas con contratos inteligentes de Solidity en versiones vulnerables y parcheadas.
* `src/`: Módulos de orquestación en Python (parser, mapeador a operador universal y cliente del LLM).
* `lean_env/`: Entorno formal con las especificaciones y demostraciones de teoremas en Lean 4.
* `tests/`: Pruebas de integración y test unitarios del pipeline de Python.
* `docs/`: Documentación complementaria y memoria técnica de la propuesta.

## Licencia

Este proyecto está distribuido bajo los términos de la Licencia GNU General Public License v3.0 (GPL-3.0).
