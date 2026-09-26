# Contribuir a Nephrite

[English](CONTRIBUTING.md) · **Español**

Nephrite crece de a una app a la vez, y la mayoría de esos temas los harán personas como tú. Gracias por estar aquí.

## Formas de ayudar

- **Pedir una app.** Dinos cuál quieres con el [formulario para pedir una app](https://github.com/Nephrite-theme/web/issues/new?template=port-request.yml). Si ya la pidieron, deja un 👍 en ese issue; usamos los votos para decidir el orden.
- **Crear un port.** Aplica la paleta Nephrite a una app. Más abajo está cómo.
- **Reportar un problema.** Un color que choca, poco contraste o una instalación que falla: abre un issue en el repositorio de ese port, o usa el [formulario de problemas](https://github.com/Nephrite-theme/web/issues/new?template=bug-report.yml) si es del sitio.
- **Traducir el sitio.** Los textos están en [`web/messages`](https://github.com/Nephrite-theme/web/tree/main/messages), un archivo JSON por idioma.

## Crear un port

1. **Revisa que esté libre.** Mira [getnephrite.dev/es/ports](https://getnephrite.dev/es/ports) y los [pedidos abiertos](https://github.com/Nephrite-theme/web/issues?q=is%3Aissue+label%3A%22port+request%22). Si alguien ya tomó la app, coordínense en ese issue.
2. **Resérvalo.** Comenta en el pedido (o abre uno) diciendo que lo estás creando, para no duplicar trabajo.
3. **Parte de la plantilla.** Haz clic en **Use this template** en [Nephrite-theme/template](https://github.com/Nephrite-theme/template). Trae el README, las carpetas, un script para sincronizar la paleta y un checklist.
4. **Usa la paleta según su función.** Toma los colores de [Nephrite-theme/palette](https://github.com/Nephrite-theme/palette) y sigue su [guía para ports](https://github.com/Nephrite-theme/palette/blob/main/README.es.md#crear-un-port): qué color va en fondos, texto, acentos, sintaxis y terminal. No inventes colores nuevos; si a la paleta le falta algo, abre un issue en su repositorio.
5. **Incluye los sabores.** Publica Forest, Jade y Mint si la app admite varios temas. Si solo admite uno, empieza por Forest.
6. **Documéntalo.** Un README con los pasos de instalación y una captura por sabor. Nombra el repositorio `<app>` si vivirá en la organización, o `<app>-nephrite` en tu propia cuenta.
7. **Envíalo.** Abre un [envío de port](https://github.com/Nephrite-theme/web/issues/new?template=port-submission.yml) con el link al repositorio y las capturas.

### Qué revisamos

- Los colores salen de `palette.json` y se usan según su función.
- El texto se lee bien: el texto principal con 4.5:1 de contraste o más sobre su fondo.
- El README explica la instalación.
- El port tiene licencia MIT.

### Después de la revisión

Los ports aceptados aparecen en [getnephrite.dev/es/ports](https://getnephrite.dev/es/ports). Tu repositorio sigue siendo tuyo. Si quieres, puede pasar a la organización Nephrite-theme contigo como responsable; lee [Mantener un port](#mantener-un-port).

## Mantener un port

### Dónde puede vivir un port

- **En tu cuenta.** El repositorio sigue siendo tuyo y lo enlazamos desde la web. No cambia nada más.
- **En la organización.** Cuando un port es aceptado y quieres seguir cuidándolo, puede pasar a Nephrite-theme. Es más fácil de encontrar y sigue funcionando aunque algún día te alejes.

Para mover un port que ya existe, agrega a un owner de Nephrite como **Admin** de tu repositorio y nosotros lo transferimos. GitHub redirige los enlaces viejos, así que nada se rompe. Para una app nueva también podemos crear el repositorio en la organización desde la plantilla y darte acceso desde el primer día, sin necesidad de transferir.

### Roles

| Rol | Quién | Acceso |
| --- | --- | --- |
| Contribuidor | Cualquiera que abra issues o pull requests | Ninguno |
| Responsable de un port | Quien cuida un port dentro de la organización | **Maintain** en el repositorio de ese port, mediante un equipo como `@Nephrite-theme/obsidian-maintainers` |
| Equipo central | Responsables de confianza que ayudan en todo el proyecto | **Write** en `palette`, `web` y `template` |
| Owner | Quien dirige el proyecto | Todo |

Por defecto, los miembros de la organización solo tienen acceso de lectura; cada rol suma acceso a repositorios concretos. Los miembros deben usar autenticación en dos pasos.

### Qué hace un responsable

- Revisa los issues y pull requests del port. Los pull requests a `main` necesitan la aprobación de un code owner.
- Mantiene el port al día con cada versión de la paleta (`sync-palette` y luego `build`).
- Publica releases y mantiene el README y las capturas al día.

### Fichas en tiendas

Los ports publicados en una tienda (Chrome Web Store, Firefox Add-ons, VS Code Marketplace, Open VSX) se publican desde las cuentas de Nephrite, y los responsables se agregan a ellas. Así una ficha y sus usuarios nunca dependen de una cuenta personal.

### Dejar un port

Pasa. Si no puedes seguir manteniendo un port, dilo en un issue y buscaremos a alguien más. Si un port pasa unos seis meses sin actividad, te escribiremos; si no hay respuesta, se retira el acceso y apareces en **Past maintainers** en su README.

## Pull requests

- Mantén cada pull request enfocado en un solo cambio.
- Describe qué cambió y agrega una captura para cualquier cambio visual.
- Los mensajes de commit siguen [Conventional Commits](https://www.conventionalcommits.org/es) cuando sea posible (`feat:`, `fix:`, `docs:`).

## Sé amable

Asume buena intención, comenta el trabajo y no a la persona, y ayuda a quien recién llega. Los mantenedores pueden quitar comentarios o contribuciones que no sigan esto.
