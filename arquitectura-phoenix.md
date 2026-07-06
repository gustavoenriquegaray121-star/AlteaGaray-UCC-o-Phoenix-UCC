graph TD
A[Sensores Criogénicos] --> B[Interfaz AXI4-Lite]
B --> C[Filtro Binomial Multitap]
C --> D[PHSE Core Estimación Predictiva]
D --> E[Predictor Híbrido Binomial]
E --> F[Analizador Trayectoria Velocidad Sacudida]
F --> G[Indice Estabilidad Homeostatica]
G --> H{Riesgo de Quench?}
H -->|Si| I[Alerta + Accion Preventiva]
H -->|No| J[Control Estandar]
I --> K[Watchdog Degradacion Respaldo PID]
J --> K
K --> L[Actuadores Criogenicos]

style D fill:#1e3a8a,stroke:#60a5fa,stroke-width:3px
style G fill:#166534,stroke:#4ade80
