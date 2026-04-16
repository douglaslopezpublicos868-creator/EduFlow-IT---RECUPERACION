# 🚀 EduFlow IT - Automatización de Notas con n8n

## 📌 Descripción del Sistema
EduFlow IT es un sistema de automatización que gestiona el envío de notificaciones de notas académicas utilizando n8n.  
Integra Google Sheets como base de datos y Gmail para el envío automático de correos a estudiantes.

Este flujo permite reducir procesos manuales, mejorar la eficiencia y garantizar una comunicación oportuna con los alumnos.

---

## 🛠️ Tecnologías Utilizadas
- n8n (automatización de procesos)
- Google Sheets (gestión de datos)
- Gmail API (envío de correos)

---

## 🔄 Flujo del Proceso

### 1. Disparador Manual
Permite ejecutar el flujo manualmente para pruebas o ejecución controlada.

### 2. Lectura de Datos
Obtiene información desde Google Sheets:
- Nombre del estudiante
- Nota final (PF)
- Correo electrónico
- Estado

### 3. Registro de Datos
Guarda los datos procesados para auditoría, debugging y trazabilidad.

### 4. Evaluación de Notas
Se utiliza una condición:
- PF < 4 → Reprobado
- PF ≥ 4 → Aprobado

---

## 📧 Envío de Notificaciones

### ✅ Estudiantes Aprobados
Se envía un correo automático de felicitación con:
- Nombre del estudiante
- Nota final

### ❌ Estudiantes Reprobados
Se envía un correo con:
- Notificación de reprobación
- Enlace al examen de recuperación

---

## 🔁 Control de Envíos
Se valida si el correo ya fue enviado para evitar duplicados.

---

## 🧹 Actualización de Datos
Se actualiza el estado del estudiante en Google Sheets para mantener control del proceso.

---

## ⚠️ Manejo de Errores
El sistema detecta fallos en la ejecución y envía una notificación automática al administrador con:
- Descripción del error
- Nodo afectado
- Fecha

---

## 🧠 Lógica del Sistema
La automatización se basa en una condición principal:
- Si la nota final es menor a 4 → recuperación
- Caso contrario → aprobación

---

## 📊 Resultados
- Automatización completa del proceso
- Reducción de errores manuales
- Notificaciones inmediatas
- Mejor control del estado de estudiantes

---

## 🎯 Conclusión
EduFlow IT demuestra cómo la automatización puede optimizar procesos educativos, mejorando la eficiencia operativa y reduciendo la carga administrativa.

---

## 🎥 Video Explicativo
🔗 https://drive.google.com/file/d/1x_P0rQKdgzRZpj-cxi_ZBE1t2MGWbaeO/view?usp=sharing

---

## 👨‍💻 Autor
Douglas Alexander Recinos Lopez
