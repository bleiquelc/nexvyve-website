# 🌅 Para revisar al despertar — web nexvyve.com (sesión autónoma 2026-06-16)

> Todo está en LOCAL, **NADA publicado**. Revisa, y cuando apruebes haces `git push` (eso publica en nexvyve.com vía GitHub Pages).

## Cómo verlo
```bash
cd ~/Desktop/nexvyve-website && python3 -m http.server 8899
```
Luego abre http://localhost:8899/ — baja del hero hasta:
1. El bloque **"También en Android · KAEL by NEXVYVE"** (diamante + colores Google) — tras los stats.
2. La feature **"RUTINAS PERSONALIZADAS"** → ahora muestra el **player de entreno EN VIVO** (cronómetro corriendo, anillo llenándose, "Serie 2/4", botón). Antes era una captura estática vieja.

## Lo que hizo el equipo + yo (autónomo)
- **Marketing + Screenshots + UX** analizaron qué vende más. Veredicto: el momento de entreno en vivo es el acelerador de conversión nº1 en fitness → implementado.
- **Player de entreno animado** en la feature de Rutinas: CSS/SVG/JS puro (0 KB de video, nítido en retina, cronómetro real con setInterval, anillo de progreso, contador de series que avanza, fases entreno/descanso). Respeta "reducir movimiento". Bilingüe ES/EN. **Verificado: el cronómetro corre (0:43→0:40 en 3s, anillo avanzando).**
- **Botón KAEL Android** (de la sesión anterior) sigue montado, listo.

## ⚠️ Decisión que necesita TU input: las capturas estáticas viejas (May-30)
Las quería renovar con las capturas del ASC, PERO al revisarlas confirmé que **las ASC son composiciones de marketing completas** (llevan wordmark + titular "EL MÚSCULO DEL DÍA" + fondo + footer), no screenshots limpios de pantalla. Si las meto en los marcos de teléfono de la web se vería "un teléfono dentro de otro" — mal. Por eso NO las usé en los marcos.

**Dos caminos para renovar las capturas (tú eliges mañana):**
- **A)** Generar screenshots LIMPIOS del build 40 (solo la pantalla, sin el compositor de marketing) → encajan perfecto en los marcos actuales. Lo más limpio. (Requiere capturar del simulador/dispositivo o que yo las recree en HTML como hice el player.)
- **B)** Añadir una sección nueva tipo "galería/mural" que muestre los slides ASC completos como pósters a sangre (son bellos con su titular). Usa las ASC tal cual, pero cambia el layout de esa zona.

Mi recomendación: **A** para los marcos (coherencia) + quizás **B** como sección extra de impacto. Pero es tu decisión de marca.

## Estado
- Commit LOCAL hecho (sin push). `git diff` para ver todo. Cuando apruebes: `git push` → publica.
- Nada tocado fuera de index.html (+ este doc).
