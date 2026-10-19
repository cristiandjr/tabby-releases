<p align="center">
  <a href="README.md">English</a> &nbsp;·&nbsp; <b>Español</b>
</p>

<p align="center">
  <picture>
    <source media="(prefers-color-scheme: dark)" srcset="docs/assets/logo-dark.png">
    <img src="docs/assets/logo-light.png" alt="Tabby" width="440">
  </picture>
</p>

<h3 align="center">Navegación con teclado para Mission Control de macOS</h3>

<p align="center">
  <img alt="macOS 14+" src="https://img.shields.io/badge/macOS-14%2B-111111?logo=apple&logoColor=white">
  <img alt="Swift 6" src="https://img.shields.io/badge/Swift-6-F05138?logo=swift&logoColor=white">
  <img alt="Free" src="https://img.shields.io/badge/price-free-2EA44F">
  <img alt="Status: alpha" src="https://img.shields.io/badge/status-alpha-F59E0B">
</p>

<p align="center">
  <a href="../../releases/latest/download/Tabby.zip"><img alt="Descargar para macOS" src="https://img.shields.io/badge/macOS-Descargar%20Tabby-0A5CFF?style=for-the-badge&logo=apple&logoColor=white"></a>
  <br>
  <sub>Sin instalador: descarga el zip, abre Tabby.app y listo. Universal (Apple Silicon + Intel) · macOS 14+ · <a href="../../releases">todas las versiones</a></sub>
</p>

<!-- Video de demostración: arrastra el .mp4 a un comentario de cualquier issue o pull request de GitHub, copia la URL que genera y pégala aquí en una línea sola. GitHub lo muestra como reproductor. -->

---

> [!NOTE]
> Tabby está en alfa: funciona todos los días en la Mac de su autor, pero puede tener detalles. Los reportes de errores son muy bienvenidos.

> [!TIP]
> **Tus atajos siguen siendo tuyos.** Tabby solo toma Tab, Enter y <kbd>⌘</kbd><kbd>1</kbd>…<kbd>⌘</kbd><kbd>9</kbd> mientras Mission Control está abierto, así que Safari, Chrome y el Finder conservan los suyos. <kbd>⌘</kbd><kbd>Tab</kbd> es de Tabby solo mientras el selector de ventanas está activado (se puede apagar en Settings), y <kbd>⌘</kbd><kbd>Q</kbd> cierra una sola ventana solo mientras ese selector está en pantalla.

## ¿Qué es Tabby?

Mission Control muestra todas tus ventanas abiertas de un vistazo, pero para elegir una todavía tienes que ir al mouse o al trackpad. **Tabby te permite hacerlo con el teclado**, igual que con ⌘Tab.

<p align="center">
  <kbd>⌃</kbd> <kbd>↑</kbd> &nbsp;➜&nbsp; <kbd>Tab</kbd> <kbd>Tab</kbd> &nbsp;➜&nbsp; <kbd>Enter ↩</kbd>
  <br>
  <sub><kbd>Tab</kbd> &nbsp;➜&nbsp; <kbd>⌘</kbd> <kbd>2</kbd> &nbsp;manda la ventana seleccionada al Escritorio 2</sub>
</p>

1. **Abre Mission Control** como siempre: atajo de teclado, F3, gesto del trackpad o esquina activa.
2. **Presiona <kbd>Tab</kbd>** para recorrer tus ventanas, empezando por la más reciente. <kbd>⇧</kbd> <kbd>Tab</kbd> vuelve atrás.
3. **Presiona <kbd>Enter ↩</kbd>**: Mission Control se cierra y esa ventana exacta pasa al frente.
4. **O presiona <kbd>⌘</kbd> + un número**: <kbd>⌘</kbd><kbd>1</kbd>…<kbd>⌘</kbd><kbd>9</kbd> manda la ventana seleccionada a ese escritorio y, si no existe, lo crea. Mission Control sigue abierto, así sigues ordenando.

