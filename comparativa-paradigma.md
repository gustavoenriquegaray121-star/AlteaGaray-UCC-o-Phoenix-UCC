#### 2. Para `plataforma-altea-garay.md` (Corrección de diseño visual colapsado en `1000092824.jpg`)
Cambiando la distribución a `TD` para que se despliegue hacia abajo de forma clara y legible en cualquier pantalla:

```markdown
# Plataforma Completa Altea-Garay UCC v15.0

```mermaid
graph TD
    A[Capa Interfaz de Sensores] --> B[PHSE Core]
    B --> C[Darwin Engine]
    C --> D[Protocolo Phoenix]
    D --> E[Watchdog Controller]
    E --> F[Actuadores Criogénicos]
    
    %% Flujos secundarios de control e interfaces
    G[Bus UCC] --> A
    H[Interfaz de Gemelo Digital] <--> B
    G <--> F
    
    style B fill:#1e3a8a,stroke:
