# ForoHub

![Estado del Proyecto](https://img.shields.io/badge/estado-finalizado-green)
![Java](https://img.shields.io/badge/Java-21-blue.svg)
![Último Commit](https://img.shields.io/github/last-commit/Kbn05/AluraChallenge.svg)

**ForoHub** es una plataforma de discusión en línea que permite a los usuarios compartir y gestionar temas relacionados con diversos cursos. La aplicación cuenta con funcionalidades completas para registro, autenticación y manejo de roles.

## 🛠️ Funcionalidades

- Sistema de registro e inicio de sesión para usuarios.
- Gestión integral de temas (crear, editar y eliminar).
- Organización de temas asociados a cursos específicos.
- Roles diferenciados para usuarios (ADMIN y USER), cada uno con permisos personalizados.

## 🔧 Herramientas y Tecnologías

Este proyecto se desarrolló utilizando las siguientes tecnologías y marcos:

- **Lenguaje**: Java 11
- **Framework principal**: Spring Boot
- **Seguridad**: Spring Security
- **Persistencia**: JPA/Hibernate
- **Base de datos**: PostgreSQL
- **Gestión de dependencias**: Maven

## 📂 Estructura del Código

La organización interna del proyecto se distribuye en los siguientes paquetes:

- **`model`**: Define las entidades para la base de datos.
- **`repository`**: Contiene las interfaces que interactúan con el almacenamiento de datos.
- **`service`**: Maneja la lógica del negocio.
- **`controller`**: Implementa las API REST que permiten interactuar con el sistema.
- **`utils`**: Proporciona herramientas y funcionalidades auxiliares.

## 🖥️ Requisitos Previos

Antes de ejecutar la aplicación, asegúrate de contar con:

- **Java 11**: Verifica tu versión usando:
    ```bash
    java -version
    ```
- **PostgreSQL**: Configura tu base de datos para almacenar la información.
- **Maven**: Para compilar y gestionar dependencias.

## 🌐 Endpoints Disponibles

### 📌 Usuarios
- **Registrar un nuevo usuario**:
    ```
    POST /users/register
    ```
- **Inicio de sesión**:
    ```
    POST /users/login
    ```

### 📌 Temas
- **Listar todos los temas**:
    ```
    GET /topics
    ```
- **Crear un nuevo tema**:
    ```
    POST /topics
    ```
- **Actualizar un tema existente**:
    ```
    PUT /topics/{id}
    ```
- **Eliminar un tema**:
    ```
    DELETE /topics/{id}
    ```

## 🚀 Configuración y Ejecución

1. **Clona el repositorio**:
    ```bash
    git clone https://github.com/Kbn05/AluraChallenge.git
    cd AluraChallenge
    ```

2. **Configura tu base de datos PostgreSQL**:
    - Crea una base de datos y ajusta las credenciales en el archivo de configuración `application.properties`.

3. **Ejecuta la aplicación**:
    - Compila y ejecuta el proyecto con Maven:
        ```bash
        mvn spring-boot:run
        ```

4. **Accede a la API**:
    - Una vez en ejecución, la aplicación estará disponible en: `http://localhost:8080`.

## 🎯 Roles y Permisos

- **ADMIN**:
    - Acceso completo a la gestión de usuarios y temas.
- **USER**:
    - Puede participar en los foros y gestionar sus propios temas.

## 🛡️ Seguridad

El proyecto utiliza **Spring Security** para la autenticación y autorización, garantizando el manejo seguro de los datos.

## 🌟 ¡Contribuye!

¿Tienes ideas para mejorar ForoHub? ¡Estamos abiertos a contribuciones! Crea un **fork** del repositorio, desarrolla tu mejora y envía un **Pull Request**. 😊

## 📝 Licencia

Este proyecto está bajo la licencia **MIT**. Consulta el archivo [LICENSE](LICENSE) para más información.

---

¡Comienza a explorar y participar en discusiones de aprendizaje con **ForoHub**!
