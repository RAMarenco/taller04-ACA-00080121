# Actualizar una capibara existente

### `PUT /capybaras/{id}`

Este endpoint permite actualizar los datos de una capibara existente identificada por su ID.

---

## Encabezados requeridos

```http
PUT /capybaras/7 HTTP/1.1
Host: api.capybaras.dev
Content-Type: application/json
Accept: application/json

{
  "nombre": "Carlitos",
  "edad": 5,
  "peso_kg": 50.0,
  "ubicacion": "Delta del Orinoco"
}
```