flowchart TD
    A[Adquisición de Datos Multi-canal] --> B[Filtrado Binomial 4-tap]
    B --> C[Cálculo de Derivadas Temporales]
    C --> D[PHSE Core]
    D --> E[Predicción de Trayectoria 90 ns]
    E --> F[Análisis de Velocidad + Jerk]
    F --> G[Índice de Estabilidad]
    G --> H{Desviación Predictiva?}
    H -->|Sí| I[Alerta Temprana + Intervención]
    H -->|No| J[Monitoreo Continuo]
    I --> K[Registro en Gemelo Digital]
    J --> K
