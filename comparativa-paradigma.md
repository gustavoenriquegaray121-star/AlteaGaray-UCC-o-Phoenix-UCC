# Comparativa de Paradigmas de Control

```mermaid
graph LR
subgraph Sistemas Convencionales [Sistemas Reactivos Convencionales]
A[Medición] --> B{¿Umbral Superado?}
B -->|No| A
B -->|Sí| C[Alarma + Protección]
C --> D[Recuperación Lenta<br/>24 a 72 horas]
end

subgraph PhoenixUCC [Phoenix-UCC (Predictivo)]
E[Muestreo Continuo] --> F[Procesamiento PHSE]
F --> G{¿Ruta hacia Quench?}
G -->|Sí| H[Estabilización Preventiva]
G -->|No| E
end

style PhoenixUCC fill:#166534,stroke:#4ade80
