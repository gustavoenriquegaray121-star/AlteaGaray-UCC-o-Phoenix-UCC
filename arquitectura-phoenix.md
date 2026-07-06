graph TD
A[Sensores Criogénicos] --> B[Interfaz AXI4-Lite]
B --> C[Filtro Binomial Multitap]
C --> D[PHSE Core<br/>Estimación de Estado Homeostático Predictivo]
D --> E[Predictor Híbrido Binomial]
E --> F[Analizador de Trayectoria<br/>(Velocidad + Sacudida)]
F --> G[Índice de Estabilidad Homeostática]
G --> H{Riesgo de Quench?}
H -->|Sí| I[Alerta Predictiva + Acción Preventiva]
H -->|No| J[Control Estándar]
I --> K[Controlador de Vigilancia<br/>Degradación Segura<br/>Respaldo PID]
J --> K
K --> L[Actuadores Criogénicos]

style D fill:#1e3a8a,stroke:#60a5fa,stroke-width:3px
style G fill:#166534,stroke:#4ade80
