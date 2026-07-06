graph TD
    A[Sensores Criogénicos] --> B[Interfaz AXI4-Lite]
    B --> C[Multi-Tap Binomial Filter]
    C --> D[PHSE Core<br/>Predictive Homeostatic State Estimation]
    D --> E[Binomial Hybrid Predictor]
    E --> F[Trajectory Analyzer<br/>(Velocity + Jerk)]
    F --> G[Homeostatic Stability Index]
    G --> H{¿Riesgo de Quench?}
    H -->|Sí| I[Alerta Predictiva + Actuación Preventiva]
    H -->|No| J[Control Normal]
    I --> K[Watchdog Controller<br/>Graceful Degradation<br/>Fallback PID]
    J --> K
    K --> L[Actuadores Criogénicos]
    
    style D fill:#1e3a8a,stroke:#60a5fa,stroke-width:3px
    style G fill:#166534,stroke:#4ade80
