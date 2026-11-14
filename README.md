# 🍽️ La Querencia - Sistema Integral de Gestión para Restaurantes

<p align="center">
<img width="831" height="591" alt="image" src="https://github.com/user-attachments/assets/233cccfd-ad66-409a-a64a-af7e42466283" />


</p>

<p align="center">
  <strong>Plataforma Web para la Administración Integral de Pedidos, Facturación, Inventarios, Menú, Usuarios y Finanzas de Restaurantes.</strong>
</p>

<p align="center">
  <img src="https://img.shields.io/badge/Python-3.13+-3776AB?style=for-the-badge&logo=python&logoColor=white" alt="Python" />
  <img src="https://img.shields.io/badge/Django-6.0+-092E20?style=for-the-badge&logo=django&logoColor=white" alt="Django" />
  <img src="https://img.shields.io/badge/Django_Ninja-FastAPI_Style-009688?style=for-the-badge&logo=fastapi&logoColor=white" alt="Django Ninja" />
  <img src="https://img.shields.io/badge/React-19.0+-61DAFB?style=for-the-badge&logo=react&logoColor=black" alt="React" />
  <img src="https://img.shields.io/badge/Vite-6.0+-646CFF?style=for-the-badge&logo=vite&logoColor=white" alt="Vite" />
  <img src="https://img.shields.io/badge/PostgreSQL-Database-4169E1?style=for-the-badge&logo=postgresql&logoColor=white" alt="PostgreSQL" />
  <img src="https://img.shields.io/badge/License-MIT-yellow?style=for-the-badge" alt="License" />
</p>

---

## 📋 Tabla de Contenidos

