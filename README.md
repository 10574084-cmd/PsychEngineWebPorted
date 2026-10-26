# PsychEngineWebPorted

Port experimental de **Friday Night Funkin': Psych Engine 0.7.3** para navegador, con publicación automática mediante GitHub Actions y GitHub Pages.

## Estado actual

- [x] Configuración inicial de compilación HTML5 en GitHub Actions.
- [x] Despliegue automático a GitHub Pages cuando la compilación termina correctamente.
- [ ] Compilación HTML5 verificada.
- [ ] Menús y gameplay verificados en navegador.
- [ ] Importación de mods ZIP desde el navegador.
- [ ] Compatibilidad con Lua/HScript de mods.

**Importante:** este repositorio todavía no contiene el motor compilado. El workflow descarga el código fuente oficial de Psych Engine 0.7.3 y prueba compilarlo para HTML5. La configuración de escritorio del motor usa algunas dependencias nativas; por eso una compilación web puede necesitar adaptaciones adicionales. No se debe considerar jugable hasta que Actions termine correctamente y se pruebe el juego publicado.

## Publicación

1. Abre la pestaña **Actions** de este repositorio.
2. Selecciona **Build Psych Engine Web Port**.
3. Pulsa **Run workflow** y espera a que termine.
4. Si la compilación y el despliegue funcionan, activa GitHub Pages en **Settings → Pages → Build and deployment → GitHub Actions** si GitHub lo solicita.
5. La URL del sitio aparecerá en el resumen del trabajo **Deploy to GitHub Pages**.

También se ejecuta automáticamente cuando cambia este workflow o este README en la rama main.

## Mods de la versión 0.7.3

La meta es permitir importar un ZIP de mod desde la página y guardar los archivos en el almacenamiento local del navegador. Eso requiere implementar un cargador web compatible con la estructura del mod; **todavía no está implementado**. Los mods con Lua, HScript, archivos nativos o vídeos pueden requerir cambios extra y no se garantiza compatibilidad automática.

## Código fuente y créditos

El motor base es [ShadowMario/FNF-PsychEngine](https://github.com/ShadowMario/FNF-PsychEngine), versión 0.7.3. Respeta su licencia y las licencias/créditos de cualquier mod y recurso que agregues. Este proyecto no incluye ni redistribuye automáticamente mods de terceros.

## Diagnóstico

Si falla el workflow, abre **Actions → Build Psych Engine Web Port → build → Build HTML5** y comparte el primer error real de compilación. El objetivo es corregir el error concreto, no ocultarlo ni publicar una página vacía como si el juego funcionara.