Tabby no reemplaza Mission Control: funciona encima del nativo. Fuera de Mission Control, también toma <kbd>⌘</kbd><kbd>Tab</kbd> para mostrar todas tus ventanas una por una, como en Windows, incluidas las minimizadas y las de otros escritorios, y <kbd>⌘</kbd><kbd>Q</kbd> cierra solo la ventana seleccionada. Esa parte se puede desactivar en Settings.

## Funciones

| | |
|---|---|
| ⌨️ **Primero el teclado** | Tab, ⇧Tab y Enter dentro de Mission Control, empezando por la ventana más reciente. |
| 🎯 **La ventana exacta** | Enfoca la ventana que elegiste, aunque haya varias de la misma app. |
| ✨ **Sabes dónde estás** | La ventana seleccionada se levanta un poco con un resorte suave y vuelve a su lugar al pasar a otra. |
| 🗂️ **Mándala a un escritorio** | <kbd>⌘</kbd><kbd>1</kbd>…<kbd>⌘</kbd><kbd>9</kbd> mueve la ventana seleccionada a ese escritorio y, si todavía no existe, lo crea. Solo dentro de Mission Control: en cualquier otro lado ⌘1…⌘9 siguen funcionando como siempre. |
| 🪟 **⌘Tab, ventana por ventana** | El selector de apps de Tabby muestra ventanas, no apps. Mantén ⌘, presiona Tab, suelta para cambiar. <kbd>⌘</kbd><kbd>Q</kbd> cierra solo la ventana seleccionada mientras el selector está abierto; en cualquier otro momento cierra apps como siempre. Desactívalo en Settings si prefieres el estándar. |
| ⚙️ **Tus atajos** | Cambia cualquier atajo en **Settings**. |
| 🪄 **Como sea que lo abras** | Atajo, F3, gesto o esquina activa: Tabby no depende de ninguno. |
| 🍎 **Nativa** | Swift, SwiftUI y AppKit. Una app mínima en la barra de menús que no estorba. |
| 🔒 **Privada** | Sin analíticas y sin cuentas. Solo escucha el teclado mientras Mission Control está abierto, y lo único que consulta por red es si hay una versión nueva (opcional). |
| 💸 **Gratis** | Gratis para todos, uso personal y comercial. Sin cuentas ni suscripciones. |

## Hoja de ruta