1. [Acerca del Proyecto](#-acerca-del-proyecto)
2. [Características Principales](#-características-principales)
3. [📸 Galería de Módulos y Capturas de Pantalla](#-galería-de-módulos-y-capturas-de-pantalla)
   - [3.1 Módulo de Autenticación y Acceso](#31-módulo-de-autenticación-y-acceso)
   - [3.2 Dashboard de Inicio](#32-dashboard--pantalla-principal)
   - [3.3 Gestión de Usuarios](#33-módulo-de-gestión-de-usuarios)
   - [3.4 Gestión de Caja y Comandas](#34-módulo-de-gestión-de-caja-y-pedidos)
   - [3.5 Gestión de Inventario y Stock](#35-módulo-de-inventario-y-stock)
   - [3.6 Gestión de Menú y Recetas](#36-módulo-de-gestión-de-menú-gastronómico)
   - [3.7 Módulo de Facturación](#37-módulo-de-facturación)
   - [3.8 Pasarela de Pagos (Wompi)](#38-pasarela-de-pagos-en-línea-wompi)
   - [3.9 Configuración, Accesibilidad y Reportes](#39-configuración-accesibilidad-y-reportes)
4. [🛠️ Stack Tecnológico](#️-stack-tecnológico)
5. [⚙️ Requisitos Previos](#️-requisitos-previos)
6. [🚀 Guía de Instalación y Ejecución Local](#-guía-de-instalación-y-ejecución-local)
   - [Backend (Django & Django Ninja)](#1-configuración-del-backend)
   - [Frontend (React + Vite)](#2-configuración-del-frontend)
7. [🔐 Variables de Entorno](#-variables-de-entorno)
8. [📁 Estructura del Repositorio](#-estructura-del-repositorio)
9. [🌐 Documentación de la API (Swagger)](#-documentación-de-la-api)
10. [👥 Autores y Créditos](#-autores-y-créditos)

---

## 📖 Acerca del Proyecto

**La Querencia** es una solución integral diseñada para automatizar y centralizar el flujo operativo, administrativo y financiero de un restaurante o cafetería.

Permite gestionar desde la toma ágil de comandas en salón o a domicilio (con cálculo automático de distancias y costo de flete), pasando por la deducción automática de insumos en inventario mediante recetas, hasta la facturación con cálculo fiscal (IVA), generación de reportes en Excel/PDF e integración con pasarelas de pago digitales (**Wompi**).

Cuenta además con una interfaz moderna y accesible que incluye soporte nativo para **Modo Oscuro/Claro** y corrección visual para **Daltonismo** (Protanopia, Deuteranopia y Tritanopia).

---

## ✨ Características Principales

- 🔐 **Autenticación y Seguridad:** JWT, control de roles (`Administrador` y `Usuario Normal`), validación de fortaleza de contraseñas y token para administradores.
- 📦 **Control de Inventario Multinivel:** Categorización de insumos, directorio de proveedores, registro de órdenes de entrada/compras y descarga de reportes en Excel (`.xlsx`).
- 🍲 **Ingeniería de Menú y Recetas:** Creación de platos gastronómicos asociando insumos específicos y porciones del inventario para control de costos y stock.
- 🛵 **Caja y Domicilios:** Registro de pedidos, clientes frecuentes, estimación de distancia en kilómetros y cobro dinámico de transporte.
- 🧾 **Facturación POS y Fiscal:** Emisión de facturas con desglose de subtotal, IVA configurable (19%), control de efectivo/cambio, tarjeta y consulta histórica.
- 💳 **Pagos Digitales Integrados:** Conexión con pasarela Wompi (Bancolombia) para pagos electrónicos seguros.
- 📊 **Métricas y Reportes:** Indicadores de desempeño (KPIs), ventas acumuladas y productos más vendidos.
- ♿ **Accesibilidad Visual:** Temas Claro/Oscuro, modos para daltonismo y escalado dinámico de tipografía.

---

## 📸 Galería de Módulos y Capturas de Pantalla

> **Nota:** Guarda tus imágenes en `docs/screenshots/` con los nombres de archivo indicados en cada sección.

---

### 3.1 Módulo de Autenticación y Acceso

Control de ingreso con verificación de credenciales, indicador de seguridad de contraseña y protección de privilegios mediante token de administrador.

#### Vista: Inicio de Sesión (Login)
<p align="center">
<img width="1416" height="880" alt="image" src="https://github.com/user-attachments/assets/27c0164c-b415-471a-a2d9-ae79305d918a" />
</p>

*Captura sugerida: Formulario con campos de correo y contraseña, botón de visibilidad de contraseña y enlace a registro.*

---

#### Vista: Registro de Usuarios
<p align="center">
<img width="1164" height="899" alt="image" src="https://github.com/user-attachments/assets/f72cbc16-659c-4e27-92f9-9229345aa5ee" />

</p>

*Captura sugerida: Formulario con campos de DNI, Nombre completo, selector de Rol (Normal / Administrador), token de verificación y medidor de seguridad de contraseña.*

---

### 3.2 Dashboard / Pantalla Principal

Vista de bienvenida al autenticarse en el sistema con información del usuario logueado, su rol y accesos a los módulos.

#### Vista: Panel de Inicio (Home)
<p align="center">
<img width="1346" height="795" alt="image" src="https://github.com/user-attachments/assets/e8974632-2f2c-4210-8f42-3c2f0465a916" />

</p>

*Captura sugerida: Menú de navegación superior activo, banner de bienvenida y tarjeta de perfil del usuario con su rol.*

---

### 3.3 Módulo de Gestión de Usuarios

Panel para la administración del personal de salón, cocina y administradores.

#### Vista: Listado, Búsqueda y Edición de Usuarios
<p align="center">
<img width="1242" height="941" alt="image" src="https://github.com/user-attachments/assets/26e1e6fa-46cd-48e6-a501-3a82dbd26e32" />

</p>

*Funcionalidades mostradas en la captura:*
- Buscador reactivo por nombre o correo electrónico.
- Tabla con DNI, Nombre, Correo, Rol y botones de acción.
- Formulario para crear o actualizar credenciales y roles.
- Modal o confirmación para eliminación segura.

---

### 3.4 Módulo de Gestión de Caja y Pedidos

Punto de venta y despacho de comandas para consumo local o entregas a domicilio.

#### Vista: Creación y Toma de Nuevo Pedido
<p align="center">
<img width="969" height="871" alt="image" src="https://github.com/user-attachments/assets/3eb567d3-b84c-42d4-9dbe-73d949c859d3" />


</p>

*Funcionalidades mostradas en la captura:*
- Selección de clientes registrados o registro de nuevos clientes.
- Formulario de dirección con cálculo de distancia (Km) y flete de envío.
- Selector interactivo de productos con cantidades y agregador al pedido en tiempo real.

---

#### Vista: Historial de Pedidos Activos y Modal de Modificación
<p align="center">
<img width="889" height="727" alt="image" src="https://github.com/user-attachments/assets/74ebe5cb-dd2c-4bdc-9442-ce4a66af24a2" />

</p>

*Captura sugerida: Tabla de pedidos activos con estados (Pendiente, Despachado, Pagado) y ventana modal de edición.*

---

### 3.5 Módulo de Inventario y Stock

Control riguroso de materias primas e insumos para evitar desabastecimientos.

#### Vista: Catálogo de Productos y Niveles de Stock
<p align="center">
<img width="920" height="811" alt="image" src="https://github.com/user-attachments/assets/9459cba6-c52b-4329-a81c-6a8dadcd9b37" />

</p>

---

#### Vista: Gestión de Categorías de Insumos
<p align="center">
<img width="1006" height="723" alt="image" src="https://github.com/user-attachments/assets/6ca7118f-cba0-4bd6-a889-051cf6ea19ec" />

</p>

---

#### Vista: Directorio de Proveedores
<p align="center">
<img width="941" height="806" alt="image" src="https://github.com/user-attachments/assets/5c1f961a-67d8-4096-8094-c697cd5146eb" />

</p>

---

#### Vista: Registro de Entradas y Compras de Mercancía
<p align="center">
<img width="913" height="872" alt="image" src="https://github.com/user-attachments/assets/a904a319-a97d-432e-8bf1-615b880d3490" />

</p>

*Funcionalidades mostradas en la captura:*
- Registro de compras con precio unitario, cantidad y proveedor asociado.
- Botón para **Descarga de Reporte en Excel (`.xlsx`)** con el consolidado de stock actual.

---

### 3.6 Módulo de Gestión de Menú Gastronómico

Definición de la carta del restaurante y vinculación de recetas a insumos del inventario.

#### Vista: Carta del Menú y Platos Disponibles
<p align="center">
<img width="920" height="932" alt="image" src="https://github.com/user-attachments/assets/3f41ddc0-cea2-4b4b-b5fb-4d8f7c347774" />

</p>

---

#### Vista: Composición de Recetas e Insumos por Plato
<p align="center">
<img width="303" height="267" alt="image" src="https://github.com/user-attachments/assets/8cc53331-e940-4b6e-b8a2-388ea90575de" />

</p>

*Captura sugerida: Formulario de plato con selector múltiple de insumos y porciones deducibles por venta.*

---

### 3.7 Módulo de Facturación

Liquidación de cuentas y generación de tickets para los pedidos finalizados.

#### Vista: Emisión de Factura y Liquidación
<p align="center">
<img width="957" height="854" alt="image" src="https://github.com/user-attachments/assets/6b2e75a9-660a-4ccd-9e35-d37780fd5f6a" />

</p>

*Funcionalidades mostradas en la captura:*
- Selección de comanda pendiente de cobro.
- Datos fiscales del cliente (NIT / Cédula, Razón Social).
- Selección de método de pago (Efectivo, Tarjeta, Transferencia).
- Desglose de Base Imponible, IVA (19%) y Total a pagar.
- Calculadora de cambio / vuelto según el importe recibido.

---

#### Vista: Historial de Facturas Emitidas
<p align="center">
<img width="918" height="533" alt="image" src="https://github.com/user-attachments/assets/ec482472-7594-4c8f-8b02-76282ab43583" />

<img width="974" height="665" alt="image" src="https://github.com/user-attachments/assets/55c450a2-409c-4392-a066-faf4d31ef205" />

<img width="905" height="556" alt="image" src="https://github.com/user-attachments/assets/711e4294-f3a0-4f06-986b-4eed447703cf" />

</p>

*Captura sugerida: Historial de facturas emitidas con fecha, cliente, método de pago, monto total y opción de reimpresión.*

---

### 3.8 Pasarela de Pagos en Línea (Wompi)

Cobro electrónico para clientes con tarjetas débito/crédito, PSE y transferencias.

#### Vista: Integración y Checkout de Pagos
<p align="center">
<img width="1140" height="657" alt="image" src="https://github.com/user-attachments/assets/e06a7ca9-e16a-4d22-93f7-453712031ff4" />

</p>

---

### 3.9 Configuración, Accesibilidad y Reportes

Ajustes del restaurante, preferencias visuales inclusivas y analítica.

#### Vista: Personalización y Accesibilidad (Modo Claro / Oscuro y Daltonismo)
<p align="center">
<img width="893" height="395" alt="image" src="https://github.com/user-attachments/assets/0b3e118d-f200-49a6-845c-3a1e1363e0fc" />

<img width="848" height="941" alt="image" src="https://github.com/user-attachments/assets/7c8c3425-2bf5-489a-80df-b04b25a6f1eb" />


</p>

*Opciones disponibles:*
- Alternador de Tema: **Modo Claro ☀️** y **Modo Oscuro 🌙**.
- Filtros para Daltonismo: **Visión Estándar**, **Deuteranopia**, **Protanopia** y **Tritanopia**.
- Escala tipográfica: Pequeña, Mediana y Grande.

---

#### Vista: Datos de la Empresa y Parámetros Operativos
<p align="center">
<img width="835" height="658" alt="image" src="https://github.com/user-attachments/assets/9265328b-033c-412c-b09a-22fbe733fa49" />
</p>

*Captura sugerida: Configuración de Nombre comercial, NIT, Teléfono, Dirección base para envíos y Tarifa de flete.*

---

#### Vista: Métricas de Rendimiento y Reportes Consolidados
<p align="center">


<img width="771" height="925" alt="image" src="https://github.com/user-attachments/assets/b1873e3e-9040-4020-8dc0-6ef369bf7644" />

</p>

---

## 🛠️ Stack Tecnológico

### Frontend
- **Framework:** [React 19](https://react.dev/)
- **Empaquetador y Build Tool:** [Vite 6](https://vitejs.dev/)
- **Estilos:** Vanilla CSS con variables de diseño, Glassmorphism, temas dinámicos (`data-theme`) y filtros SVG de accesibilidad.
- **Iconografía:** SVG nativos optimizados para máximo rendimiento.

### Backend
- **Lenguaje:** [Python 3.13+](https://www.python.org/)
- **Framework Web:** [Django 6.0+](https://www.djangoproject.com/)
- **API Framework:** [Django Ninja 1.6+](https://django-ninja.dev/) *(rápido, tipado estricto con Pydantic y documentación OpenAPI / Swagger automática)*.
- **ORM:** Django ORM con modelos relacionales.
- **Exportación de Datos:**
  - `openpyxl`: Generación y exportación de reportes tabulares en Excel (`.xlsx`).
  - `reportlab`: Renderizado de documentos PDF.

### Base de Datos & Despliegue
- **Base de Datos:** [PostgreSQL](https://www.postgresql.org/) (Compatible con Supabase, Neon, AWS RDS o PostgreSQL local).
- **Servidor WSGI/ASGI:** Gunicorn / Uvicorn.
- **Hosting sugerido:** Backend en [Render](https://render.com/) y Frontend en [Vercel](https://vercel.com/).

---

## ⚙️ Requisitos Previos

- **Git** (versión 2.30 o superior)
- **Python** (versión 3.11, 3.12 o 3.13)
- **Node.js** (versión 18.0 o superior) y gestor de paquetes **npm**
- **PostgreSQL** (local o en la nube)

---

## 🚀 Guía de Instalación y Ejecución Local

### 1. Clonar el Repositorio

```bash
git clone https://github.com/TU_USUARIO/ProyectoQuerencia.git
cd ProyectoQuerencia
```

---

### 2. Configuración del Backend

1. Abre una terminal y dirígete al directorio del backend:
   ```bash
   cd backend
   ```

2. Crea y activa un entorno virtual de Python:
   - **En Windows (PowerShell):**
     ```powershell
     python -m venv .venv
     .\.venv\Scripts\Activate.ps1
     ```
   - **En macOS / Linux:**
     ```bash
     python3 -m venv .venv
     source .venv/bin/activate
     ```

3. Instala las dependencias requeridas:
   ```bash
   pip install --upgrade pip
   pip install -r requirements.txt
   ```

4. Configura el archivo `.env` en la raíz de `backend/` (ver sección [Variables de Entorno](#-variables-de-entorno)).

5. Aplica las migraciones de la base de datos:
   ```bash
   python manage.py migrate
   ```

6. *(Opcional)* Crea un superusuario para acceder al panel de Django:
   ```bash
   python manage.py createsuperuser
   ```

7. Inicia el servidor de desarrollo:
   ```bash
   python main.py
   # O alternativamente:
   python manage.py runserver 127.0.0.1:8000
   ```
   El backend quedará escuchando en: `http://127.0.0.1:8000`

---

### 3. Configuración del Frontend

1. Abre otra terminal y navega al directorio del frontend:
   ```bash
   cd frontend
   ```

2. Instala las dependencias de Node.js:
   ```bash
   npm install
   ```

3. Configura la URL del backend en `src/App.jsx`:
   - Desarrollo local: `http://127.0.0.1:8000/api`
   - Producción: `https://super-duper-backend-pvrx.onrender.com/api`

4. Inicia el servidor de desarrollo de Vite:
   ```bash
   npm run dev
   ```

5. Abre en tu navegador la URL mostrada en consola (normalmente `http://localhost:5173`).

---

## 🔐 Variables de Entorno

### Backend (`backend/.env`)

```env
# Conexión a la base de datos PostgreSQL
DATABASE_URL=postgresql://usuario:contraseña@localhost:5432/nombre_bd

# Configuración de Seguridad Django
SECRET_KEY=tu_clave_secreta_super_segura
DEBUG=True

# Configuración de Pasarela de Pagos (Wompi)
WOMPI_PUBLIC_KEY=pub_test_xxxxxxxxxxxxxxxxxxxxxxxx
WOMPI_PRIVATE_KEY=prv_test_xxxxxxxxxxxxxxxxxxxxxxxx
WOMPI_EVENTS_SECRET=test_events_xxxxxxxxxxxxxxxxxxxx
```

---

## 📁 Estructura del Repositorio

```text
ProyectoQuerencia/
├── .github/                      # Flujos de trabajo CI/CD (GitHub Actions)
│   └── workflows/
│       └── django.yml
├── docs/                         # Documentación y capturas
│   └── screenshots/              # 📸 Carpeta de capturas para el README
├── backend/                      # Servidor y APIs en Django Ninja
│   ├── conexion/                 # Módulos de conexión a BD
│   ├── core/                     # Configuración principal (settings, urls)
│   ├── crud/                     # Lógica de operaciones CRUD
│   ├── esquemas/                 # Esquemas Pydantic / DTOs
│   ├── modelos/                  # Modelos relacionales ORM
│   ├── rutas/                    # Controladores y endpoints REST
│   │   ├── auth.py               # Autenticación y registro
│   │   ├── caja.py               # Comandas, pedidos y domicilios
│   │   ├── configuracion.py      # Datos de negocio y métricas
│   │   ├── facturacion.py        # Generación de facturas
│   │   ├── inventario.py         # Insumos, compras y reporte Excel
│   │   ├── menu.py               # Platos y recetas
│   │   ├── usuario.py            # Cuentas y roles
│   │   └── wompi.py              # Pasarela Wompi
│   ├── main.py                   # Script de inicio rápido
│   ├── manage.py                 # CLI de Django
│   └── requirements.txt          # Dependencias Python
└── frontend/                     # Aplicación SPA en React + Vite
    ├── public/                   # Recursos estáticos
    ├── src/                      # Código fuente de React
    │   ├── assets/               # Imágenes y vectores
    │   ├── App.css               # Estilos globales, temas y accesibilidad
    │   ├── App.jsx               # Enrutamiento, Auth y Dashboard principal
    │   ├── Caja.jsx              # Módulo de Caja y Domicilios
    │   ├── Configuracion.jsx     # Módulo de Apariencia, Negocio y Reportes
    │   ├── Facturacion.jsx       # Módulo de Facturación POS
    │   ├── Inventario.jsx        # Módulo de Inventario y Stock
    │   ├── MenuGestion.jsx       # Módulo de Gestión de Menú
    │   └── main.jsx              # Entrada de la app
    ├── package.json              # Dependencias de npm
    └── vite.config.js            # Configuración de Vite
```

---

## 🌐 Documentación de la API

La API cuenta con documentación interactiva autogenerada con Swagger / OpenAPI:

- **Swagger UI interactivo:** `http://127.0.0.1:8000/api/docs`
- **ReDoc UI:** `http://127.0.0.1:8000/api/redoc`
- **Especificación OpenAPI (JSON):** `http://127.0.0.1:8000/api/openapi.json`

Permite explorar y probar en vivo las operaciones de cada endpoint:
- `/api/auth` - Login, registro y validación de tokens.
- `/api/usuarios` - Administración de cuentas y roles.
- `/api/caja` - Pedidos, clientes y envíos.
- `/api/inventario` - Stock, proveedores, categorías y compras.
- `/api/menu` - Platos y recetas de cocina.
- `/api/facturacion` - Emisión e historial de facturación.
- `/api/configuracion` - Datos del establecimiento y métricas.
- `/api/wompi` - Webhooks y pagos en línea.

---

## ♿ Características de Accesibilidad

1. **Modo Claro y Oscuro:** Interfaz adaptable según el entorno de trabajo.
2. **Filtros para Daltonismo:** Adaptación de contraste y espectros cromáticos para:
   - *Deuteranopia* (dificultad para percibir tonos verdes).
   - *Protanopia* (dificultad para percibir tonos rojos).
   - *Tritanopia* (dificultad para percibir tonos azules).
3. **Escalabilidad de Texto:** Ajuste de tamaño tipográfico sin romper el diseño responsivo.

---

## 🤝 Contribuciones

Las contribuciones son bienvenidas:

1. Haz un Fork del repositorio.
2. Crea una rama para tu función: `git checkout -b feature/NuevaCaracteristica`.
3. Confirma tus cambios: `git commit -m 'Añadir nueva característica'`.
4. Sube la rama: `git push origin feature/NuevaCaracteristica`.
5. Abre un **Pull Request**.

---

## 📄 Licencia

Este proyecto está bajo la Licencia **MIT**. Consulta el archivo `LICENSE` para más detalles.

---

<p align="center">
  Desarrollado con ❤️ para <strong>La Querencia</strong> • Universidad del Valle
</p>
