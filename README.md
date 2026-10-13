# HotelGest

Sistema de reservas y gestión de hotel para controlar habitaciones,
huéspedes, reservas, check-in/check-out y facturación.

## Datos del proyecto

| | |
|---|---|
| **Institución** | Universidad Tecnológica de Pereira |
| **Asignatura** | Entornos de Desarrollo de Software |
| **Proyecto** | Proyecto Integrador, primera entrega |
| **Integrante** | Oscar David Muñoz García |
| **Docente** | Juan Camilo Olarte |
| **Fecha** | 13 de octubre de 2026 |

## Problema

El hotel lleva las reservas de los huéspedes en cuadernos o en hojas de Excel.
Esto causa reservas duplicadas, poca claridad sobre qué habitaciones están
libres u ocupadas, facturas hechas a mano con errores y falta de información
sobre la ocupación.

## Objetivo

Centralizar la información del hotel en un sistema que automatice las
reservas, el check-in, el check-out y la facturación.

## Usuarios

| Usuario | Qué hace |
|---|---|
| Huésped | Consulta disponibilidad, reserva, cancela y ve su factura. |
| Recepcionista | Registra huéspedes y reservas, hace check-in y check-out y genera facturas. |
| Administrador | Gestiona habitaciones, tarifas y personal, y consulta reportes. |

## Funcionalidades principales

1. Gestión de habitaciones
2. Gestión de huéspedes
3. Reservas
4. Check-in y check-out
5. Facturación
6. Reportes de ocupación e ingresos

## Arquitectura

Arquitectura en tres capas:

- **Interfaz de usuario:** pantallas para huésped, recepcionista y administrador.
- **Lógica de negocio:** reglas de reservas, disponibilidad y facturación.
- **Acceso a datos:** almacenamiento de habitaciones, huéspedes, reservas y facturas.

## Estructura del repositorio

```
Hotelgest/
├── README.md
├── docs/
│   ├── analisis.md
│   ├── requerimientos.md
│   ├── arquitectura.md
│   └── diagramas.md
├── diagramas/
│   ├── casos-de-uso.puml
│   ├── clases.puml
│   ├── secuencia-reserva.puml
│   ├── arquitectura.puml
│   └── img/
└── src/
    ├── interfaz/
    ├── logica/
    └── datos/
```

La carpeta `src/` queda vacía en esta primera entrega: la implementación
se hará en la entrega final.

## Documentación

- [Análisis del sistema](docs/analisis.md)
- [Requerimientos funcionales y no funcionales](docs/requerimientos.md)
- [Arquitectura propuesta](docs/arquitectura.md)
- [Diagramas UML](docs/diagramas.md)

## Estrategia de ramas

| Rama | Uso |
|---|---|
| `main` | Versión estable. No se trabaja directamente sobre ella. |
| `develop` | Integración del trabajo. |
| `feature/*` | Una rama por cada tarea. |

## Flujo de trabajo

1. Actualizar `develop` con `git pull`.
2. Crear una rama `feature/...` desde `develop`.
3. Hacer commits pequeños y con mensajes claros (`docs:`, `chore:`, `feat:`).
4. Subir la rama y abrir un Pull Request hacia `develop`.
5. Revisar y hacer el merge.

## Estado del proyecto

Primera entrega: análisis, modelado y organización del proyecto.
Pendiente para la entrega final: implementación del sistema y base de datos.
