# DIAGRAMAS

### EJERCICIO DE DIAGRAMAS CON MERMAID

### DIAGRAMAS DEL EJERCICIO CAJERO AUTOMÁTICO

##### DIAGRAMA DE FLUJO

```mermaid
flowchart
    A(Preguntamos al usuario) -->B(Cantidad aceptada)
    B -->|No| C(Error)
    B -->|Si| D(Seleccionamos billetes)
    C --> A
    D --> E{Valor>500}
    E -->|Si| F(Sumamos cantidad de billetes necesaria hasta que valor<500)
    E -->|No| G{Valor=0}
    G -->|Si| Z(Resultado)
    G -->|No| H{Valor>200}
    H -->|Si| I(Sumamos cantidad de billetes necesaria hasta que valor<200)
    H -->|No| J{Valor=0}
    K -->|Si| Z(Resultado)
    K -->|No| L{Valor>100}
    L -->|Si| M(Sumamos cantidad de billetes necesaria hasta que valor<100)
    L -->|No| Ñ{Valor=0}
    Ñ -->|Si| Z(Resultado)
    Ñ -->|No| O{Valor>500}
    O -->|Si| P(Sumamos cantidad de billetes necesaria hasta que valor<50)
    O -->|No| Q{Valor=0}
    Q -->|Si| Z(Resultado)
    Q -->|No| R{Valor>20}
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
