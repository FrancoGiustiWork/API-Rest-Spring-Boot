# API REST – Gestión de Productos

API desarrollada como trabajo práctico integrador para la materia **Programación III**, basada en arquitectura en capas, validaciones, manejo global de errores, persistencia con JPA/H2 y documentación con Swagger/OpenAPI.

## Descripción del Proyecto

Esta API REST permite gestionar productos de un e-commerce básico. Incluye creación, actualización, eliminación, consulta por ID y filtrado por categoría.
El proyecto implementa buenas prácticas profesionales:

* Arquitectura en capas (controller, service, repository, model, dto, exception)
* Validación de datos con **Bean Validation**
* Manejo centralizado de errores con **@ControllerAdvice**
* Persistencia con **Spring Data JPA + H2 Database**
* Documentación automática con **Swagger/OpenAPI**
* Uso de DTOs para desacoplar el modelo de dominio de las solicitudes/respuestas

---

## Tecnologías Utilizadas

* **Java 17+**
* **Spring Boot 3.x**
* **Spring Web**
* **Spring Data JPA**
* **H2 Database**
* **Bean Validation (Jakarta Validation)**
* **Lombok**
* **Spring Boot DevTools**
* **Swagger/OpenAPI (springdoc-openapi)**
* **Maven**

---

## Instrucciones para Clonar y Ejecutar el Proyecto

1. **Clonar el repositorio**

```bash
git clone https://github.com/FrancoGiustiWork/API-Rest-Spring-Boot.git
cd API-Rest-Spring-Boot
```

2. **Ejecutar la aplicación**

```bash
mvn spring-boot:run
```

3. **Acceder a la API**

* Swagger UI:
  [http://localhost:8080/swagger-ui/index.html](http://localhost:8080/swagger-ui/index.html)
* Consola H2:
  [http://localhost:8080/h2-console](http://localhost:8080/h2-console)

  * JDBC URL (según configuración): `jdbc:h2:mem:productosdb`
  * Usuario: `sa`
  * Clave: *(vacía)*

---

## Endpoints de la API

| Método     | Ruta                                   | Descripción                                 |
| ---------- | -------------------------------------- | ------------------------------------------- |
| **GET**    | `/api/productos`                       | Lista todos los productos                   |
| **GET**    | `/api/productos/{id}`                  | Obtiene un producto por ID                  |
| **GET**    | `/api/productos/categoria/{categoria}` | Filtra productos por categoría              |
| **POST**   | `/api/productos`                       | Crea un nuevo producto (valida DTO)         |
| **PUT**    | `/api/productos/{id}`                  | Actualiza un producto completo              |
| **PATCH**  | `/api/productos/{id}/stock`            | Actualiza únicamente el stock               |
| **DELETE** | `/api/productos/{id}`                  | Elimina un producto por ID (204 No Content) |

---

## Accesos Útiles

* **Swagger UI:**
  [http://localhost:8080/swagger-ui/index.html](http://localhost:8080/swagger-ui/index.html)
* **Consola H2:**
  [http://localhost:8080/h2-console](http://localhost:8080/h2-console)

---

## Capturas Obligatorias
<img width="1421" height="679" alt="image" src="https://github.com/user-attachments/assets/19480d8e-f0ad-4d5d-8319-85e1233da201" />
<img width="1420" height="890" alt="image" src="https://github.com/user-attachments/assets/47031e74-1071-4266-9acf-5c17c0bcec5e" />
<img width="1419" height="758" alt="image" src="https://github.com/user-attachments/assets/4b45e151-dd85-4a8f-9223-ee3a25d588b0" />
<img width="1426" height="913" alt="image" src="https://github.com/user-attachments/assets/f083cbd6-15d5-4b14-8bba-592c309c9b73" />
![Uploading image.png…]()


---

## Autor

**Nombre:** Franco Giusti
**Legajo:** 50926

---

