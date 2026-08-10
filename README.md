# nube-mensajes

Mensajes diarios para la app **Nube** 🐶. La app descarga `messages.json` de este repo y muestra un mensaje según el día del año (`día % total de mensajes`).

## Cómo agregar mensajes

Edita `messages.json` y agrega objetos a la lista `mensajes`:

```json
{ "texto": "Tu mensaje aquí" }
```

Con imagen opcional (ruta relativa dentro de este repo):

```json
{ "texto": "Mira esto:", "imagen": "imagenes/foto.png" }
```

Pon las imágenes en la carpeta `imagenes/`.

## Conectar con la app

En `app/src/main/java/com/fabi/nube/MessageRepo.kt` cambia:

```kotlin
const val REPO_RAW_BASE = "https://raw.githubusercontent.com/TODO_USER/nube-mensajes/main"
```

por la URL real de este repo (usuario y nombre correctos). El repo debe ser **público**.
