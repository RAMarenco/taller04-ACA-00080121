# Crear una nueva capibara
### `POST /capybaras`
Este endpoint permite registrar una nueva capibara en la base de datos.
## Encabezados requeridos
```http
POST /capybaras HTTP/1.1
Host: api.capybaras.dev
Content-Type: application/json
Accept: application/json

{
  "nombre": "Carlitos",
  "edad": 4,
  "peso_kg": 48.3,
  "ubicacion": "Llanos venezolanos"
}
```