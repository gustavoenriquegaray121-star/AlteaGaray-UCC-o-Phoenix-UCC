graph LR
subgraph Reactivos
A[Medicion] --> B{Umbral Superado?}
B -->|No| A
B -->|Si| C[Alarma]
C --> D[Recuperacion Lenta]
end

subgraph Phoenix-UCC
E[Muestreo Continuo] --> F[PHSE]
F --> G{Riesgo?}
G -->|Si| H[Estabilizacion Preventiva]
G -->|No| E
end

style Phoenix-UCC fill:#166534,stroke:#4ade80
