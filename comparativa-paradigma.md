flowchart TD
    A[Adquisición Datos] --> B[Filtrado 4-tap]
    B --> C[Derivadas]
    C --> D[PHSE Core]
    D --> E[Predicción 90ns]
    E --> F[Velocidad + Jerk]
    F --> G[Índice Estabilidad]
    G --> H{Desviación?}
    H -->|Sí| I[Alerta]
    H -->|No| J[Continuar]
