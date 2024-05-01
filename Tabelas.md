```mermaid
erDiagram
    Alunos {
        string Nome
        string RA
        string Curso
        string TCC_id
        int Semestre
        int Creditos
    }
    Professores {
        string Nome
        string Id
        string Departamento
        string Disciplina
    }
    Cursos {
        string Nome
        string id
        string Cordenador
    }
    Departamentos {
        string Nome
        string Id
        string Id_chefe
    }
    Disciplinas {
        string Nome
        string Id
        string Departamento
    }
    TCC {
        string TCC_id
        string Id_professor
    }
    Hist_a {
        string RA
        string Id_Curso
        int Semestre
        int ano
        int nota
    }
    Hist_p {
        string Id_Professor
        string RA
        string Id_Curso
        int Semestre
        int ano
    }

    CUSTOMER ||--o{ ORDER : places
    CUSTOMER {
        string name
        string custNumber
        string sector
    }
    ORDER ||--|{ LINE-ITEM : contains
    ORDER {
        int orderNumber
        string deliveryAddress
    }
    LINE-ITEM {
        string productCode
        int quantity
        float pricePerUnit
    }
```
