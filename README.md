# VerbFlow Pro

Aplicación de escritorio para aprender verbos en inglés — Ubuntu / Debian.

Rota verbos automáticamente, muestra conjugaciones, ejemplos de uso y niveles CEFR.
Al minimizar aparece una mini ventana flotante siempre visible con modo quiz integrado.

---

## Instalación

### Requisitos
- Ubuntu 20.04 o superior (o cualquier distro basada en Debian)
- Arquitectura x86_64 (amd64)

### Pasos

**1. Descarga el instalador**

Ve a [Releases](../../releases/latest) y descarga el archivo
`verbflow-pro_X.Y.Z_amd64.deb`.

O desde la terminal:

```bash
wget https://github.com/vosores/verbflow-releases/releases/latest/download/verbflow-pro_1.0.0_amd64.deb
```

**2. Instala el paquete**

```bash
sudo dpkg -i verbflow-pro_1.0.0_amd64.deb
sudo apt-get install -f
```

El segundo comando resuelve automáticamente cualquier dependencia faltante.

**3. Abre la aplicación**

Busca **VerbFlow Pro** en el menú de aplicaciones, o ejecuta desde terminal:

```bash
verbflowpro
```

---

## Desinstalar

```bash
sudo apt remove verbflow-pro
```

Tu configuración y favoritos en `~/.config/verbflow/` no se eliminan.

---

## Funcionalidades

| Función | Descripción |
|---|---|
| Rotación automática | Cambia de verbo cada N minutos (configurable) |
| Mini ventana flotante | Al minimizar, queda una ventana siempre visible sobre el escritorio |
| Modo Quiz | Pulsa 📝 en la mini ventana para responder preguntas sobre el verbo |
| Transparencia | Controla la opacidad de la mini ventana desde el slider en ajustes |
| Favoritos | Guarda los verbos que más te interesen |
| Estadísticas | Contador de verbos vistos hoy, racha de días y precisión en quiz |
| Pronunciación | Pronuncia el verbo con espeak (opcional) |
| Niveles CEFR | Filtra por nivel A1–C2 |

---

## Problemas comunes

**La app no abre después de instalar**
```bash
sudo apt-get install -f
verbflowpro
```

**No hay sonido al pronunciar**
```bash
sudo apt install espeak
```

**Error de librerías gráficas**
```bash
sudo apt install libxcb-xinerama0 libgl1 libdbus-1-3 libxkbcommon0
```
