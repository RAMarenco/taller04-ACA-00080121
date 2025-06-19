# Guía de uso

Esta guía te ayudará a comenzar rápidamente con el uso de la **Capybara API**.  
A través de ejemplos prácticos, aprenderás cómo conectarte, realizar solicitudes y manipular datos de capibaras desde distintos lenguajes.

## Requisitos

No necesitas autenticación para comenzar (por ahora).  
Solo asegúrate de tener acceso a internet y usar alguna herramienta o lenguaje que permita hacer solicitudes HTTP.

## Primeros pasos

A continuación, te mostramos cómo obtener la lista de capibaras usando diferentes lenguajes.

=== "cURL"
    ```bash
    curl -X GET https://api.capybaras.dev/capybaras \
      -H "Accept: application/json"
    ```

=== "Python (requests)"
    ```python
    import requests

    url = "https://api.capybaras.dev/capybaras"
    response = requests.get(url)
    data = response.json()

    for capy in data:
        print(f"{capy['nombre']} tiene {capy['edad']} años")
    ```

=== "JavaScript (fetch)"
    ```javascript
    fetch("https://api.capybaras.dev/capybaras")
      .then(res => res.json())
      .then(data => {
        data.forEach(capy => {
          console.log(`${capy.nombre} tiene ${capy.edad} años`);
        });
      });
    ```

## Siguientes pasos

Una vez que puedas obtener la lista de capibaras, puedes:

- Usar `GET /capybaras/{id}` para ver detalles específicos.
- Usar `POST` para agregar nuevas capibaras.
- Usar `PUT` y `DELETE` para editar o eliminar registros.

Continúa con la sección de [endpoints](./endpoints.md) para explorar todas las operaciones disponibles.

!!! tip "Consejo"
    Puedes usar herramientas como [Postman](https://www.postman.com/) o [Insomnia](https://insomnia.rest/) si prefieres explorar la API sin escribir código.

