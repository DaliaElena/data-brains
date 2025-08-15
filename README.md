# 📊 Monitoreo y Golden Metrics – Data-Brains

Este documento describe las métricas clave (Golden Metrics) y cómo visualizarlas para el sitio [www.data-brains.net](https://www.data-brains.net).

## 📌 Golden Metrics

| Métrica     | Descripción | Herramienta de seguimiento |
|-------------|-------------|----------------------------|
| **Latency** | Tiempo de respuesta del sitio (ms). | Pingdom, UptimeRobot |
| **Traffic** | Número de visitas / solicitudes HTTP. | Google Analytics, Plausible |
| **Errors**  | Porcentaje de errores 4xx / 5xx. | UptimeRobot, Google Search Console |
| **Saturation** | Uso de recursos o límites de hosting. | GitHub Pages Usage (Settings) |

---

## 🔍 Cómo visualizar las métricas

### 1. Disponibilidad y tiempo de respuesta (Latency & Errors)
- Configura un monitor en **[UptimeRobot](https://uptimerobot.com/)** o **[Pingdom](https://www.pingdom.com/)**.
- Ejemplo con UptimeRobot:
  1. Crear un monitor tipo *HTTP(s)*.
  2. URL: `https://www.data-brains.net`
  3. Intervalo: 5 minutos.
  4. UptimeRobot mostrará tiempo de respuesta promedio y porcentaje de disponibilidad.

### 2. Tráfico (Traffic)
- Si quieres datos sin cookies, usa **[Plausible](https://plausible.io/)** o **[Umami](https://umami.is/)**.
- Para integración rápida:
  ```html
  <script async defer data-domain="data-brains.net" src="https://plausible.io/js/script.js"></script>
