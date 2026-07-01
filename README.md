# GoEngine - Sistema de Gestión de Mantenimiento de Vehículos 🚚

Este proyecto es una solución integral para la gestión y control del mantenimiento de una flota de transporte de carga pesada, desarrollada para la materia **Fundamentos de Bases de Datos**.

## 📊 Modelo Entidad-Relación (Base de Datos MySQL)
A continuación se detalla de forma visual la estructura lógica, las tablas y las relaciones de llaves foráneas generadas de manera automática para el sistema:

![Modelo Entidad Relación](diagrama.png)

## 📝 Descripción del Proyecto
La base de datos centraliza y administra de manera eficiente la información de vehículos, repuestos, kilometrajes y órdenes de trabajo, facilitando un seguimiento minucioso para planificar intervenciones futuras y tomar decisiones basadas en datos confiables.

## 🛠️ Tecnologías Utilizadas
- **Base de Datos:** MySQL
- **Lenguaje de Programación:** Python 3 (usando `mysql-connector-python`)

## 🗂️ Estructura del Repositorio
- `sqlscript.sql`: Script completo para la creación de la base de datos `myEngineBase`, definición de tablas, relaciones (Foreign Keys) e inserción de datos de prueba.
- `GoEngine_conexion_mysql.py`: Módulo de conexión en Python que implementa operaciones CRUD mediante programación orientada a objetos.
- `Documento Principal Bases de Datos.docx`: Documentación formal con los requerimientos y el alcance del proyecto.

## 💻 Ejemplos de Consultas Incluidas
El sistema permite realizar análisis detallados mediante sentencias estructuradas como:
```sql
-- Consultar la programación de mantenimientos ordenados por el más reciente
SELECT * FROM myenginebase.programacion_mantenimiento ORDER BY Consecutivo_orden DESC;

-- Filtrar el historial de mantenimiento por la placa de un vehículo específico
SELECT * FROM myenginebase.registro_mantenimiento WHERE Placa ='STT030';
