# DIAGRAMAS

### EJERCICIO DE DIAGRAMAS CON MERMAID

### DIAGRAMAS DEL EJERCICIO CAJERO AUTOMÁTICO

##### DIAGRAMA DE FLUJO

```mermaid
flowchart LR
    A(Preguntamos al usuario) -->B(Cantidad aceptada)
    B --> C{Decision}
    C -->|No| D(Error)
    C -->|Si| E(Seleccionamos billetes)
    D --> A
    E --> F[Valor>500]
    F --> G{Decision}
    G -->|Si| H(Sumamos cantidad de billetes necesaria hasta que valor<500)
    G --> |No| I[Valor>200]
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
