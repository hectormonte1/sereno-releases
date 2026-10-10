# Sereno

Sereno es una app gratuita para la barra de menús de macOS que te ayuda a estar un poco más presente: mide de forma local cuánto tiempo pasas activo en tu Mac, te propone pausas suaves y te deja ver tu día y tu semana sin puntuaciones ni rachas. Tu historial nunca sale de tu Mac.

Este repositorio solo contiene los instaladores y el archivo de actualizaciones (`appcast.xml`). El código fuente es privado.

## Requisitos

- macOS 14 Sonoma o posterior.
- Mac con Apple Silicon o Intel.

## Instalación

1. Descarga `Sereno-X.Y.Z.dmg` desde [Releases](https://github.com/hectormonte1/sereno-releases/releases/latest).
2. Abre el DMG y arrastra **Sereno** a **Aplicaciones**.
3. Abre Sereno desde Aplicaciones. Aparecerá el símbolo ◷ en la barra de menús.

## Cómo abrirla la primera vez

Sereno es gratuita y está firmada por su autor, pero **no está notarizada por Apple** (eso requiere una cuenta de pago de Apple Developer). Por eso macOS la bloquea la primera vez que la abres. Solo tienes que autorizarla una vez:

- **macOS 15 Sequoia o posterior:** intenta abrir Sereno, cierra el aviso, ve a **Ajustes del Sistema › Privacidad y seguridad**, baja hasta el mensaje sobre Sereno y pulsa **Abrir igualmente**. Confirma con tu contraseña o Touch ID.
- **macOS 14 Sonoma:** haz **clic derecho (o Control‑clic) sobre Sereno › Abrir** y luego pulsa **Abrir** en el aviso. También funciona el botón **Abrir igualmente** de Privacidad y seguridad.

Después de eso, Sereno se abre normalmente.

## Actualizaciones

Sereno busca versiones nuevas una vez al día con [Sparkle](https://sparkle-project.org) y te pregunta antes de instalarlas. También puedes usar **◷ › Buscar actualizaciones…**. Cada actualización se verifica con una firma EdDSA y con la firma de código de la app antes de instalarse. Puedes desactivar la revisión automática en **Preferencias › Actualizaciones**.

La única conexión de red de Sereno es la consulta de `appcast.xml` y la descarga del DMG. No se envía tu historial ni datos de uso.
