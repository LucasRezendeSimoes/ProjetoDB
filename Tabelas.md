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
