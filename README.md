#  ForoHub

**ForoHub** es una API REST desarrollada como parte de un reto de conocimeinto en Java y Spring Framework

## Características

- Crear un nuevo tópico
- Mostrar todos los tópicos creados
- Mostrar un tópico específico
- Actualizar un tópico
- Eliminar un tópico
- Autenticación y autorización de usuarios

## Tecnologías Utilizadas

- **Java 11**
- **Spring Boot**
- **Spring Data JPA**
- **Spring Security**
- **Hibernate**
- **MySQL** 

1. **Configurar la base de datos**:

    - **Producción**: Actualiza las configuraciones en `src/main/resources/application.properties` con las credenciales de tu base de datos MySQL.

    ```properties
    spring.datasource.url=jdbc:mysql://localhost:3306/forohub
    spring.datasource.username=tu-usuario
    spring.datasource.password=tu-contraseña
    spring.jpa.hibernate.ddl-auto=update
    ```

### Autenticación y Autorización

La API usa **Spring Security** para la autenticación y autorización. Los usuarios deben autenticarse para acceder a los endpoints. 

### Validaciones

- Todos los campos son obligatorios al crear o actualizar un tópico.
- Los mensajes de error se devuelven en caso de fallos en las validaciones.
