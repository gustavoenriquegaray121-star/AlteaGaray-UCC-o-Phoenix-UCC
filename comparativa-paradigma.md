flowchart TD
    A[Adquisición de Datos Multi-canal] --> B[Filtrado Binomial 4-tap]
    B --> C[Cálculo de Derivadas Temporales]
    C --> D[PHSE Core<br/>Predictive Homeostatic State Estimation]
    D --> E[Predicción de Trayectoria<br/>Horizonte 90 ns]
    E --> F[Análisis de Velocidad + Jerk]
    F --> G[Cálculo de Índice de Estabilidad]
    G --> H{¿Desviación Predictiva?}
    H -->|Sí| I[Alerta Temprana + Intervención]
    H -->|No| J[Monitoreo Continuo]
    I --> K[Registro en Digital Twin]
    J --> K
