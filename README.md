# Tecleador de Ventana

Programa gratis para Windows que repite por vos una lista de pasos (escribir texto, apretar teclas, hacer clics y esperar) en la ventana que elijas.

## Descargar

1. Entrá a **[Releases](../../releases/latest)** y bajá `TecleadorDeVentana.exe`.
2. Abrilo con doble clic. No necesita instalación (usa .NET Framework, que ya viene con Windows 10 y 11).

> Windows puede avisar "Windows protegió su PC" porque el programa no está firmado: **Más información → Ejecutar de todas formas**.

## Cómo se usa


**Rutina** (arriba de todo): podés tener varias rutinas con nombre ("Cargar pedidos", "Saludo"…) y elegirlas de la lista. Con **+ Nueva / Duplicar / Renombrar / Borrar** las manejás. Se guardan solas.

**1. Ventana:** elegí de la lista la ventana donde va a trabajar (o escribí una parte del título).

**2. Pasos:** agregalos con los botones de la derecha. Se hacen en orden, de arriba hacia abajo.

| Botón | Qué hace |
|---|---|
| Escribir texto | Escribe el texto tal cual (mayúsculas, ñ, tildes, símbolos). Un renglón nuevo = Enter. |
| Apretar tecla | Enter, Tab, Escape, flechas, F1–F12, letras… solas o con Ctrl / Shift / Alt (ej. Ctrl + V). |
| Clic izquierdo / derecho | Donde esté el mouse, o siempre en el mismo punto. Para elegir el punto: **Capturar posición** y en 3 segundos poné el mouse ahí. |
| Esperar | Una pausa, en segundos (se puede usar 0,5). |

**● Grabar** (lo más fácil): tocalo, hacé los pasos vos una vez en la ventana (clics, texto, teclas) y apretá **F9** para terminar. El programa anota cada clic con su posición, el texto que escribiste (con las correcciones de Borrar ya aplicadas), las teclas especiales y combinaciones (Ctrl + C…), los dobles clics y las pausas de 1 segundo o más. Después podés editar lo grabado.

Con **Subir / Bajar / Editar / Duplicar / Quitar** ordenás la lista. Doble clic en un paso para editarlo.

**3. Ritmo** (todo en segundos):
- **Pausa entre pasos** y **+ al azar hasta**: cada pausa suma un extra al azar, así cada vuelta no es idéntica a la anterior.
- **Repetir X veces** o **Sin fin**, y la pausa entre vueltas.
- **Modo humano**: escribe letra por letra a ritmo irregular y corre unos píxeles los clics fijos.

Después: **▶ Iniciar**.

### Para detenerlo
- Tecla **F9** (funciona aunque el programa esté atrás), o
- el botón **Detener**, o
- llevar el mouse a la **esquina de arriba a la izquierda** de la pantalla (freno de emergencia).

### Protecciones
- Antes de cada paso trae la ventana elegida al frente; si no puede (o se cerró), se detiene para no escribir en otra.
- Si un clic caería sobre otra ventana (algo la tapa o el punto queda afuera), se detiene y avisa.
- Todo se guarda solo y abre en la última rutina usada.

### Opciones para accesos directos
```
TecleadorDeVentana.exe --rutina "Cargar pedidos" --iniciar --salir
```
- `--rutina "nombre"`: abre esa rutina.
- `--config "archivo.txt"`: usa ese archivo en vez de las rutinas (las rutinas están en `%APPDATA%\TecleadorDeVentana\rutinas`).
- `--iniciar`: arranca solo al abrir.
- `--salir`: se cierra al terminar.

## Limitaciones
- Las teclas y clics van a la ventana que está al frente: mientras corre, no uses la PC para otra cosa.
- Algunos juegos con protección (anti-trampas) o programas como administrador pueden ignorar las teclas simuladas.

## Licencia
MIT. by insider
