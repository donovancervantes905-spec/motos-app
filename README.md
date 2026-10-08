# 🏍️ MundoMotos™ - Plataforma Web de Motocicletas

Sitio web completo e interactivo desarrollado en **Python** (`codigo.py`) sin dependencias externas. Incorpora catálogo oficial de motocicletas, especificaciones completas, precios, cuotas estimadas, reseñas con valoraciones dinámicas, simulador acústico de motor y cotizador de crédito.

---

## 🚀 Cómo Iniciar el Sitio Web

Solo necesitas tener instalado Python en tu computadora (no requiere instalar librerías con `pip`):

```bash
python codigo.py
```

Al iniciarse:
1. El servidor HTTP comenzará en `http://localhost:8000`.
2. **Tu navegador web se abrirá automáticamente** con el sitio listo para usar.
3. Para detener el servidor, presiona `Ctrl + C` en la consola.

---

## ✨ Características Principales

### 1. 💰 Precios Claros & Financiamiento
- Precios de contado expresados en USD para cada modelo.
- Cálculo de **cuota mensual estimada** según enganche (10% al 60%) y plazo (12, 24, 36 o 48 meses).
- Simulador interactivo en tiempo real con tasa preferencial.

### 2. 📝 Descripciones Detalladas & Ficha Técnica
- Resumen de diseño y enfoque de manejo para cada modelo.
- Ficha técnica completa:
  - **Cilindrada**, **Potencia (HP)** y **Torque (Nm)**
  - **Velocidad máxima** y aceleración **0 a 100 km/h**
  - **Capacidad de tanque**, **peso** y tipo de transmisión.
  - Puntos destacados de chasis, electrónica y frenos.

### 3. ⭐ Sistema Dinámico de Reseñas y Valoraciones
- Calificaciones con estrellas (1 a 5 estrellas) y opiniones de probadores verificados.
- **Formulario interactivo para publicar nuevas reseñas**:
  - Ingresa tu nombre, título, calificación y comentario.
  - Se guarda automáticamente en el servidor (`motos_data.json`).
  - El promedio de estrellas de la moto se recalcula al instante en el catálogo.

### 4. 🔊 Simulador Acústico de Motor (Web Audio API)
- En el modal de detalle de cada moto, presiona el botón **"🔊 Acelerar"** para escuchar una síntesis sonora en tiempo real del acelerón de las revoluciones (RPM) según el motor.

### 5. 🎨 Selector de Colores y Lista de Favoritos
- Visualiza los colores oficiales de cada moto.
- Guarda tus modelos favoritos haciendo clic en el corazón; consúltalos en cualquier momento en la cabecera.

### 6. 📅 Formulario de Test Drive y Cotizaciones
- Reserva tu prueba de manejo o solicita asesoría personalizada.
- Las solicitudes se almacenan en `cotizaciones.json`.

---

## 🛠️ Estructura del Proyecto

```text
motos-app/
├── codigo.py           # Servidor web Python y aplicación completa
├── motos_data.json     # Base de datos local (motos, especificaciones y reseñas)
├── cotizaciones.json   # Registro de reservas y cotizaciones
└── README.md           # Documentación del proyecto
```
