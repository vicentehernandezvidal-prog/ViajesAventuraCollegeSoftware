# Viajes Aventura — Sistema de gestión turística

Proyecto académico de la asignatura **TI3021 – Programación Orientada a Objeto Seguro**, correspondiente a la Evaluación Sumativa 4 

El objetivo es diseñar y desarrollar una solución de software en Python para apoyar la operación de **Viajes Aventura**, empresa dedicada a la planificación y venta de servicios turísticos. El sistema debe gestionar destinos, paquetes turísticos y reservas, incorporando autenticación, persistencia de datos y medidas para proteger la información de los clientes.


## Objetivos del proyecto

- Registrar, consultar, modificar y eliminar destinos turísticos.
- Crear paquetes turísticos que agrupen uno o más destinos, con fechas y costos.
- Consultar la disponibilidad y calcular el costo de los paquetes.
- Permitir el registro y autenticación de usuarios.
- Registrar reservas en una base de datos y consultar su historial.
- Validar los datos ingresados y proteger credenciales e información sensible.

## Alcance funcional

| Módulo | Capacidades contempladas |
|---|---|
| Destinos | Crear, listar, modificar y eliminar destinos. |
| Paquetes | Crear paquetes con múltiples destinos, fechas y costos; consultar disponibilidad y calcular costos. |
| Usuarios | Registrar usuarios y autenticar sus credenciales. |
| Reservas | Reservar paquetes, persistir reservas y consultar historial. |
| Seguridad | Validar entradas, controlar el acceso y proteger credenciales y datos sensibles. |

Los permisos concretos por tipo de usuario, los estados de reserva, las reglas de cancelación y los campos exactos de cada entidad deben ser acordados por el equipo y documentados antes de implementarlos.

## Tecnologías

Python 3.10 o superior.
MySQL/MariaDB (por ejemplo, XAMPP).

Librerias: 
- PyMySQL
- Python dotenv 
- request 
- bcrypt
- cryptography

## Requisitos previos

- Python 3 instalado.
- Motor de base de datos seleccionado y en ejecución.
- Git para obtener y actualizar el repositorio.

Las dependencias definitivas se documentarán en `requirements.txt` cuando estén definidas.

## Instalación

1. Clonar el repositorio.
2. Crear un entorno virtual: `python -m venv .venv`
3. Instalar dependencias: `pip install -r requirements.txt`
4. Copiar `.env.example` a `.env` y configurar las credenciales locales de MySQL.
5. Importar `database/schema.sql` desde phpMyAdmin o MySQL.
6. Importar `database/schema.sql` desde phpMyAdmin o MySQL.
