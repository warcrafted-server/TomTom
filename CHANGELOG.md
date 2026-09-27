# Changelog

Formato basado en [Keep a Changelog](https://keepachangelog.com/es-ES/1.0.0/).
Versionado [SemVer](https://semver.org/lang/es/) propio de este fork.

## [Sin publicar]

## [1.1.0] - 2026-09-27

### Añadido
- Traducción completa al español (esES/esMX), 148 cadenas.

### Corregido
- `WaypointExists` devolvía tras la primera iteración del bucle.
- `AddZWaypoint` fallaba con `custom_callbacks` sin tabla `.distance`.
- `CHAT_MSG_ADDON` podía recibir datos nulos y romper con un waypoint
  mal formado.
- `Block_OnClick` fallaba al pulsar el bloque de coordenadas sin
  posición del jugador (p. ej. dentro de una instancia).
- `ShowWaypoint` leía campos inexistentes (`point.data.*`).
- El menú "eliminar waypoints de esta zona" de la flecha podía indexar
  un waypoint ya eliminado.
- `Minimap_OnUpdate` compartía el contador de throttle entre todos los
  iconos de waypoint en vez de llevar uno por icono.
- Variables globales sin declarar (`cell`, `numObjectives`) que
  contaminaban `_G`.
- Autor duplicado y versión fija en `TomTom.toc`; ahora refleja la
  versión real del addon.

## [1.0.0] - 2026-09-27

Punto de partida de este fork: TomTom r240-release (Cladhaire), sin modificaciones,
para WoW 3.3.5a (Interface 30300).

### Idiomas incluidos
- Alemán (deDE): 71 cadenas
- Chino simplificado (zhCN): 114 cadenas
- Chino tradicional (zhTW): 114 cadenas
- Ruso (ruRU): 118 cadenas
- Inglés (enUS): fallback vacío (usa la clave como texto)

[Sin publicar]: https://github.com/warcrafted-server/TomTom/compare/v1.1.0...HEAD
[1.1.0]: https://github.com/warcrafted-server/TomTom/compare/v1.0.0...v1.1.0
[1.0.0]: https://github.com/warcrafted-server/TomTom/releases/tag/v1.0.0
