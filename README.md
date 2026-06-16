# Sistema_de_control_para_gimnasio
Sistema creado para gestionar membresias, asistencia, caja, profesores, mensajes de alerta y rutinas. Este sistema ayuda a la gestion de los gimnasios, fue creado como una web virtual pero empaquetado para su instalacion y funcionamiento local
# 🏋️‍♂️ Ragnarok Gym | Sistema Integral de Gestión y Control de Acceso (Showcase)

![NodeJS](https://img.shields.io/badge/Node.js-43853D?style=for-the-badge&logo=node.js&logoColor=white)
![Express](https://img.shields.io/badge/Express.js-404D59?style=for-the-badge)
![MySQL](https://img.shields.io/badge/MySQL-005C84?style=for-the-badge&logo=mysql&logoColor=white)
![Socket.io](https://img.shields.io/badge/Socket.io-black?style=for-the-badge&logo=socket.io&badgeColor=010101)
![JavaScript](https://img.shields.io/badge/JavaScript-F7DF1E?style=for-the-badge&logo=javascript&logoColor=black)

> 🔒 **Nota sobre el código fuente:** Este repositorio funciona como un caso de estudio arquitectónico (Showcase) para mi portfolio. El código fuente de la aplicación es privado por tratarse de un software comercial desarrollado a medida y actualmente en producción.

Ragnarok Gym es una plataforma Fullstack diseñada para automatizar y digitalizar la operativa diaria de un centro deportivo. Combina un robusto panel de administración con control de acceso en tiempo real y notificaciones automatizadas. 

> **💡 Destacado Arquitectónico:** El sistema está diseñado como una Web App, pero **empaquetado como una aplicación de escritorio portable** para Windows. Incluye sus propios binarios de Node.js y MySQL 8.4, permitiendo al usuario final instalar y ejecutar el sistema con un simple `.exe`, sin necesidad de configurar variables de entorno o instalar software de terceros.

---

## 📸 Interfaz y Funcionamiento
*(Nota: Arrastrá y soltá acá 3 o 4 capturas de pantalla de tu sistema. Sugerencia: una del panel principal/caja, una del molinete inteligente y una de las rutinas)*

---

## 🚀 Características Principales

* **Control de Acceso en Tiempo Real:** Interfaz tipo "Molinete Inteligente" potenciada por WebSockets (`socket.io`). Valida ingresos por DNI de forma instantánea, verificando estado del socio, pagos al día y límites de clases semanales.
* **Bot de WhatsApp Integrado:** Automatización de comunicaciones mediante `whatsapp-web.js`. El backend genera un código QR para vincular la cuenta del gimnasio, permitiendo enviar recordatorios de pago a clientes con cuotas vencidas mediante un solo clic.
* **Gestión Financiera y Caja Dinámica:** Registro automático de pagos de cuotas. Permite división de ingresos mediante un slider dinámico (Efectivo vs. Transferencia), registro manual de egresos y cálculo del balance neto mensual y diario.
* **Rutinas Personalizadas:** Sistema de interfaz tipo acordeón para diseñar y asignar rutinas semanales específicas para cada socio.
* **Seguridad y Roles:** Autenticación dinámica de usuarios. Rutas y vistas protegidas según el nivel de acceso (Dueño / Administrador).
* **Gestión de Socios (CRUD):** Altas, bajas, modificaciones, asignación de planes y vinculación con profesores.

---

## 🛠️ Stack Tecnológico

**Backend & Integraciones:**
* **Node.js & Express:** Creación de la API RESTful y servidor.
* **MySQL (mysql2/promise):** Base de datos relacional con manejo de peticiones asíncronas para máxima eficiencia.
* **Socket.io:** Comunicación bidireccional en tiempo real para el módulo de control de acceso.
* **whatsapp-web.js:** Integración de WhatsApp Web a nivel servidor para la automatización de mensajería.

**Frontend:**
* **HTML5 & CSS3:** Interfaces responsivas y modernas.
* **JavaScript Vanilla:** Manipulación eficiente del DOM y lógica de cliente sin depender de frameworks pesados, garantizando tiempos de carga óptimos.

**Arquitectura de Despliegue (Portable):**
* **Inno Setup:** Creación del instalador `.exe`.
* **Scripts Batch & VBS:** Orquestación y ejecución silenciosa del servidor Node y la base de datos MySQL en entornos Windows.

---
*Diseñado y desarrollado por [Ale Vallejo](https://www.linkedin.com/in/ale-vallejo-dev) 🚀*
