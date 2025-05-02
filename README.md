# DataFlowLab

Laboratorio de flujos de datos y concurrencia.  
Demuestra manejo de estado, resiliencia y asincronía moderna en iOS.

---

## Propósito

Dominar el manejo de estado y concurrencia en aplicaciones reales.  
Aplicar `Combine`, `async/await`, `Task`, y patrones de resiliencia.

---

## Contenido

- Manejo de errores y cancelaciones
- Integración con servicios simulados
- Ejecución concurrente segura
- Estrategias de recuperación

---

## Ideal para:

- Comprender los desafíos reales del data flow
- Practicar arquitecturas resilientes
- Validar flujos asincrónicos en UI reales

---

## Ejemplo

```swift
Task {
    let result = try await viewModel.fetchContacts()
    await MainActor.run {
        self.state = .loaded(result)
    }
}

