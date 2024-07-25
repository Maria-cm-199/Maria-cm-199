''' mermaid
erDiagram
    Estudiante {
        int id PK
        string nombre
        string email
    }

    Curso {
        string codigo PK
        string nombre
        int creditos
    }

    Inscripcion {
        int id PK
        date fechaInscripcion
        string estado
    }

    Calificacion {
        int id PK
        float nota
    }

    Estudiante ||--o{ Inscripcion : "se inscribe en"
    Curso ||--o{ Inscripcion : "tiene"
    Inscripcion ||--|{ Calificacion : "asigna" '''
    
