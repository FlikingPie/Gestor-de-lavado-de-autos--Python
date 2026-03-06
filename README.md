# 🚗 Gestor de Lavado de Autos

Aplicación de escritorio desarrollada en **Python con Tkinter y SQLite** para gestionar clientes, vehículos y ventas en un negocio de lavado de autos.

El sistema permite registrar clientes, registrar autos, generar ventas, buscar información y generar reportes.

---

# 📌 Características

El sistema incluye las siguientes funcionalidades:

## 👤 Gestión de Clientes
- Agregar clientes
- Modificar clientes
- Eliminar clientes
- Visualizar clientes en una tabla
- Exportar lista de clientes a archivo `.txt`

Campos registrados:
- Nombre
- DNI
- Teléfono

---

## 🚘 Gestión de Autos
- Registrar autos
- Modificar autos
- Eliminar autos
- Visualizar autos en una tabla
- Exportar lista de autos a archivo `.txt`

Campos registrados:
- Placa
- Número de autos
- Tipo de lavado
- Precio

---

## 💰 Gestión de Ventas
- Registrar venta
- Eliminar venta
- Visualizar ventas
- Ordenar ventas por precio
- Exportar ventas a archivo `.txt`
- Generar **boleta en PDF**

Datos registrados:
- Cliente
- DNI
- Teléfono
- Placa
- Número de autos
- Tipo de lavado
- Precio

---

## 🔎 Sistema de Búsqueda

Permite buscar ventas por:

- Nombre del cliente
- DNI
- Placa del vehículo

---

## 📊 Reportes

El sistema puede generar reportes como:

- Lavado más vendido
- Listado de clientes según tipo de lavado:
  - Lavado Básico
  - Lavado Exterior
  - Lavado Motor
  - Lavado Vapor
  - Lavado Premium

---

## 📄 Generación de Boleta

Se puede generar una **boleta de venta en PDF** con los datos del cliente y el servicio realizado.

Ejemplo de información en la boleta:

```
BOLETA DE VENTA

Cliente: Juan Perez
DNI: 12345678
Teléfono: 987654321
Placa: ABC-123
Nro Autos: 1

DETALLE DEL SERVICIO
Tipo de lavado: Premium
Precio: S/ 45

Gracias por su preferencia
```

---

# 🛠 Tecnologías utilizadas

- **Python**
- **Tkinter** → Interfaz gráfica
- **SQLite3** → Base de datos
- **FPDF** → Generación de PDF
- **Tabulate** → Exportación de tablas

---

# 📂 Estructura del proyecto

```
GestorLavadoAutos/
│
├── main.py
├── Gestor de Lavado_de_Autos.db
├── ClientesAutos.txt
├── AutosLavados.txt
├── VentasLavados.txt
├── boleta_lavado.pdf
└── README.md
```

---

# 🗄 Base de Datos

El sistema utiliza SQLite con la siguiente tabla:

```
Lavado_de_Autos
```

Columnas:

| Campo | Tipo |
|------|------|
| Cliente | TEXT |
| DNI | INTEGER |
| Telefono | INTEGER |
| Placa | TEXT |
| Nro_Autos | INTEGER |
| Lavado | TEXT |
| Precio | REAL |

---

# 💲 Tipos de Lavado

| Tipo | Precio |
|-----|------|
| Básico | S/10 |
| Exterior | S/15 |
| Motor | S/25 |
| Vapor | S/25 |
| Premium | S/45 |

---

# ▶ Cómo ejecutar el programa

### 1️⃣ Instalar Python

Descargar Python desde:

https://www.python.org

---

### 2️⃣ Instalar dependencias

```
pip install tabulate
pip install fpdf
```

---

### 3️⃣ Ejecutar el programa

```
python main.py
```

---

# 📈 Posibles mejoras futuras

- Gráficos de ventas
- Login de administrador
- Estadísticas mensuales
- Exportación a Excel
- Interfaz con **CustomTkinter**
- Sistema de reportes más avanzado

---

# 👨‍💻 Autor
- Utrilla Solis, Angel Kyle