- [x] **Spike 0:** validar las capacidades de macOS que necesita Tabby
- [x] **Mission Control con el teclado:** Tab, ⇧Tab y Enter, efecto de agrandar, cambio de escritorio, Configuración y bienvenida
- [x] **Mover la ventana seleccionada a otro escritorio** con ⌘1…⌘9
- [x] **⌘Tab ventana por ventana**, con ⌘Q cerrando solo la ventana seleccionada (0.1.0-alpha.7)
- [x] **Mover a Aplicaciones** desde la bienvenida (0.1.0-alpha.6)
- [ ] **v0.1.0:** primera versión estable, después de una ronda de uso real
- [ ] Navegación con flechas según la posición de las miniaturas
- [ ] Atajos numéricos (1–9) y búsqueda de ventanas
- [ ] Extras del selector: atajo configurable (⌥Tab), ⌘` para las ventanas de la misma app

## Descarga

Tabby es una sola descarga, sin instalador. Usa el botón **Download** de arriba, o:

1. Descarga [**Tabby.zip**](../../releases/latest/download/Tabby.zip) de la última versión y ábrelo para descomprimir **Tabby.app**.
2. Arrastra **Tabby.app** a la carpeta **Aplicaciones**. También funciona desde Descargas, pero *Abrir al iniciar sesión* necesita que esté en Aplicaciones.
3. Abre **Tabby.app**.

### La primera vez, macOS la bloquea

Tabby es gratis y no está notarizada por Apple, porque eso requiere una cuenta paga de desarrollador. Por eso, la primera vez que la abres, macOS avisa que Apple no pudo verificar que Tabby no contenga software malicioso y ofrece mandarla a la papelera. Tabby es segura y su código es abierto, así que:

1. Haz clic en **Listo**. No la mandes a la papelera.
2. Abre **Configuración del Sistema → Privacidad y seguridad** y baja hasta **Seguridad**. Vas a ver *Se bloqueó "Tabby" para proteger tu Mac.*
3. Haz clic en **Abrir de todos modos**.
4. macOS vuelve a preguntar: haz clic en **Abrir de todos modos**.
5. Escribe tu contraseña o usa Touch ID. **En una Mac con Touch ID, apoya el dedo en el sensor aunque no veas ningún diálogo:** el pedido puede esperar en silencio, sobre todo con un monitor externo. Si no, mira tu otra pantalla.
6. **Si el ícono de Tabby no aparece en la barra de menús después de unos segundos, cierra la copia trabada y vuelve a abrir Tabby.** La copia que abriste antes de aprobar queda congelada, y macOS manda cada doble clic nuevo a esa copia. Abre el **Monitor de Actividad**, selecciona **Tabby**, haz clic en **ⓧ** → **Forzar salida**, y abre Tabby otra vez. Tu aprobación ya quedó guardada, así que esta vez arranca al instante. (Terminal: `pkill -9 Tabby; open ~/Downloads/Tabby.app`.)

Tabby se abre, su ícono aparece en la barra de menús y una bienvenida corta te guía con el permiso de **Accesibilidad** y una primera prueba. Esto se hace una sola vez, aunque una versión nueva descargada de internet puede volver a pedirlo.

## Problemas frecuentes

**macOS dice que no pudo verificar Tabby.** Es lo esperable: Tabby no está notarizada por Apple. Haz clic en **Listo** y sigue los pasos de arriba (Privacidad y seguridad → Abrir de todos modos).

**Hice clic en «Abrir de todos modos» y no pasa nada. El Monitor de Actividad muestra a Tabby con 0 % de CPU.** macOS está esperando tu aprobación y el pedido puede ser silencioso: en una Mac con Touch ID, apoya el dedo en el sensor; con un monitor externo, mira la otra pantalla. Si sigue trabada, la copia que abriste antes de aprobar quedó congelada: fuerza la salida de Tabby en el **Monitor de Actividad** y ábrela otra vez; tu aprobación ya quedó guardada. En la Terminal: `pkill -9 Tabby; open ~/Downloads/Tabby.app`. Si aun así no arranca, el propio servicio de Gatekeeper se trabó: ejecuta `sudo killall syspolicyd` en la Terminal y abre Tabby de nuevo.

**Hago doble clic en Tabby y no pasa nada.** Misma causa: una copia congelada se queda con cada clic. Fuérzala a salir y abre Tabby otra vez.

**No aparece «Abrir de todos modos».** El botón está solo durante una hora, más o menos, después de que macOS bloquea Tabby. Vuelve a abrir Tabby para que macOS la bloquee y entra otra vez a Privacidad y seguridad.

**Tabby está en la barra de menús, pero en Mission Control no pasa nada.** Tabby necesita el permiso de Accesibilidad. **Settings → General** muestra si está concedido; concédelo en **Configuración del Sistema → Privacidad y seguridad → Accesibilidad**. Si Tabby figura ahí y aun así no funciona (pasa al reemplazar la app), apaga y vuelve a encender su interruptor. **Diagnostics…** en el menú muestra exactamente qué ve Tabby.

**⌘Tab sigue mostrando el selector de apps estándar.** Revisa que **Settings → General → «⌘Tab shows windows, not apps»** esté activado, que Tabby esté habilitada y que tenga Accesibilidad (el selector usa el mismo acceso al teclado que Mission Control). Dentro de Mission Control, ⌘Tab sigue siendo nativo a propósito. En campos de contraseña (Secure Input) macOS bloquea cualquier herramienta de teclado, Tabby incluida.

**La ventana seleccionada no se agranda, o ⌘Tab muestra íconos en vez de miniaturas.** Las dos cosas necesitan el permiso opcional de Grabación de pantalla: **Settings → General → Allow Screen Recording**. Sin él, Tabby funciona con un recuadro simple e íconos de app.

**«Launch at login» aparece deshabilitado.** Tabby está corriendo desde Descargas u otra carpeta. Usa **Settings → General → Move to Applications**, o arrastra Tabby.app a Aplicaciones con el Finder y ábrela otra vez.

**⌘1…⌘9 dice que la ventana está en todos los escritorios.** Esa app está asignada a todos los escritorios en macOS: clic derecho en su ícono del Dock → **Opciones → Asignar a → Ninguno**.

**Cambié de escritorio dentro de Mission Control y la lista se vio mal un instante.** Tabby espera a que macOS termine el cambio (alrededor de un segundo) antes de rearmar la lista; las teclas que presiones mientras tanto se aplican cuando está lista. Si queda mal, abre un issue con el reporte de Diagnóstico.

**Tabby pidió aprobación otra vez después de una actualización.** Cada descarga pasa por Gatekeeper una vez. Los permisos se conservan, porque todas las versiones van firmadas con el mismo certificado. En una Mac que nunca muestra el pedido de aprobación, puedes saltar Gatekeeper para la copia nueva antes de abrirla: `find ~/Downloads/Tabby.app -print0 | xargs -0 xattr -d com.apple.quarantine`.

**Tienes varias copias de Tabby.** Deja solo la de Aplicaciones y borra las demás, también el zip, así siempre abres la misma.

**¿Cómo reporto un problema?** Abre un [reporte de error](../../issues/new/choose) y pega el reporte de Diagnóstico (**Diagnostics…** en el menú → **Copy Report**). Incluye lo que cambia el comportamiento de Mission Control: tu versión de macOS, tus pantallas y si tienen espacios separados. No tiene títulos de ventanas, teclas ni datos personales.

## Privacidad

macOS exige el permiso de Accesibilidad a las apps que detectan Mission Control, leen información de las ventanas y enfocan ventanas de otras apps. Tabby lo usa solo para eso:

- Solo escucha el teclado mientras Mission Control está abierto, más ⌘Tab (y las teclas que le siguen) mientras el selector de ventanas está activado.
- Nunca guarda ni envía lo que escribes.
- No tiene analíticas ni cuentas. Lo único que hace por red es buscar versiones nuevas: al abrirse y cada 12 horas lee la última versión publicada en GitHub. No se envía nada sobre ti, y se puede desactivar en Settings.
- **Grabación de pantalla es opcional** y solo se usa para el efecto de agrandar. Tabby captura las ventanas de la pantalla actual mientras Mission Control está abierto, guarda las imágenes en memoria y las descarta al cerrarlo. No se guarda ni se envía nada. Sin ese permiso, Tabby funciona igual con un recuadro simple.
- **Diagnostics…** en el menú muestra exactamente qué permisos tiene Tabby y qué detecta, y su reporte no tiene datos personales.

## Requisitos

macOS 14 Sonoma o posterior · Apple Silicon o Intel

## Comentarios y errores

Si algo no funciona, abre **Diagnostics…** en el menú, haz clic en **Copy Report** y pégalo en un [issue nuevo](../../issues/new). El reporte no tiene títulos de ventanas, teclas ni datos personales.

## Apoya a Tabby

Tabby es gratis para todos, hecho con ❤️ en Argentina 🇦🇷. Si te ahorra tiempo todos los días, puedes invitarme un café: cada aporte ayuda a sumar funciones y a mantener Tabby al día con cada macOS nuevo.

- Alias de **Mercado Pago** (Argentina): `cristiandjr.mp`
- **USDT** por la red Tron (TRC20), desde cualquier país: `TFUMsNxJGjum96MKHLfwabf8MTxpVuZLBx` — envía solo USDT por TRC20 a esta dirección.
- Dejar una ⭐ en el repo y compartir Tabby con alguien también ayuda muchísimo.

## Licencia

Tabby es gratis para descargar y usar, con fines personales y comerciales, bajo la [Licencia de Tabby](LICENSE). Tabby es software propietario: su código fuente no es público, y el nombre, el logo y el ícono de Tabby pertenecen a su autor. Las versiones hasta la 0.1.0-alpha.4 se publicaron bajo la Licencia MIT, que sigue aplicando solo a esas versiones.
