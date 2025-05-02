# DataFlowLab

**Exploración de manejo de estado, concurrencia moderna y resiliencia.**

`DataFlowLab` permite experimentar con `async/await`, `Combine` y estructuras modernas para construir flujos de datos seguros, reactivos y predecibles.

---

## Propósito

- Probar distintos modelos de estado en escenarios reales.
- Analizar puntos de falla y recuperación de datos.
- Integrar persistencia y recuperación sin bloquear la UI.

---

## Contenido

- Modelos de estado centralizados (ObservableObject, StateObject).
- Ejecuciones controladas con `async/await`.
- Integración básica de `Combine` para flujos reactivos.
- Simulación de errores, estados de carga, y recuperación.

---

## Pruebas

| Componente     | Tipo de prueba         |
|----------------|------------------------|
| Estado         | Unitarias              |
| Carga remota   | Simulación + async     |
| Recuperación   | Validación de fallback |

---

## Integración

Usado desde `ProductSuiteApp` como módulo exploratorio. Permite aislar problemas de concurrencia y probar su impacto en la experiencia del usuario.

---

## Requisitos

- iOS 15+
- Swift 6
- Swift Package Manager

---

## Licencia

MIT © Matías Adrián Molina
