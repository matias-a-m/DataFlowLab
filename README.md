# DataFlowLab

Laboratorio de flujos de datos y concurrencia.  
Demuestra manejo de estado, resiliencia y asincronía moderna en iOS.

---

## Propósito

Practicar el manejo seguro y eficiente del estado en aplicaciones reales, utilizando técnicas modernas como `async/await`, `Combine` y tareas concurrentes.

---

## Contenido

- Manejo de errores y cancelaciones
- Integración con servicios simulados
- Ejecución concurrente segura
- Estrategias de recuperación ante fallos

---

## Ejemplo

```swift
Task {
    let result = try await viewModel.fetchSecureContent()
    await MainActor.run {
        self.state = .loaded(result)
    }
}
```

---

## Integración con Seguridad

Incluye flujos de datos protegidos con `SecurityKit`, manejo de credenciales sensibles, validaciones y recuperación segura ante fallos.

