```mermaid
graph TD
    A[Sensores Criogénicos] --> B[Interfaz AXI4-Lite]
    B --> C[Filtro Binomial Multitap]
    C --> D[PHSE Core]
    D --> E[Predictor Híbrido Binomial]
    E --> F[Analizador de Trayectoria]
    F --> G[Índice de Estabilidad]
    G --> H{¿Riesgo de Quench?}
    H -->|Sí| I[Alerta Predictiva + Actuación]
    H -->|No| J[Control Normal]
    I --> K[Watchdog Controller]
    J --> K
    K --> L[Actuadores Criogénicos]

    style D fill:#1e3a8a,stroke:#60a5fa,stroke-width:3px
    style G fill:#166534,stroke:#4ade80,stroke-width:3px
