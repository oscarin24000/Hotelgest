\# Arquitectura propuesta de HotelGest



\## Estilo elegido

Arquitectura en tres capas.



\## Componentes



| Capa | Función | Ejemplos en HotelGest |

|---|---|---|

| Interfaz de usuario | Pantallas con las que interactúan huésped, recepcionista y administrador. | Formulario de reserva, panel de recepción, reportes |

| Lógica de negocio | Reglas del hotel y procesos del sistema. | ServicioReserva, cálculo de factura, validación de disponibilidad |

| Acceso a datos | Guarda y consulta la información. | Base de datos de habitaciones, huéspedes, reservas y facturas |



\## Flujo

El usuario usa la interfaz, la interfaz llama a la lógica de negocio, y la lógica de negocio consulta o guarda datos en la base de datos. La interfaz nunca accede directamente a los datos.



\## Justificación

\- Separa responsabilidades: cada capa tiene una función clara.

\- Facilita el mantenimiento: se puede cambiar la interfaz sin tocar las reglas del hotel.

\- Permite repartir el trabajo si el equipo crece.

\- Corresponde con las carpetas del proyecto: `src/interfaz`, `src/logica` y `src/datos`.



\## Nota

Esta arquitectura se propone en la primera entrega; su implementación queda para la entrega final.

