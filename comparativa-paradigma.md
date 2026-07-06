# Plataforma Completa Altea-Garay UCC v15.0

```mermaid
graph TD
    A[Capa Interfaz de Sensores] --> B[PHSE Core]
    B --> C[Darwin Engine]
    C --> D[Protocolo Phoenix]
    D --> E[Watchdog Controller]
    E --> F[Actuadores Criogénicos]
    
    G[Bus UCC] --> A
    H[Interfaz de Gemelo Digital] <--> B
    G <--> F
    
    style B fill:#1e3a8a,stroke:#60a5fa,stroke-width:4px
