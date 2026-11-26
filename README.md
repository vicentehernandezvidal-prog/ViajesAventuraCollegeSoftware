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

La guía exige desarrollar en **Python** y conectar la solución a una base de datos. El motor de base de datos, la interfaz y las librerías definitivas deben quedar registrados aquí una vez que el equipo los confirme.

Como referencia de organización técnica se revisó un proyecto Python/MySQL modular que separa entidades, repositorios, servicios, seguridad y menús. Esa estructura sirve como antecedente, pero no implica que este proyecto ya use MySQL ni que deba copiar esa implementación.

## Requisitos previos

- Python 3 instalado.
- Motor de base de datos seleccionado y en ejecución.
- Git para obtener y actualizar el repositorio.

Las dependencias definitivas se documentarán en `requirements.txt` cuando estén definidas.

## Puesta en marcha

Los pasos concretos de instalación y ejecución se incorporarán cuando exista una primera versión ejecutable. Como flujo esperado:

1. Clonar el repositorio.
2. Crear y activar un entorno virtual.
3. Instalar las dependencias declaradas por el proyecto.
4. Configurar las variables de entorno locales a partir de una plantilla, sin compartir credenciales.
5. Crear la base de datos e importar el esquema y los datos de prueba, si corresponde.
6. Ejecutar el punto de entrada documentado por el equipo.

## Estructura documental

```text
.
├── README.md
└── docs/
    ├── requisitos.md
    ├── modelado.md
    ├── arquitectura.md
    ├── seguridad.md
    ├── planificacion_agil.md
    ├── trazabilidad.md
    └── uso_ia.md
```

La estructura real del código se agregará a este README cuando se consolide la implementación.

## Documentos del proyecto

- [Requerimientos funcionales y no funcionales](docs/requisitos.md)
- [Modelado UML y BPMN](docs/modelado.md)
- [Arquitectura y persistencia](docs/arquitectura.md)
- [Seguridad](docs/seguridad.md)
- [Planificación ágil](docs/planificacion_agil.md)
- [Matriz de trazabilidad](docs/trazabilidad.md)
- [Registro y evaluación del uso de IA](docs/uso_ia.md)

## Trabajo ágil y equipo

El borrador de planificación del repositorio identifica a **Pipe** como Product Owner, a **Vicho** como Scrum Master y a ambos como desarrolladores. Confirmen estos roles con el equipo y mantengan el backlog actualizado. La planificación inicial considera aproximadamente dos semanas; el detalle y las fechas tentativas están en `docs/planificacion_agil.md`.

## Evaluación ES4

La guía establece cinco criterios: levantamiento de requerimientos (4.1.1), modelado UML/BPMN (4.1.2), metodología ágil (4.1.3), desarrollo Python con persistencia (4.1.4) y acceso seguro (4.1.5). El producto grupal incluye informe técnico, documentación y código fuente; además, cada integrante debe realizar una defensa individual y explicar su aporte, decisiones técnicas, seguridad, persistencia y uso de IA.

## Seguridad del repositorio

- No subir archivos `.env`, contraseñas, claves, tokens ni datos reales de clientes.
- Mantener una plantilla sin secretos, por ejemplo `.env.example`.
- Usar consultas parametrizadas para interactuar con la base de datos.
- No almacenar contraseñas en texto plano.
- Evitar incluir datos personales reales en capturas, respaldos o datos de prueba.

## Estado y mantenimiento

Este README es una base documental inicial. Antes de la entrega, revisen que los diagramas coincidan con el código, que los requisitos sean verificables y que las instrucciones de instalación se hayan probado desde un clon limpio del repositorio.
