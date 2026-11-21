# Minimarket — catálogo y punto de venta para GitHub Pages

Funciona 100 % en GitHub Pages, gratis y sin servidor. El panel de administración
guarda cada cambio directamente en tu repositorio de GitHub.

## Qué incluye

- **Catálogo** (`index.html`): búsqueda por producto, marca, SKU o código, franja de
  marcas que filtra al tocarla, filtro por categoría y orden por precio/nombre,
  y botón de WhatsApp con el producto y la forma de pago.
- **Panel** (`admin.html` o `/admin`): productos (con costo privado, precio, código de
  barras y stock), marcas, clientes, proveedores, compras, caja (efectivo y
  transferencia), ventas, devoluciones con vale a favor, descuentos, reportes con
  gráficos, usuarios con permisos (administrador y cajero) y cambio de **usuario y
  contraseña**. Ticket térmico de 80 mm y envío por PDF / WhatsApp / correo.

> Las marcas vienen vacías: cargá las de tu negocio desde **Panel → Marcas**.

## Publicarlo (una sola vez)

### 1. Crear el repositorio
1. Entrá a github.com (creá una cuenta si no tenés).
2. Arriba a la derecha: **+ → New repository**.
3. Nombre: `minimarket` · marcá **Public** · **Create repository**.
4. Tocá **uploading an existing file** y arrastrá **todo el contenido** de esta carpeta
   (las carpetas `assets`, `data`, `img`, `admin` y los archivos sueltos). **Commit changes**.

### 2. Activar GitHub Pages
1. En el repositorio: **Settings → Pages**.
2. En *Branch* elegí **main** y la carpeta **/ (root)** → **Save**.
3. En 1 o 2 minutos aparece tu dirección: `https://TU-USUARIO.github.io/minimarket/`

### 3. Crear el token para el panel
El panel necesita un permiso de GitHub para poder guardar los cambios.
1. En github.com: **Settings (de tu cuenta) → Developer settings → Personal access tokens
   → Fine-grained tokens → Generate new token**.
2. Dale un nombre, elegí tu repositorio `minimarket` y en **Permissions → Contents**
   poné **Read and write**. Generá y **copiá** el token.
3. Entrá a `https://TU-USUARIO.github.io/minimarket/conectar.html`, cargá tu usuario y
   contraseña nuevos, el dueño (tu usuario de GitHub), el repositorio `minimarket` y el token.
   Guardá. ¡Listo! El panel ya guarda directo en GitHub.

> **Cuidá tu token:** no lo compartas ni lo subas al repositorio. Si se filtra,
> borralo desde GitHub y generá uno nuevo.

## Usuario y contraseña de fábrica
`admin` / `admin123` — cambialos apenas entres, desde **conectar.html** o
**Panel → Configuración → Usuarios**.

## Probarlo en tu computadora
Doble clic en `probar_en_mi_pc.py` (o `python probar_en_mi_pc.py`) y se abre
`http://localhost:8000`. El panel queda en `http://localhost:8000/admin.html`.

---
Sistema provisto por **Spycomers** · Tel (0983) 411 544 · www.spynetpy.com
