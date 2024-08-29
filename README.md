flowchart TD
    A[Subgerente de Obras Públicas e Infraestructura Menor]
    
    B[Coordinador de Proyectos]
    C[Supervisor de Obras]
    D[Encargado de Seguridad y Salud Ocupacional]
    E[Encargado de Control de Calidad]
    F[Administrativo de Proyectos]
    G[Ingenieros de Proyecto]
    H[Equipo de Trabajo / Obreros]

    A --> B
    A --> C
    A --> D
    A --> E
    A --> F
    
    B --> G
    C --> H
    D --> H
    E --> H

    subgraph Planificación y Programación
        B --> |Elaboración de planes de proyecto| G
        F --> |Control del presupuesto| B
    end
    
    subgraph Ejecución y Supervisión
        C --> |Supervisión de ejecución| G
        C --> |Control de contratistas| H
        D --> |Implementación de planes de seguridad| H
        E --> |Implementación de controles de calidad| H
    end
    
    subgraph Gestión Administrativa
        F --> |Gestión de documentación| A
        F --> |Control financiero| A
        F --> |Reportes de progreso| A
    end
