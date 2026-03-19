classDiagram
    class Componente {
        <<abstract>>
        +Nombre
        +Descripcion
        +Categoria
        +Gama
        +AgregarHijo()*
        +ObtenerHijos()*
        +ObtenerPrecio()*
    }
    
    class Archivo {
        -Precio
        -Marca
        +AgregarHijo() (no hace nada)
        +ObtenerPrecio()
    }
    
    class Directorio {
        -ListaDeHijos
        +AgregarHijo()
        +ObtenerHijos()
        +ObtenerPrecio() (suma recursiva)
    }
    
    Componente <|-- Archivo : hereda
    Componente <|-- Directorio : hereda
    Directorio --> Componente : contiene (0..*)
