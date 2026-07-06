# Plataforma Completa Altea-Garay UCC v15.0

```mermaid
graph TD
subgraph AlteaGaray ["Altea-Garay UCC Platform v15.0"]
A[Capa Interfaz de Sensores]
B[Núcleo PHSE]
C[Motor Darwin]
D[Protocolo Phoenix]
E[Controlador Watchdog]
F[Interfaz de Gemelo Digital]
G[Bus AXI4]
H[Actuadores Criogénicos]

A --> B
B --> C
C --> D
D --> E
E --> H
F <--> B
G <--> A
G <--> H
end

style B fill:#1e3a8a,stroke:#60a5fa,stroke-width:4px
