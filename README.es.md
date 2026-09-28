# ZipMania

**Un compresor gratuito para Windows, rápido y ligero, que abre más de 50 formatos y comprime en 7Z · ZIP · TAR.**

[English](README.md) · [한국어](README.ko.md) · [简体中文](README.zh-CN.md) · [日本語](README.ja.md) · Español · [Português (Brasil)](README.pt-BR.md) · [Français](README.fr.md)

> Este documento es una traducción. Si hay alguna diferencia, prevalece la [versión en coreano](README.ko.md).

![Platform](https://img.shields.io/badge/platform-Windows%2010%20%2F%2011%20x64-0078D4)
![License](https://img.shields.io/badge/license-Freeware-brightgreen)
![Source](https://img.shields.io/badge/source-Apache%202.0-lightgrey)
![Version](https://img.shields.io/badge/version-0.9.9-blue)
[![Download](https://img.shields.io/badge/download-kilho.net-orange)](https://down.kilho.net/zipmania?lang=es)

![Captura de pantalla de ZipMania](images/zipmania-en.webp)

## Descripción general

ZipMania es un compresor centrado en una sola cosa: abrir y crear archivos comprimidos. Lee más de 50 formatos, entre ellos ZIP, RAR, 7Z, EGG, ALZ e ISO, y crea archivos en **7Z · ZIP · TAR**.

Al abrir un archivo comprimido, verás el árbol de carpetas a la izquierda y la lista de archivos a la derecha. Elige solo los archivos que necesitas y extráelos, o arrástralos directamente al Explorador. Las imágenes se previsualizan sin extraer. Haz doble clic en un archivo para abrirlo con su programa asociado, y un archivo comprimido dentro de otro se abre en una ventana nueva.

El menú contextual del Explorador ofrece acciones de un clic como «Extraer aquí» y «Comprimir en *nombre*.zip», y se incluye una herramienta de línea de comandos (`zm.exe`) para scripts de copia de seguridad y programas externos como Total Commander. Sin anuncios ni software adicional.

## Funciones

- **Abre más de 50 formatos** — ZIP, ZIPX, JAR, RAR, 7Z, EGG, ALZ, TAR, GZ, BZ2, XZ, ZST, ISO, IMG, WIM, DMG, MSI, RPM, DEB, CAB, CBZ, CBR y más.
- **Comprime en 7Z · ZIP · TAR** — cinco niveles de compresión, contraseñas, cifrado de nombres de archivo en 7Z, archivos divididos.
- **ZIP rápido** — un motor dedicado se encarga de comprimir y extraer ZIP.
- **Solo lo que necesitas** — extrae los archivos seleccionados, arrástralos al Explorador o ábrelos con doble clic.
- **Archivos dentro de archivos** — doble clic para abrirlos en una ventana nueva.
- **Vista previa de imágenes** — JPG, PNG, GIF, WebP, SVG y más, en el panel inferior izquierdo sin extraer.
- **Edición de archivos** — añade o elimina archivos en 7Z, ZIP y TAR.
- **Verificar · Analizar** — una tabla CRC muestra si el archivo está dañado, y el antivirus de Windows (AMSI) puede analizar los archivos internos.
- **Limpieza tras comprimir** — verifica el archivo al terminar y elimina los originales solo si supera la prueba.
- **Menú contextual del Explorador** — Extraer aquí, Extraer en *nombre*, Comprimir en *nombre*.zip, Comprimir cada uno por separado, Extraer cada uno en su carpeta.
- **Línea de comandos** — `zm.exe` (consola) y `ZipMania.exe` (ventana de progreso) para comprimir, extraer, listar y probar. Acepta la sintaxis de opciones de 7-Zip y de Bandizip.
- **Tema claro/oscuro, 9 idiomas** — sigue a Windows por defecto, o elige el tuyo.

## Descarga / Instalación

| Paquete | Enlace |
|---|---|
| Instalador | [Descargar](https://down.kilho.net/zipmania?lang=es) |
| Portátil (ZIP) | [Descargar](https://down.kilho.net/zipmania?lang=es&nosetup) |

ZipMania puede usarse como aplicación portátil: descomprime en cualquier lugar y ejecuta `ZipMania.exe`. La configuración se guarda en `settings.toml` junto al ejecutable, así que viaja contigo en una memoria USB.

## Uso

### Flujo básico

**Extraer**

1. Haz doble clic en un archivo comprimido, ábrelo con **[Abrir]** en ZipMania o suéltalo en la ventana.
2. Revisa el árbol de carpetas a la izquierda y la lista de archivos a la derecha. Selecciona archivos y pulsa **[Extraer]**.
3. En la ventana **Extraer**, elige la carpeta de destino. Usa los accesos rápidos de la izquierda (Escritorio, Documentos, Descargas…) o el árbol de carpetas; haz clic derecho en un espacio vacío para crear una carpeta nueva.
4. En **Archivos a extraer** elige **Todos los archivos** o **Archivos seleccionados** y pulsa **[Aceptar]**. Se muestran el progreso, la velocidad y el tiempo restante; al terminar, **[Abrir carpeta]** te lleva al resultado.

**Comprimir**

1. Pulsa **[Nuevo archivo]** en la barra de herramientas o suelta archivos y carpetas en la ventana de ZipMania.
2. La ventana **Nuevo archivo** los lista. Añade más con **[Añadir archivos]** / **[Añadir carpetas]** o arrastrándolos.
3. Define el **Nombre de archivo** (ubicación), el **Formato** (7Z · ZIP · TAR) y, si hace falta, **Establecer contraseña**, **Dividir**, las acciones de **Después** y el **Método**.
4. Pulsa **[Iniciar]**. Al terminar, **[Abrir carpeta]** o **[Cerrar]**.

Para hacerlo directamente desde el Explorador, usa el menú contextual — consulta «Cómo…» más abajo.

### La ventana

| Botón de la barra | Qué hace |
|---|---|
| **Abrir** | Abrir un archivo comprimido |
| **Extraer** | Extraer el archivo abierto (o solo los archivos seleccionados) |
| **Nuevo archivo** | Elegir archivos y carpetas y crear un archivo nuevo |
| **Añadir archivos** / **Eliminar archivos** | Meter o quitar archivos del archivo abierto (solo 7Z · ZIP · TAR) |
| **Verificar** | Comprobar si el archivo está dañado (CRC) |
| **Analizar** | Analizar los archivos internos con el antivirus de Windows (archivos de menos de 10 MB) |
| **Vista plana** | Mostrar todos los archivos en una sola lista con su ruta completa, sin carpetas |
| **Configuración** | Tema, idioma, valores de extracción, asociaciones de archivos, menú del Explorador |

- **Árbol de carpetas (arriba a la izquierda)** — haz clic en una carpeta para ver sus archivos a la derecha.
- **Vista previa (abajo a la izquierda)** — aparece al seleccionar un único archivo de imagen.
- **Lista de archivos** — Nombre · Tamaño · Tamaño comprimido · Tipo · Modificado. Haz clic en la cabecera Nombre, Tamaño o Modificado para ordenar; arrastra los bordes para cambiar el ancho de las columnas.
- **Barra de estado** — número de elementos, cantidad y tamaño de los archivos seleccionados, tamaño comprimido y ratio.
- Arrastra el separador para cambiar el ancho del árbol y la lista. El tamaño de la ventana y el estado maximizado se restauran la próxima vez.

### Cómo…

**Extraer directamente desde el Explorador**
Haz clic derecho en un archivo comprimido para ver las entradas de ZipMania.
- **Extraer aquí** — extrae en la carpeta del propio archivo sin preguntar. Activa **Cerrar ventana** en la ventana de progreso para que se cierre en cuanto termine.
- **Extraer en «nombre»** — crea una carpeta nueva con el nombre del archivo y extrae dentro. Ideal para archivos con muchos elementos.
- **Extraer con ZipMania…** — abre la ventana donde eliges el destino y las opciones.
- **Abrir con ZipMania** — mira primero el contenido.

Con **varios archivos seleccionados**, **Extraer aquí** los extrae uno tras otro, y **Extraer cada uno en su carpeta** coloca cada archivo en una carpeta con su propio nombre.

**Comprimir directamente desde el Explorador**
Haz clic derecho en archivos o carpetas.
- **Comprimir en «nombre.zip»** — crea un ZIP ahí mismo sin preguntar. Una carpeta toma el nombre de la carpeta; varios elementos toman el nombre de la carpeta actual. Si el nombre ya existe, se añade un número: `nombre (2).zip`.
- **Comprimir con ZipMania** — abre la ventana para elegir formato, contraseña, división, etc.
- **Comprimir cada uno por separado** — crea un ZIP por cada elemento seleccionado, con su nombre. Práctico para archivar varias carpetas por separado.

**Sacar solo unos pocos archivos de un archivo comprimido**
Tres formas:
- Selecciona los archivos (Ctrl/Mayús para varios) y pulsa **[Extraer]** → **Archivos a extraer: Archivos seleccionados**.
- Clic derecho en la selección → **Extraer archivos seleccionados**.
- **Arrastra la selección al Explorador o al escritorio** — se extrae ahí mismo.

**Abrir un archivo interno sin extraer**
Haz doble clic o pulsa Intro; se abre con su programa asociado (los documentos en tu editor, los vídeos en tu reproductor). Clic derecho → **Ejecutar archivo** hace lo mismo. Las copias temporales se limpian al cerrar ZipMania.

**Un archivo comprimido dentro de otro**
Haz doble clic y se abre en una **ventana nueva**. Puedes mantener varias ventanas abiertas y alternar entre ellas.

**Hojear fotos dentro de un archivo**
Selecciona un archivo de imagen (JPG · PNG · GIF · BMP · WebP · ICO · SVG · TIFF · AVIF) y aparece una vista previa abajo a la izquierda. Usa las flechas para recorrerlas. Las imágenes de más de 32 MB muestran un aviso en lugar de la vista previa.

**Las carpetas profundas dificultan encontrar archivos**
Activa **[Vista plana]** en la barra: las carpetas desaparecen y cada archivo se lista con su ruta. Ordena por nombre, tamaño o fecha para encontrar de inmediato los archivos más grandes o más recientes. Pulsa de nuevo para volver a la vista de carpetas.

**Archivos protegidos con contraseña**
Al abrirlos aparece un cuadro de contraseña. Una contraseña incorrecta vuelve a preguntar; una correcta se recuerda para ese archivo, así que vista previa, apertura y extracción no vuelven a pedirla. Si durante la extracción aparece un archivo protegido, se pregunta en ese momento; si lo dejas en blanco, solo se omite ese archivo y el resto continúa.

**Comprimir con contraseña**
En la ventana **Nuevo archivo** pulsa **[Establecer contraseña]** y escríbela.
- Con **7Z** también puedes activar **Cifrar nombres de archivo** — sin la contraseña nadie puede ver siquiera qué hay dentro.
- **ZIP** solo acepta letras y dígitos. Una contraseña no ASCII muestra un aviso y no arranca — cambia a 7Z o usa una contraseña ASCII.
- **TAR** no admite contraseñas.

**Enviar un archivo grande por correo o mensajería**
En **Dividir** elige 10 MB · 25 MB · 100 MB · 700 MB · 1 GB · 4 GB, o elige **Personalizado…** y escribe algo como `700M` o `4GB`. El archivo se guarda como `nombre.7z.001`, `.002`, … (7Z · ZIP). Quien lo recibe pone las partes en una carpeta y abre o extrae **solo el archivo `.001`**.

**Borrar los originales tras comprimir para liberar espacio**
En **Después** activa **Verificar archivo** y **Eliminar originales**. Los originales se eliminan solo cuando todos los archivos se guardaron y la verificación se superó, así que un archivo defectuoso nunca te costará los originales.

**Comprimir varias carpetas por separado**
Pon las carpetas en la ventana **Nuevo archivo** y activa **Comprimir cada elemento en su propio archivo**. Cada carpeta obtiene un archivo con su nombre, junto a ella. Es lo mismo que **Comprimir cada uno por separado** del Explorador, pero aquí puedes elegir también el formato y una contraseña.

**Más rápido o más pequeño**
**Método** tiene cinco niveles: **Almacenar (sin compresión)** · **Rápido** · **Normal** · **Alto** · **Máximo**. Para simplemente agrupar fotos o vídeos ya comprimidos, **Almacenar** es lo más rápido; para documentos y código fuente, que se reducen bien, **Alto** o **Máximo** compensan. Para el resultado más pequeño usa el formato **7Z** (el predeterminado).

**Añadir o quitar archivos de un archivo existente**
Con un archivo 7Z · ZIP · TAR abierto:
- Pulsa **[Añadir archivos]** o suelta archivos en la ventana — responde Sí a «¿Añadir N archivo(s) a …?».
- Selecciona archivos y pulsa **[Eliminar archivos]** o clic derecho → **Eliminar archivos**.
Los demás formatos (RAR, EGG, …) no se pueden editar, por lo que los botones aparecen desactivados.

**Comprobar si un archivo descargado está intacto**
Pulsa **[Verificar]**: se comparan el CRC esperado y el real de cada archivo y se muestran en una tabla. Los archivos dañados o descargados parcialmente se detectan antes de extraerlos.

**Comprobar si un archivo descargado es seguro**
**[Analizar]** entrega los archivos internos al antivirus de Windows (AMSI) sin extraerlos. Los archivos de 10 MB o más se omiten, y debe haber un antivirus con protección en tiempo real activa. El resultado muestra cada archivo como Limpio · Amenaza · Omitido.

**Ya existe un archivo con el mismo nombre al extraer**
Se pregunta por cada archivo: **Sobrescribir** · **Omitir** · **Renombrar**. Activa **Aplicar a todos los archivos restantes** para usar la misma respuesta con el resto.

**La extracción dispersó archivos por toda la carpeta**
**Crear una subcarpeta con el nombre del archivo** está activado por defecto, así que los archivos van a una carpeta con el nombre del archivo comprimido. Para extraer directamente, desactívalo en la ventana **Extraer** o en **Configuración → Extracción**, o usa **Extraer aquí** del Explorador.

**Borrar el archivo y abrir la carpeta al terminar**
En **Configuración → Extracción** activa **Eliminar el archivo tras una extracción correcta**, **Abrir la carpeta de destino tras extraer** y **Cerrar la ventana de extracción tras extraer**. También se pueden cambiar en la ventana Extraer cada vez. El archivo se elimina solo si la extracción fue correcta.

**Hacer que el doble clic abra los archivos en ZipMania**
Marca las extensiones en **Configuración → Asociación de archivos**. Si otro programa ya posee una extensión, se muestra **[No aplicado]**; haz clic para abrir el selector de aplicaciones predeterminadas de Windows y elegir ZipMania. Cuando ZipMania abre un archivo y muestra arriba «¿Hacer de ZipMania la aplicación predeterminada para los archivos …?», puedes cambiarlo ahí mismo.

**ZipMania no aparece en el menú contextual**
En **Configuración → Menú del Explorador** activa **Añadir comprimir/extraer de ZipMania al menú contextual del Explorador**. En Windows 11 aparece en el menú principal; si no lo ves, busca en **Mostrar más opciones** (Mayús+F10).

**Abrir la carpeta del archivo / eliminar el archivo**
Haz clic derecho en un espacio vacío de la lista para **Abrir carpeta contenedora** y **Eliminar archivo**. Tras revisar el contenido, puedes borrar un archivo que ya no necesitas sin salir de ZipMania.

**Manejar la lista con el teclado**
Flechas · Re Pág/Av Pág · Inicio/Fin para moverte, Mayús para un rango, Ctrl+clic para añadir elementos sueltos, **Ctrl+A** para seleccionar todo, Intro para entrar en una carpeta o abrir un archivo, Esc para cerrar el cuadro de contraseña o de informe.

**Modo oscuro e idioma**
Ambos siguen a Windows por defecto. En **Configuración → General** elige el tema (Sistema · Claro · Oscuro) y el idioma (한국어 · English · 日本語 · 中文 · Русский · Italiano · Français · Español · العربية); los cambios se aplican al instante. El menú del Explorador usa el mismo idioma.

**Scripts de copia de seguridad y Total Commander**
Se incluyen dos ejecutables.
- **`zm.exe`** — escribe en la consola. cmd, PowerShell y los archivos por lotes esperan a que termine y reciben un código de salida (0 correcto / 1 aviso / 2 error).
- **`ZipMania.exe`** — ejecuta los mismos comandos con una **ventana de progreso**. Adecuado para entornos sin consola, como Total Commander.

```
<exe> a|c [opciones] <archivo> <entradas...>   comprimir (a añade a un archivo existente)
<exe> x|e [opciones] <archivo> [elementos...]  extraer (x conserva carpetas, e solo archivos)
<exe> bx  [opciones] <archivos...>             extraer cada archivo en una carpeta con su nombre
<exe> l   [opciones] <archivo>                 listar
<exe> t   [opciones] <archivo>                 prueba de integridad
```

| Opción | Significado |
|---|---|
| `-l:0..9` / `-mx9` | Nivel de compresión |
| `-fmt:zip\|7z\|tar` / `-t7z` | Formato (por defecto, según la extensión) |
| `-v:700M` / `-v700m` | Tamaño de volumen |
| `-p:contraseña` / `-pcontraseña` | Contraseña |
| `-o:carpeta` / `-ocarpeta` | Carpeta de destino |
| `-target:auto\|name\|none` | Extraer en una subcarpeta con el nombre del archivo (`auto` = solo si hay más de un elemento de nivel superior) |
| `-aoa` `-y` / `-aos` / `-aou` | Si el nombre coincide: sobrescribir / omitir / guardar como `nombre (2)` |
| `-testdst` | Verificar el archivo tras comprimir |
| `-delsrc` / `-sdel` | Eliminar los originales si la verificación se supera |
| `-date` | Sustituir `%Y %y %m %d %H %M %S` en el nombre por la hora actual |

Ejemplos:

```
zm c -l:9 -fmt:7z -testdst -delsrc -date "backup_%y%m%d_%H%M.7z" "D:\Work"   copia 7Z con fecha, verificar y borrar originales
zm a -mx9 -psecret backup.7z D:\Work                                       sintaxis 7-Zip, añadir a un archivo existente
zm x -o:D:\Out -target:auto backup.7z                                      extraer en una carpeta con el nombre del archivo
zm bx a.zip b.7z                                                            extraer en a\ y b\ respectivamente
zm l backup.7z.001                                                          listar la primera parte de un archivo dividido
```

Ejecuta `zm` sin argumentos para ver la ayuda. Dentro de un archivo por lotes escribe `%` como `%%`. Para un comando de usuario de Total Commander, pon como comando `zm.exe` y como parámetros `c -l:9 -fmt:7z -aou -testdst -delsrc -date "%T%S %y%m%d_%H%M".7z "%P%S"` para comprimir los elementos seleccionados en un 7Z con fecha en la carpeta del panel opuesto.

## Configuración

Todo se cambia en **Configuración** (botón más a la derecha de la barra) y se guarda de inmediato. **[Restablecer]** devuelve todos los valores predeterminados.

| Categoría | Elemento | Predeterminado |
|---|---|---|
| General | Tema (Sistema · Claro · Oscuro) | Sistema |
| General | Idioma (Sistema + 9 idiomas) | Sistema |
| Extracción | Crear una subcarpeta con el nombre del archivo | Activado |
| Extracción | Eliminar el archivo tras una extracción correcta | Desactivado |
| Extracción | Abrir la carpeta de destino tras extraer | Desactivado |
| Extracción | Cerrar la ventana de extracción tras extraer | Desactivado |
| Asociación de archivos | Extensiones que se abren en ZipMania con doble clic (zip · 7z · rar · tar · gz · tgz · bz2 · xz · egg · alz · cbz) | Asociadas por el instalador |
| Menú del Explorador | Añadir comprimir/extraer de ZipMania al menú contextual del Explorador | Activado por el instalador |

Las casillas **Cerrar ventana** y **Abrir carpeta** de las ventanas Nuevo archivo y Extraer recuerdan tu última elección.

## Requisitos

- Windows 10 o Windows 11, **64 bits**
- No se necesita ningún runtime ni componente adicional.
- Internet se usa solo para comprobar si hay una versión nueva. Comprimir y extraer funciona sin conexión.

## Actualizaciones

ZipMania **no** se actualiza solo. Al iniciarse comprueba si hay una versión nueva y solo te avisa; las versiones nuevas se publican manualmente tras una verificación interna y se anuncian en la [página de ZipMania](https://kilho.net/zipmania). Consulta el [aviso sobre la política de actualizaciones](https://en.kilho.net/archives/notice/2940).

**Historial de versiones**

| Versión | Fecha | Notas |
|---|---|---|
| 0.9.9 | 2026-09-21 | Reconstruido sobre su propio motor gráfico — inicio e interfaz unas 9 veces más rápidos, funciona sin componentes adicionales, corrige problemas de inicio y retrasos de la interfaz en algunos entornos |
| 0.9.8 | 2026-09-18 | Renovación de la línea de comandos — opciones compatibles con 7-Zip/Bandizip, nuevo `zm.exe`, comandos de extraer/listar/probar, verificar y eliminar originales tras comprimir, añadir a archivos existentes, extraer cada uno en su carpeta, elección de sobrescribir/omitir/renombrar, progreso, velocidad y tiempo restante |
| 0.9.6 | 2026-09-16 | Archivos divididos, abrir archivos divididos desde la primera parte, compresión silenciosa desde programas externos, sin archivos incompletos tras cancelar o fallar |
| 0.9.5 | 2026-09-10 | Menú del Explorador más fiable, progreso con recuento de fallos y faltantes, abrir la carpeta de resultado al terminar, navegación de carpetas más sencilla |

## Compilar desde el código fuente

El código es público en [github.com/newkilho/ZipMania](https://github.com/newkilho/ZipMania) (Rust 1.88 o superior). El motor de archivos, `crates/zipmania-archive`, se compila y prueba solo con el repositorio:

```
cargo test -p zipmania-archive
```

La aplicación (`app/`) depende de un motor gráfico propio y de bibliotecas compartidas externas al repositorio, por lo que el ejecutable no puede compilarse solo con el repositorio.

## Contribuir

Los informes de errores y las sugerencias son bienvenidos mediante GitHub Issues o el [foro](https://groups.google.com/g/kilhonet).

## Licencia

El programa ZipMania es **Freeware**. Úsalo donde quieras — en casa, en el trabajo, en escuelas y en organismos públicos — y redistribúyelo libremente sin modificar.

El código fuente se publica bajo la **Apache License 2.0**; los crates reutilizables de `crates/` están disponibles bajo MIT o Apache-2.0, a tu elección. Los nombres «ZipMania» y «집매니아» y los logotipos e iconos son marcas de Kilho.net y no están cubiertos por la licencia — distribuye las versiones modificadas con otro nombre e icono. Los componentes de código abierto, incluido `7z.dll` de 7-Zip (LGPL), figuran en `THIRD-PARTY-NOTICES.txt` en el repositorio.

## Enlaces

- Sitio web: <https://kilho.net/zipmania>
- Código fuente: <https://github.com/newkilho/ZipMania>
- Foro: <https://groups.google.com/g/kilhonet>
- X (Twitter): <https://www.twitter.com/kilhonet>

© KILHO.NET
