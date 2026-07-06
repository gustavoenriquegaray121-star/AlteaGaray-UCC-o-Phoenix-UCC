graph TD
    A[Sensores] --> B[AXI4 Interface]
    B --> C[Filtro Binomial]
    C --> D[PHSE Core]
    D --> E[Predictor Binomial]
    E --> F[Trayectoria]
    F --> G[Estabilidad]
    G --> H{Riesgo Quench?}
    H -->|Sí| I[Alerta + Actuación]
    H -->|No| J[Control Normal]
    I --> K[Watchdog]
    J --> K
    K --> L[Actuadores]
