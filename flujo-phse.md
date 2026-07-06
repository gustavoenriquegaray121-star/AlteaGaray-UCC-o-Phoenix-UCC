graph LR
    subgraph Reactivo ["Sistemas Convencionales (Reactive)"]
        A[Medición] --> B[Umbral Excedido?]
        B -->|No| A
        B -->|Sí| C[Alarma + Protección]
        C --> D[Recuperación Lenta<br/>24-72 horas]
    end

    subgraph Predictivo ["Phoenix-UCC (Predictive)"]
        E[Medición Continua] --> F[PHSE Core]
        F --> G{¿Trayectoria hacia Quench?}
        G -->|Sí| H[Preventive Thermal Stabilization]
        G -->|No| E
    end

    style Predictivo fill:#166534,stroke:#4ade80
