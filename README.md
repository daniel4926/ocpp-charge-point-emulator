#SKY-EVSE OCPP 1.6-J Simulator ⚡🔌

Un simulador ligero, de un solo archivo (Single-File) y basado en navegador para estaciones de carga de vehículos eléctricos (EVSE). Implementa el protocolo **OCPP 1.6 JSON** y está diseñado para ayudar a desarrolladores a probar y depurar sistemas centrales (CSMS / Backends) sin necesidad de hardware físico.

## Características Principales

- **Zero Install:** No requiere Node.js, Python, ni frameworks complejos. Solo abre el archivo `index.html` en cualquier navegador moderno.
- **Interfaz Intuitiva:** Paneles separados para configuración, operaciones manuales, simulación de medidor y consola de logs.
- **Consola de Logs JSON:** Visualización en tiempo real del tráfico WebSocket con mensajes formateados (Pretty Print) y diferenciación por colores (Entrada, Salida, Sistema, Errores).
- **Operaciones Core Implementadas:**
  - `BootNotification`
  - `Heartbeat`
  - `Authorize`
  - `StartTransaction` / `StopTransaction`
  - `MeterValues` (Envío único o en bucle automático)
  - `StatusNotification`
- **Soporte para Comandos Remotos (Server-to-Client):**
  - `RemoteStartTransaction`
  - `RemoteStopTransaction`
  - `TriggerMessage`
  - `Reset`
  - `UnlockConnector`
  - `GetConfiguration` / `ChangeConfiguration`

## Requisitos

- Un navegador web moderno (Chrome, Firefox, Edge, Safari).
- Conexión a internet (para cargar la librería jQuery desde su CDN).
- Un servidor OCPP 1.6 (CSMS) local o remoto para establecer la conexión.


