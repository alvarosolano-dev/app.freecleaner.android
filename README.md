# 🧹 Limpiador

**Una app para Android que te muestra qué está ocupando espacio en tu teléfono y te ayuda a liberarlo.**
Sin publicidad, sin conexión a internet y sin cuentas: un solo propósito, ordenar tu almacenamiento.

!\[Android](https://img.shields.io/badge/Android-8.0%2B-3DDC84?logo=android\&logoColor=white)
!\[Versión](https://img.shields.io/badge/versi%C3%B3n-1.0-7C3AED)
!\[Sin internet](https://img.shields.io/badge/Internet-no%20usa-success)

\---

## ¿Qué hace?

Limpiador tiene cuatro pestañas en la barra inferior:

### 📊 Panel

La pantalla de inicio. Muestra de un vistazo:

* **Espacio utilizado y libre** del almacenamiento interno, en un anillo que cambia de color según qué tan lleno está (violeta → amarillo → rojo).
* **Resumen rápido:** cuánta caché se puede liberar, cuántas actualizaciones de sistema se pueden revertir, cuántas apps tenés instaladas y cuánto pesan tus documentos.
* **Salud del teléfono:** uso de memoria RAM, nivel de batería, temperatura, si está cargando y estado de salud de la batería.
* Modelo del dispositivo y versión de Android.

### 🗂️ Caché

Lista tus apps ordenadas de **mayor a menor caché acumulada** (archivos temporales que se pueden borrar sin perder datos). Tocás una app y te lleva directo a su pantalla de información en los ajustes de Android, donde podés usar *Almacenamiento → Borrar caché*.

### ⬆️ Updates

Encuentra las **apps del sistema que tienen una actualización instalada encima** (Chrome, Google, etc.) y muestra cuánto espacio ocupa cada una. Desde ahí podés desinstalar la actualización para volver a la versión original de fábrica y recuperar espacio.

### 📄 Docs

Escanea el almacenamiento y lista tus **PDF, Word, Excel y PowerPoint del más pesado al más liviano**, con filtros por tipo. Tocás un archivo y podés **abrirlo** con la app que prefieras o **borrarlo** (siempre con confirmación previa).

### 🎨 Extras

* Tema **automático, claro u oscuro** (se cambia con el botón de arriba a la derecha y se recuerda).
* Interfaz limpia con la tipografía [Inter](https://rsms.me/inter/).

\---

## 📸 Capturas

|Panel|Caché|Updates|Docs|
|:-:|:-:|:-:|:-:|
|!\[Panel](screenshots/panel.png)|!\[Caché](screenshots/cache.png)|!\[Updates](screenshots/updates.png)|!\[Docs](screenshots/docs.png)|

\---

## 📲 Instalación

**Requisitos:** teléfono con **Android 8.0 o superior**. La pestaña **Docs** requiere **Android 11 o superior**.

1. Entrá a la sección [**Releases**](../../releases) de este repositorio y descargá el archivo **`app-debug.apk`** (aprox. 3,4 MB).
2. Abrilo desde tu teléfono. Si Android lo pide, habilitá **"Instalar apps de fuentes desconocidas"** para el navegador o administrador de archivos que estés usando.
3. Tocá **Instalar**. Si Google Play Protect muestra una advertencia, es porque la app no viene de Play Store: elegí **"Instalar de todas formas"**.
4. Abrí **Limpiador** y seguí con la sección de permisos.

> ℹ️ Es una versión de prueba (\*debug\*), por eso puede aparecer esa advertencia de seguridad al instalar.

**Para desinstalarla:** mantené presionado el ícono → *Información de la app* → *Desinstalar*.

\---

## 🔑 Permisos

Limpiador necesita tres permisos especiales que **Android no concede automáticamente**: hay que activarlos a mano desde los ajustes. La app te avisa con una tarjeta y un botón que lleva directo a la pantalla correcta.

|Permiso|Para qué se usa|Pestañas que lo necesitan|
|-|-|-|
|**Acceso a datos de uso**|Medir el tamaño y la caché de cada app instalada|Panel, Caché, Updates|
|**Ver todas las apps**|Listar las apps instaladas|Panel, Caché, Updates|
|**Acceso a todos los archivos**|Buscar tus PDF, Word, Excel y PowerPoint|Docs|

**Primer uso:** abrí la app → tocá **Dar permiso** → buscá **Limpiador** en la lista → activalo → volvé atrás.

\---

## 🔒 Privacidad

* **No tiene permiso de internet:** la app no puede enviar nada fuera de tu teléfono.
* **Sin anuncios, analíticas, cuentas ni rastreadores.**
* La copia de seguridad automática de Android está desactivada.
* El escaneo de documentos solo mira **nombres, rutas y tamaños** de archivos PDF, Word, Excel y PowerPoint. No lee su contenido ni toca fotos ni videos.
* La app **no borra nada por sí sola**: la única acción destructiva es borrar un documento, y siempre te pide confirmación.

\---

## ⚠️ Limitaciones

* **La caché no se borra desde la app.** Android no permite que una app común limpie la caché de otras, así que Limpiador te muestra cuánto ocupa cada una y te lleva a la pantalla del sistema donde se borra con un toque.
* **Borrar un documento es permanente:** no hay papelera.
* La lista de **Caché** muestra las 60 apps con más caché y la de **Docs** los 100 archivos más pesados.
* El escaneo de documentos **omite la carpeta `Android/`** (datos internos de otras apps).
* Los tamaños pueden variar levemente según el fabricante y la versión de Android.

\---

## ℹ️ Información de la versión

|||
|-|-|
|Versión|1.0|
|Paquete|`com.limpiador.app`|
|Android mínimo|8.0 (API 26)|
|Optimizada para|Android 14 (API 34)|
|Tamaño|\~3,4 MB|

\---

## 🐞 Reportar problemas

Si algo no funciona, abrí un [issue](../../issues) contándome qué **modelo de teléfono** y qué **versión de Android** usás.

## 📜 Licencia y créditos

Licencia **MIT**. La tipografía **Inter** está bajo la [SIL Open Font License](https://openfontlicense.org/).

\---

<p align="center">Hecho con Android Studio por <a href="https://github.com/solanoalvaro96-bot>

