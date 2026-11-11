# Heart Scanner Patch

Repositorio académico con los avances 1 al 16 del prototipo web, organizado por carpetas y ejecutable sin Node.js ni npm.

## Estructura

- `index.html`: menú principal del repositorio.
- `Avance_01/` a `Avance_16/`: cada avance tiene su propio `index.html`.

## Cómo probar

1. Descarga o clona este repositorio.
2. Abre `index.html` para ver el menú o entra directamente a cualquier carpeta `Avance_XX`.
3. Abre el archivo `index.html` de ese avance con Chrome, Edge o Firefox.
4. Para avances que guardan información, utiliza el mismo navegador y perfil.

No requiere Node.js, npm ni instalación de dependencias. Puede publicarse con GitHub Pages.

## Avance 11

Incluye exportación de respaldo JSON, validación de archivo e importación con dos modos: agregar registros sin duplicados exactos o reemplazar la lista actual. Usa la clave local `heartScannerPatchAvance9`, compartida con los avances 9 y 10.

## Limitaciones importantes

- Es un prototipo académico con datos de demostración; no mide signos vitales reales.
- No se conecta a sensores, ESP32, Bluetooth BLE, Firebase ni servicios clínicos.
- El almacenamiento es local al navegador y dispositivo; no es una base de datos en la nube.
- Las alertas y valores son demostrativos y no sirven para diagnosticar ni tomar decisiones médicas.
- El avance 7 incluye elementos PWA que requieren servidor/HTTPS para algunas funciones; el HTML principal se puede abrir localmente.


## Avance 12

Incluye un panel para agregar registros manuales de demostración, consultar el historial, filtrar por paciente o fecha, visualizar los valores en una gráfica, revisar un resumen y exportar los datos filtrados a CSV o imprimirlos. Comparte la clave local `heartScannerPatchAvance9` con los avances 9, 10 y 11.

Los valores son ficticios o ingresados manualmente: no provienen de sensores y no tienen utilidad diagnóstica.


## Avance 13
Incluye seguimiento de pacientes ficticios, búsqueda, resumen y una conexión BLE representada de forma simulada. Los registros de prueba se guardan en el almacenamiento local compartido `heartScannerPatchAvance9`. No se conecta a hardware Bluetooth real.

## Avance 14
Incluye un centro de notificaciones para crear avisos informativos, advertencias y avisos de atención, relacionarlos con un paciente, filtrarlos y marcarlos como revisados. Se guardan localmente con la clave `heartScannerPatchNotificaciones14`.

## Avance 15
Integra en un panel general los registros de seguimiento y las notificaciones de los avances anteriores, con resumen, últimas entradas, exportación CSV e impresión.

Los avances 13, 14 y 15 son páginas HTML independientes y no requieren Node.js ni npm. La conexión BLE es solo una simulación de interfaz.


## Avance 16

Incluye un sistema de reportes que resume los registros del Avance 9/12 y los avisos del Avance 14, con filtros por paciente y periodo, tabla de historial, resumen estadístico, exportación CSV e impresión o guardado como PDF desde el navegador. Se encuentra en `Avance_16/index.html` y también como `Heart_Scanner_Patch_Avance_16.html`. Lee los datos locales mediante las claves `heartScannerPatchAvance9` y `heartScannerPatchNotificaciones14`; no requiere Node.js ni npm.

Los reportes son demostrativos. No presentan mediciones clínicas ni conclusiones médicas. Para ver los mismos datos, abre los avances en el mismo navegador y perfil.
