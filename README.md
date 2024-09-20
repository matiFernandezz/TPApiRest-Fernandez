# Desarrollo de Software - Trabajo Práctico API REST

## Autor

**Matias Fernández** - Legajo: **49483** - Comisión **3K10**

## Descripcion
Este es un proyecto de ejemplo realizado con JPA, Envers, y una base de datos en memoria H2. El proyecto está diseñado para demostrar el uso de entidades, relaciones y auditoría en un contexto de API REST.

## Tecnologías Utilizadas

- **Java**: Lenguaje de programación.
- **JPA (Java Persistence API)**: Para la persistencia de datos.
- **Hibernate Envers**: Para la auditoría de cambios en las entidades.
- **H2 Database**: Base de datos en memoria para pruebas.

## Configuración del Proyecto

### Requisitos implementados 

- JDK 17 o superior
- Gradle
- IDE (IntelliJ IDEA)
- H2 Database
- Envers
- JPA
- Hibernate
- Java Persistence API
- OpenAPI

## Packages del Proyecto
- **audit**: Contiene la clase Revision.
- **config**: Contiene la clase CustomRevisionListener para la auditoría.
- **controllers**: Contiene el controlador de Persona, Autor y Localidad.
- **entities**: Contiene las entidades Autor, Domicilio, Libro, Localidad y Persona.
- **repositories**: Contiene el repositorio de Persona, Autor y Localidad.
- **services**: Contiene la interfaz AutorService, PersonaService y LocalidadService, con sus Implementaciones.

## Ejecutar el Proyecto
### Paso 1
Descargar el repositorio de GitHub.

```bash
git clone https://github.com/matiFernandezz/TPApiRest-Fernandez
```
### Paso 2
Abrir el proyecto en IntelliJ IDEA.
### Paso 3
Ejecutar el archivo 'Inicial1Application.java' dentro del proyecto.

### Paso 4
- En el navegador: 
  - Abrir la consola de H2: ("localhost:8080/h2-console")\
  [H2 Console](http://localhost:8080/h2-console)
  - Abrir la consola de OPEN API: ("localhost:8080/swagger-ui/index.html")\
  [OPEN API](http://localhost:8080/swagger-ui/index.html)



## Imágenes del Proyecto
### Entidades Creadas en H2
![H2](/src/Capturas/Tablas%20Creadas%20en%20H2.png)

### Vista de OPEN API
![OPEN API](/src/Capturas/Vista%20OpenApi.png)

### Vista de Controllers
![CONTROLLER](/src/Capturas/VistaControladores.png)

### Método POST para la entidad Autor 
![PostAutor](/src/Capturas/PostAutor.png)
### Creación de la Tabla Autor
![TablaAutor](/src/Capturas/TablaAutor.png)

### Método POST para la entidad Localidad
![PostLocalidad](/src/Capturas/PostLocalidad.png)
### Creación de la Tabla Localidad
![TablaLocalidad](/src/Capturas/TablaLocalidad.png)

### Método POST para la entidad Persona
![PostPersona](/src/Capturas/PostPersona.png)
### Creación de la Tabla Persona
![TablaPersona](/src/Capturas/TablaPersona.png)

#### A partir de la utilización del método POST en la entidad Persona, se crean las tablas de Domicilio y Libro

### Creación de la Tabla Domicilio 
![TablaDomicilio](/src/Capturas/TablaDomicilio.png)
### Creación de la Tabla Libro 
![TablaLibro](/src/Capturas/TablaLibro.png)

### Tablas Persona_Libro y Libro_Autor creadas por las relaciones
![TablaPersonaLibro](/src/Capturas/Persona_Libro.png)
![TablaLibroAutor](/src/Capturas/Libro_Autor.png)

### Obteniendo la Persona por ID
![GetById](/src/Capturas/GetPersonaById.png)
