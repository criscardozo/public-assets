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

## Cómo se usan

Las URLs `raw` sirven el archivo directo, sin autenticación:

```
https://raw.githubusercontent.com/criscardozo/public-assets/main/dotfiles/icon-256.png
```
