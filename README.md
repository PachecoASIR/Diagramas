# DIAGRAMAS

### EJERCICIO DE DIAGRAMAS CON MERMAID

### DIAGRAMAS DEL EJERCICIO CAJERO AUTOMÁTICO

##### DIAGRAMA DE FLUJO

```mermaid
graph TD
    A(Preguntamos al usuario) -->B(Cantidad aceptada)
    B -->|Si| C(Seleccionamos billetes)
    B -->|No| D(Error)
    D --> A
    C --> E{Valor>500}
    E -->|Si| F(Sumamos cantidad de billetes necesaria hasta que valor<500)
    E -->|No| G{Valor=0}
    G -->|Si| Z(Resultado)
    G -->|No| H{Valor>200}
    H -->|Si| I(Sumamos cantidad de billetes necesaria hasta que valor<200)
    H -->|No| J{Valor=0}
    J -->|Si| Z(Resultado)
    J -->|No| K{Valor>100}
    K -->|Si| L(Sumamos cantidad de billetes necesaria hasta que valor<100)
    K -->|No| M{Valor=0}
    M -->|Si| Z(Resultado)
    M -->|No| N{Valor>50}
    N -->|Si| Ñ(Sumamos cantidad de billetes necesaria hasta que valor<50)
    N -->|No| O{Valor=0}
    O -->|Si| Z(Resultado)
    O -->|No| P{Valor>20}
    P -->|Si| Q(Sumamos cantidad de billetes necesaria hasta que valor<20)
    P -->|No| R{Valor=0}
    R -->|Si| Z(Resultado)
    R -->|No| S{Valor>10}
    S -->|Si| T(Sumamos cantidad de billetes necesaria hasta que valor<10)
    S -->|No| U{Valor=0}
    U -->|Si| Z(Resultado)
    U -->|No| V{Valor>5}
    V -->|Si| W(Sumamos cantidad de billetes necesaria hasta que valor<5)
    V -->|No| X{Valor=0}
    X --> Z(Resultado)
```
##### DIAGRAMA DE CLASES

```mermaid
classDiagram
  direction RL
  class Main {
    -cantidad_usuario : int
    -valor_billete : int
    -cantidad_billetes: int
    -mensaje: String []
  }
```

### DIAGRAMAS DEL EJERCICIO FIGURAS GEOMÉTRICAS

##### DIAGRAMA DE FLUJO

```mermaid
graph TD
    A(Preguntamos al usuario) -->B(Operación aceptada)
    B -->|Si| C(Solicitamos valores)
    B -->|No| D(Error)
    D --> A
    C --> E{Suma}
    E -->|Si| F(Sumamos cantidad de billetes necesaria hasta que valor<500)
    E -->|No| G{Valor=0}
    G -->|Si| Z(Resultado)
    G -->|No| H{Resta}
    H -->|Si| I(Sumamos cantidad de billetes necesaria hasta que valor<200)
    H -->|No| J{Valor=0}
    J -->|Si| Z(Resultado)
    J -->|No| K{Multiplicación}
    K -->|Si| L(Sumamos cantidad de billetes necesaria hasta que valor<100)
    K -->|No| M{Valor=0}
    M -->|Si| Z(Resultado)
    M -->|No| N{División}
    N --> Z(Resultado)
```
##### DIAGRAMA DE CLASES

```mermaid
classDiagram
  direction RL
  class Ejercicio5 {
    -p : String []
    -p1 : String []
    -p2 : String []
    -p3 : String []
    -p4 : String []
    -n1 : Double []
    -n2 : Double []
    -resultado : Double []
  }
```
