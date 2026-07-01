# GoEngine - Sistema de Gestión de Mantenimiento de Vehículos 🚚

Este proyecto es una solución integral para la gestión y control del mantenimiento de una flota de transporte de carga pesada, desarrollada para la materia **Fundamentos de Bases de Datos** [1].

## 📊 Descripción del Proyecto
La base de datos centraliza y administra de manera eficiente la información de vehículos, repuestos, kilometrajes y órdenes de trabajo, facilitando un seguimiento minucioso para planificar intervenciones futuras y tomar decisiones basadas en datos confiables [1].

## 🛠️ Tecnologías Utilizadas
- **Base de Datos:** MySQL
- **Lenguaje de Programación:** Python 3 (usando `mysql-connector-python`) [2]

## 🗂️ Estructura del Repositorio
- `sqlscript.sql`: Script completo para la creación de la base de datos `myEngineBase`, definición de tablas, relaciones (Foreign Keys) e inserción de datos de prueba [3].
- `GoEngine_conexion_mysql.py`: Módulo de conexión en Python que implementa operaciones CRUD (Crear, Leer, Actualizar, Eliminar) mediante programación orientada a objetos [2].
- `Documento Principal Bases de Datos.docx`: Documentación formal con los requerimientos y el alcance del proyecto [1].

## 💻 Ejemplos de Consultas Incluidas
El sistema permite realizar análisis detallados mediante sentencias estructuradas como [1]:
```sql
-- Consultar la programación de mantenimientos ordenados por el más reciente
SELECT * FROM myenginebase.programacion_mantenimiento ORDER BY Consecutivo_orden DESC;

-- Filtrar el historial de mantenimiento por la placa de un vehículo específico
SELECT * FROM myenginebase.registro_mantenimiento WHERE Placa ='STT030';
