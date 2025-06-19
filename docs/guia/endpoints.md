# Tabla de Endpoints

A continuación se presenta una tabla con los endpoints disponibles en la Capybara API, sus métodos HTTP y una breve descripción de su funcionalidad:

| Método | Endpoint               | Descripción                                      |
|--------|------------------------|--------------------------------------------------|
| GET    | `/capybaras`          | Obtiene la lista de todas las capibaras         |
| GET    | `/capybaras/{id}`     | Obtiene los detalles de una capibara específica |
| POST   | `/capybaras`          | Crea una nueva capibara                          |
| PUT    | `/capybaras/{id}`     | Actualiza los datos de una capibara existente   |
| DELETE | `/capybaras/{id}`     | Elimina una capibara de la base de datos        |

## Notas

- Todos los endpoints responden con JSON.
- Los campos requeridos para `POST` y `PUT` están documentados en sus respectivas secciones.
- Por ahora, no se requiere autenticación, pero esto puede cambiar en futuras versiones.

> [POST](./post.md)

> [PUT](./put.md)