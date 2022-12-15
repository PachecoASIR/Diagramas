# DIAGRAMAS

### EJERCICIO DE DIAGRAMAS CON MERMAID

### DIAGRAMAS DEL EJERCICIO CAJERO AUTOMÁTICO

##### DIAGRAMA DE FLUJO

```mermaid
flowchart LR
    A(Preguntamos al usuario) -->B(Cantidad aceptada)
    B -->|No| C(Error)
    B -->|Si| D(Seleccionamos billetes)
    C --> A
    D --> E{Valor>500}
    E -->|Si| F(Sumamos cantidad de billetes necesaria hasta que valor<500)
    E -->|No| G[Valor>200]
```
##### DIAGRAMA DE CLASES

```mermaid
sequenceDiagram
    participant Pacheco
    participant Pepe
    Pacheco->>Pepe: Hola Pepe, como estás?
    loop Pensando
        Pepe->>Pepe: Lucha con sus pensamientos
    end
    Note right of Pepe: Pensamientos racionales <br/>Prevalecen!
    Pepe-->>Pacheco: Bien!
    Pepe->>Pacheco: Y tu que tal?
    Pacheco-->>Pepe: Mejor ni hablemos!
```
