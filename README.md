# TomTom

🌐 [English version](README.en.md)

Addon de navegación para World of Warcraft 3.3.5a: flecha de ruta ("crazy arrow"),
waypoints en minimapa y mapa del mundo, coordenadas del cursor/jugador y comando
`/way`. Este repositorio es un fork del TomTom original de Cladhaire (r240-release),
mantenido por [WarCrafted](https://logon.warcrafted.com) para su servidor
AzerothCore, con traducción al español y mejoras propias.

## Integración con Questie

TomTom funciona junto a [Questie](https://github.com/warcrafted-server/Questie)
para el seguimiento de misiones. Cuando Questie está instalado:

- Los botones "Establecer objetivo TomTom" del rastreador de misiones, del menú
  de misión y del buscador de Questie crean waypoints de TomTom automáticamente.
- La ruta automática de Questie (AutoRoute) mueve la flecha de TomTom al
  siguiente objetivo sin que tengas que hacer nada.
- La flecha muestra, además del nombre del objetivo, el nombre de la misión a
  la que pertenece (ver más abajo).
- Al completar o abandonar una misión, Questie retira el waypoint
  correspondiente.

No hace falta configurar nada: si detecta Questie cargado, la integración se
activa sola. Si quieres desactivar el nombre de la misión en la flecha, hay una
opción en `/tomtom` → Flecha → "Mostrar nombre de la misión".

## Instalación

1. Copia esta carpeta a `Interface/AddOns/TomTom` en tu cliente de WoW.
2. Activa el addon en la pantalla de selección de personaje.
3. Opcional: instala también [Questie](https://github.com/warcrafted-server/Questie)
   para el seguimiento de misiones.

## Comandos

| Comando | Función |
|---|---|
| `/way <x> <y> [descripción]` | Añade un waypoint en la zona actual |
| `/way <zona> <x> <y> [descripción]` | Añade un waypoint en otra zona |
| `/way reset all` | Elimina todos los waypoints |
| `/way reset <zona>` | Elimina los waypoints de una zona |
| `/cway` o `/closestway` | Apunta la flecha al waypoint más cercano |
| `/wayb` o `/wayback` | Crea un waypoint en tu posición actual |
| `/tomtom` | Abre el panel de opciones |

## Idiomas

Español, inglés, alemán, ruso, chino simplificado y chino tradicional. Ver
[CHANGELOG.md](CHANGELOG.md) para el detalle de cobertura por idioma.

## Licencia

Ver [LICENSE](LICENSE): el código original es de Cladhaire, las modificaciones
de este fork son MIT, y cada librería incluida mantiene su propia licencia.

## Documentación para desarrollo

Ver [CONTRIBUTING.md](CONTRIBUTING.md) si vas a contribuir con cambios en este repositorio.
