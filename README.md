# QA ERLA - Aseguramiento de Calidad del Sistema ERLA

[![Programa Delfín](https://img.shields.io/badge/Programa_Delfin-2026-blue)](https://www.programadelfin.org.mx/)
[![ISO 25010](https://img.shields.io/badge/ISO%2FIEC-25010-green)]()
[![ISTQB](https://img.shields.io/badge/ISTQB-CTFL_v4.0-orange)]()

Proceso de aseguramiento de calidad aplicado al sistema ERLA (Eventos, Rutas, Lugares y Aventuras), plataforma web desarrollada por la Universidad Tecnológica de Bahía de Banderas para la gestión operativa del Hotel Escuela Gran Nayar.

Proyecto desarrollado durante el XXXI Verano de la Investigación Científica y Tecnológica del Pacífico (Programa Delfín 2026) en la UTBB, bajo la asesoría del Mtro. Ernesto Alonso Ávila Soto.

---

## Tabla de contenidos

- [Contexto](#contexto)
- [Objetivo](#objetivo)
- [Metodología](#metodología)
- [Resultados](#resultados)
- [Incidencias principales](#incidencias-principales)
- [Competencias aplicadas](#competencias-aplicadas)
- [Documentación](#documentación)
- [Créditos](#créditos)

---

## Contexto

El sistema ERLA (Eventos, Rutas, Lugares y Aventuras) es una plataforma web modular que apoya la gestión operativa del Hotel Escuela Gran Nayar. Integra módulos de reservaciones, recepción, habitaciones, huéspedes, inventario, finanzas, reportes y centros de consumo.

Al tratarse de un sistema en operación activa y constante evolución, resulta indispensable verificar que sus funcionalidades respondan correctamente y que los distintos roles de usuario ejecuten sus actividades sin errores que afecten la operación diaria.

**Modalidad:** Estancia presencial de 7 semanas (8 de junio al 24 de julio de 2026).
**Institución receptora:** Universidad Tecnológica de Bahía de Banderas (Nuevo Nayarit, Nayarit).
**Asesor académico:** Mtro. Ernesto Alonso Ávila Soto.

---

## Objetivo

Diseñar y ejecutar un proceso de aseguramiento de calidad para el sistema ERLA mediante pruebas funcionales manuales, validación de flujos críticos por rol de usuario y documentación de incidencias, con el fin de mejorar la confiabilidad y experiencia de uso de la plataforma.

### Objetivos específicos

- Analizar la arquitectura funcional y módulos del sistema ERLA.
- Identificar los flujos críticos por cada rol de usuario.
- Diseñar y ejecutar casos de prueba funcionales por módulo.
- Documentar incidencias detectadas y clasificarlas por severidad.
- Verificar la corrección de errores mediante pruebas de regresión.
- Elaborar recomendaciones técnicas de mejora para el sistema.

---

## Metodología

Investigación aplicada, descriptiva y tecnológica con pruebas funcionales manuales estructuradas en 4 fases:

### Fase 1 - Análisis

Revisión de manuales del sistema ERLA. Estudio de la arquitectura funcional, módulos y roles de usuario.

**Roles evaluados:** Administrador, Recepcionista, Mesero, Cajero/Barman, Kitchen/Barista, Cocina, DAF, Housekeeping, Gerente CC y Secretario Académico.

### Fase 2 - Diseño

Identificación de flujos críticos por rol. Elaboración de la Matriz de Casos de Prueba con 105 casos distribuidos en 10 roles del sistema, documentando pasos, resultados esperados y criterios de aceptación.

### Fase 3 - Ejecución

Pruebas manuales en entorno local de red institucional utilizando los navegadores Safari y Google Chrome con credenciales reales para cada rol.

Se evaluaron: navegación, validación de formularios, permisos de acceso, consistencia de interfaz e interacción entre módulos.

### Fase 4 - Documentación

Registro de incidencias con descripción, severidad, pasos para reproducir y evidencia fotográfica. Ejecución de pruebas de regresión para verificar correcciones. Elaboración de recomendaciones técnicas.

**Estándares de referencia:**

- ISO/IEC 25010 (modelo de calidad de producto de software).
- ISTQB Certified Tester Foundation Level v4.0.
- Enfoque de pruebas de caja negra.

---

## Resultados

| Métrica | Valor |
|---|---|
| Casos de prueba ejecutados | 105 |
| Roles de usuario evaluados | 10 |
| Incidencias documentadas | 9 |
| Regresiones verificadas (bugs corregidos y confirmados) | 2 |

**Distribución:**

- **PASS** - Mayoría de casos funcionales correctos.
- **BUG** - 9 incidencias registradas (2 corregidas durante la estancia).
- **REGRESIÓN** - 2 correcciones verificadas exitosamente.

Se realizaron pruebas de regresión que permitieron comprobar la corrección de incidencias previamente reportadas, cerrando el ciclo completo de QA: detección → reporte → corrección → verificación.

---

## Incidencias principales

Entre las incidencias documentadas destacan:

- **BUG-001** - Indicador TIEMPO REAL desconectado en Safari (módulo Kitchen/KDS).
- **BUG-003** - Mesas asignadas no aparecen en KDS en navegador Safari.
- **BUG-006** - Warning de PHP expone rutas del servidor en módulo DAF (Information Disclosure).
- **BUG-007** - Columna Folio recortada por menú lateral en Verificador de Tickets, impidiendo la auditoría visual de folios.

**Regresiones verificadas:**

- Corrección del error al cargar imágenes en servidor (módulo DAF).
- Corrección del botón Cerrar Sesión en rol Mesero.

---

## Competencias aplicadas

- Diseño de planes de prueba y matrices de casos funcionales.
- Ejecución de pruebas manuales bajo enfoque de caja negra.
- Documentación y clasificación de incidencias por severidad.
- Pruebas de regresión y verificación de correcciones.
- Análisis de compatibilidad entre navegadores (Safari vs Chrome).
- Comunicación efectiva con el equipo de desarrollo.
- Aplicación de estándares ISO/IEC 25010 e ISTQB CTFL.

---

## Documentación

- [Constancia Delfín](docs/constancia-delfin.pdf) - constancia oficial de participación en el programa.
- [Constancia UTBB](docs/constancia-utbb.pdf) - constancia emitida por la Universidad Tecnológica de Bahía de Banderas.
- [Reconocimiento Verano XXXI](docs/reconocimiento-verano.pdf) - reconocimiento por la participación en la estancia académica.

**Nota:** La matriz completa de casos de prueba y el informe técnico no se incluyen en este repositorio público por contener información interna del sistema evaluado y de la institución. Se pueden solicitar al autor con autorización del asesor académico.

---

## Créditos

**Autor:** Angel de Jesús Canela Figueroa
**Asesor académico:** Mtro. Ernesto Alonso Ávila Soto
**Institución receptora:** Universidad Tecnológica de Bahía de Banderas
**Institución de origen:** Instituto Tecnológico de Jiquilpan (TecNM)
**Programa:** XXXI Verano de la Investigación Científica y Tecnológica del Pacífico - Programa Delfín 2026

**Aporte al ODS 9 - Industria, Innovación e Infraestructura:** este proyecto contribuye al fortalecimiento de infraestructuras tecnológicas confiables, promoviendo la mejora continua del software mediante procesos sistemáticos de aseguramiento de calidad aplicados a un sistema digital en operación real.
