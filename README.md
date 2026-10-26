# PsychEngineWebPorted

Port experimental de **Friday Night Funkin': Psych Engine 0.7.3** para navegador. El objetivo es generar un paquete HTML5 descargable como **GitHub Release**, en vez de depender de GitHub Pages.

## Estado del proyecto

- [x] Workflow de GitHub Actions para compilar el port.
- [x] Publicación preparada como prerelease descargable cuando la compilación termine correctamente.
- [ ] Compilación HTML5 verificada.
- [ ] Menús y gameplay verificados en navegador.
- [ ] Importación de mods ZIP desde el navegador.
- [ ] Compatibilidad con Lua/HScript de mods.

**Importante:** el HTML no se considera jugable hasta que Actions termine bien y se pruebe. El workflow se detiene si no encuentra la salida real de HTML5; no publica una página falsa o vacía.

## Descargar el port

1. Abre [Releases](https://github.com/10574084-cmd/PsychEngineWebPorted/releases).
2. Descarga `PsychEngineWebPort-WebBuild.zip` para obtener el HTML y los recursos que necesita el juego.
3. `PsychEngineWebPort.html` también se adjunta como acceso directo, pero puede no funcionar por sí solo si necesita archivos externos.

Las versiones de prueba se publican como **prereleases** porque este port aún es experimental. Si una compilación falla, no se creará una release nueva.

## Compilación manual

1. Abre [Actions](https://github.com/10574084-cmd/PsychEngineWebPorted/actions).
2. Selecciona **Build and Release Psych Engine HTML Port**.
3. Pulsa **Run workflow**.
4. Al terminar correctamente, abre la pestaña [Releases](https://github.com/10574084-cmd/PsychEngineWebPorted/releases) y descarga el paquete.

## Mods de la versión 0.7.3

La importación de mods ZIP, Lua y HScript todavía no está implementada ni verificada para navegador. Los mods que dependan de APIs nativas pueden necesitar adaptaciones; no se promete compatibilidad automática.

## Código fuente y créditos

El motor base es [ShadowMario/FNF-PsychEngine](https://github.com/ShadowMario/FNF-PsychEngine), versión 0.7.3. Respeta su licencia y las licencias/créditos de cualquier mod o recurso añadido. Este repositorio no redistribuye automáticamente mods de terceros.
