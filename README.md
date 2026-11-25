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

## Firma y notarización

Desde la versión 3.3.2, Sereno está firmada con Developer ID y notarizada por Apple. Se abre a la primera, sin avisos de seguridad de macOS. Puedes comprobar la descarga con el SHA-256 publicado en las notas de cada versión.

## Actualizaciones

Sereno busca versiones nuevas una vez al día con [Sparkle](https://sparkle-project.org) y te pregunta antes de instalarlas. También puedes usar **◷ › Buscar actualizaciones…**. Cada actualización se verifica con una firma EdDSA y con la firma de código de la app antes de instalarse. Puedes desactivar la revisión automática en **Preferencias › Actualizaciones**.

La única conexión de red de Sereno es la consulta de `appcast.xml` y la descarga del DMG. No se envía tu historial ni datos de uso.
