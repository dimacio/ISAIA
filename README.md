# ISAIA

Entrega para: **Ingeniería de Software Asistida por Inteligencia Artificial** | Fecha: 6 de mayo de 2026

## Descripción

Proyecto con dos entregas principales:

1. Un captcha interactivo que requiere mantener una pelota en equilibrio sobre una barra inclinada durante 60 segundos.
2. Una API de calendario modelada en OpenAPI y el chat de diseño usado para entender el esquema REST.

La segunda entrega consiste en `openapi.yml` y `chat_API_calendario.txt`. En esta parte del trabajo se usó una charla previa con Gemini para entender mejor cómo diseñar una API REST, tomando esta API de calendario como ejemplo práctico. Con ese trabajo previo pude armar un prompt ordenado pude obtener la api en un solo paso, si no cuento el intento fallido de visualizarlo en Canvas.

## Conversación con IA

### Captcha

🧑 **Usuario:** Quiero hacer el peor captcha posible. La idea básica es que uno tiene que evitar que se caiga un círculo apoyado en una barra. Quiero una sola implementación en un solo archivo que contenga HTML, CSS y JS.

Necesito tres estados:
1. Un botón que dice "Entrar"
2. El captcha interactivo con flechas izquierda/derecha para inclinar la barra, contador que baja desde 60 segundos
3. Resultado final (sonrisa feliz si ganas, triste si pierdes)

Usa tags semánticos y reduce divs al mínimo.

🤖 **IA:** Entendido. He implementado un captcha interactivo con los tres estados solicitados, HTML5 semántico, simulación física realista y arte ASCII para los resultados.

🧑 **Usuario:** Modifica `posicionXPelota` para colocar la pelota a 5 píxeles del extremo derecho.

🤖 **IA:** He modificado el Canvas para que la pelota inicie a 5 píxeles del extremo derecho de la barra, actualizando la variable `posicionXPelota` tanto en su declaración inicial como en la función que reinicia el estado del captcha. El código ha sido actualizado.

🧑 **Usuario:** Ahora ajusta `anguloBarra` para que comience a 45 grados.

🤖 **IA:** Actualizando el Canvas para que el `anguloBarra` inicie a 45 grados.

🧑 **Usuario:** 45 grados para el otro lado.

🤖 **IA:** Perfecto, ambos lados están configurados a ±45 grados. El proyecto está completo y funcional.

---

### API de Calendario

En la segunda entrega se diseñó una API REST para calendario usando OpenAPI 3.1. La idea fue modelar las siguientes entidades:

- `Evento`: id, título, fecha_hora_inicio (ISO), duración_horas (opcional)
- `Recordatorio`: id, tiempo_previo, unidad_tiempo (minutos u horas), evento_id

Endpoints incluidos:

- `GET /agenta/eventos`
- `POST /agenta/eventos`
- `PUT /agenta/eventos/{id_evento}`
- `DELETE /agenta/eventos/{id_evento}`
- `GET /agenta/eventos/{id_evento}/recordatorios`
- `POST /agenta/eventos/{id_evento}/recordatorios`
- `PUT /agenta/eventos/{id_evento}/recordatorios/{id_recordatorio}`
- `DELETE /agenta/eventos/{id_evento}/recordatorios/{id_recordatorio}`



---

## Características

- **Dos entregas:** Captcha interactivo + API de calendario
- **Especificación OpenAPI 3.1:** Incluye schemas, request bodies y respuestas de error
- **Conversación de diseño:** Registro del intercambio con IA para la segunda entrega
- **Formato compatible:** `openapi.yml`

---

## Cómo Usar

1. Abre `captcha.html` en el navegador para probar el captcha.
2. Prueba `openapi.yml` en Swagger o una herramienta compatible con OpenAPI para validar la especificación de la API de calendario.
3. Consulta `chat_API_calendario.txt` para el diálogo de apoyo utilizado en el diseño.

---

## Archivos

- `captcha.html` - Código funcional del captcha (HTML + CSS + JS)
- `chat_captcha.txt` - Diálogo del primer proyecto de captcha
- `openapi.yml` - Especificación OpenAPI de la API de calendario
- `chat_API_calendario.txt` - Diálogo con Gemini para el diseño de la API de calendario
- `README.md` - Este documento
