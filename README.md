#Santader 2024

## Diagrama de classes

```mermeid
classDiagram
    class Usuario {
        -name: String
    }

    class Conta {
        -number: String
        -agency: String
        -balance: Float
        -limit: Float
    }

    class Feature {
        -icon: String
        -description: String
    }

    class Cartao {
        -number: String
        -limit: Float
    }

    class Noticia {
        -icon: String
        -description: String
    }

    Usuario --> Conta : possui
    Usuario --> "0..*" Feature : possui
    Usuario --> Cartao : possui
    Usuario --> "0..*" Noticia : possui
```
