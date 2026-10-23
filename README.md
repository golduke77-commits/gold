# 💎 Golduke - Sistema POS & Gestión Joyera SaaS

Plataforma integral de Punto de Venta (POS), control de inventario de metales preciosos (Oro 18K, 14K, Plata 925), compras por pesaje, plan separe, crédito a clientes, arqueo de caja y facturación con soporte para impresora térmica de 80mm / 58mm.

---

## ✨ Características Principales

- ⚖️ **Control de Inventario por Gramaje & Pesaje Joyero**: Stock en gramos reales (`kg`, `g`, `mg`, `oz`), radar de stock con ordenamiento ascendente/descendente y costo promedio ponderado.
- 🛒 **Punto de Venta (POS)**: Búsqueda ágil por código/SKU, selector de clientes con tipos de documento (CC, CE, Pasaporte, NIT), cálculo de precio según gramaje y soporte de múltiples formas de pago.
- 📦 **Módulo de Compras**: Registro de compras de oro y metales con actualización instantánea de stock y recálculo automático del costo promedio ponderado.
- 📅 **Plan Separe & Créditos**: Gestión de abonos, seguimiento de saldos y recordatorios de pago.
- 💰 **Arqueo y Cierre de Caja**: Registro de apertura, movimientos en efectivo, transferencias, QR y arqueo ciego con detección de discrepancias.
- 🧾 **Impresión Térmica Directa**: Tickets de venta, recibos de compra y comprobantes de abono formateados para impresoras térmicas ESC/POS (80mm y 58mm).
- 🔐 **Control de Acceso Basado en Roles (RBAC)**: Perfiles diferenciados para Super Admin, Gerente, Cajero y Contador.
- ☁️ **Persistencia Independiente**: Preparado para sincronización con MongoDB Atlas y persistencia local en `db.json` / LocalStorage.

---

## 🚀 Puesta en Marcha

### Prerrequisitos
- [Node.js](https://nodejs.org/) (versión 18 o superior)
- Instancia de [MongoDB Atlas](https://www.mongodb.com/) (opcional si se usa en modo local)

### Configuración de Variables de Entorno
Crea o edita tu archivo `.env` en la raíz del proyecto:
```env
# Cadena de conexión de tu cluster MongoDB Atlas para Golduke
MONGO_URI=mongodb+srv://<usuario>:<password>@cluster0.mongodb.net/golduke_pos?retryWrites=true&w=majority

# Puerto del servidor local (Por defecto 3000)
PORT=3000
```

### Ejecución
```bash
# Iniciar servidor local
npm start
```
El sistema estará accesible en `http://localhost:3000`.

---

## 🔑 Credenciales Iniciales de Administrador
- **Usuario:** `admin@golduke.com`
- **Contraseña:** `admin123`
- **Rol:** Super Admin

---

## 📄 Licencia
Propiedad de **Golduke Joyería**. Todos los derechos reservados.
