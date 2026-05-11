# El Peor Captcha Posible

Entrega para: **Ingeniería de Software Asistida por Inteligencia Artificial** | Fecha: 6 de mayo de 2026

## Descripción

Un captcha interactivo que requiere mantener una pelota en equilibrio sobre una barra inclinada durante 60 segundos. Implementado en HTML, CSS y JavaScript.

## Conversación con IA

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

## Características

- **Tres estados:** Inicio → Juego → Resultado
- **Control:** Flechas izquierda/derecha para inclinar la barra
- **Física realista:** Gravedad, fricción y detección de colisiones
- **HTML5 semántico:** Uso de `<main>`, `<section>`, `<header>`, `<figure>`, `<output>`
- **Responsivo:** Diseño adaptable con CSS variables

---

## Cómo Usar

1. Abre `captcha.html` en el navegador
2. Haz clic en **"Entrar"**
3. Usa **flechas del teclado** para inclinar la barra:
   - Izquierda: levanta lado izquierdo
   - Derecha: levanta lado derecho
4. Mantén la pelota 60 segundos
5. Resultado: ✓ sonrisa si ganas, ✗ tristeza si pierdes

---

## Archivos

- `captcha.html` - Código funcional (HTML + CSS + JS)
- `chat.txt` - Diálogo con IA
- `README.md` - Este documento
