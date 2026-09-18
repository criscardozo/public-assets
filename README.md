# public-assets

Archivos que necesitan una **URL pública y estable**: íconos de notificaciones,
imágenes para READMEs de repos privados, y demás.

Existe por una razón concreta: varios servicios (ntfy.sh entre ellos) piden una
URL que su servidor pueda descargar sin autenticación. Los repos privados no
sirven para eso, y los hosts de imágenes gratuitos se caen o limitan el tráfico
sin avisar, dejando la imagen rota en silencio.

**Nada sensible acá.** Todo lo de este repo es visible para cualquiera.

## Contenido

| Archivo | Para qué |
| --- | --- |
| `dotfiles/icon.png` | Ícono de [dotfiles](https://github.com/criscardozo/dotfiles) y de `dotfilesUI`, 512 px |
| `dotfiles/icon-256.png` | El mismo a 256 px, para notificaciones |
| `dotfiles/icon.svg` | El fuente vectorial |
| `media-stack/seerr.png` | Logo de Seerr, para los avisos de ObiWan |
| `media-stack/radarr.png` | Logo de Radarr, ídem |
| `media-stack/sonarr.png` | Logo de Sonarr, ídem |
| `media-stack/prowlarr.png` | Logo de Prowlarr, ídem |
| `media-stack/bazarr.png` | Logo de Bazarr, ídem |
| `media-stack/trailarr.png` | Logo de Trailarr, ídem |
| `media-stack/obiwan.png` | El sable de ObiWan, para los avisos del sistema (fallas de servicios) |

Los de `media-stack/` son los logos oficiales de cada proyecto, copiados acá
para que las notificaciones no dependan de que un repo ajeno mueva un archivo.
Todos a 256 px salvo `bazarr.png`, que es de 128: es el tamaño más grande que
publica el proyecto con fondo transparente, y agrandarlo sería inventar píxeles.

Se eligieron mirándolos sobre fondo claro **y oscuro**: en la pantalla de
bloqueo de un teléfono en modo oscuro, un logo sin fondo propio desaparece.

## Cómo se usan

Las URLs `raw` sirven el archivo directo, sin autenticación:

```
https://raw.githubusercontent.com/criscardozo/public-assets/main/dotfiles/icon-256.png
```
