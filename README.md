# HistoriasCalidadTeam2_202501


# Historia _: Dispinibilidad al 99.99%

Prioridad: Crítica

Atributo de calidad: Disponibilidad

-Cuando: Un usuario accede a la plataforma en cualquier momento del dia

-Dado que:  la plataforma debe estar operativa con una disponibilidad del 99.9999% para garantizar el acceso continuo a los Objetos Virtuales de Aprendizaje (OVA).

-Yo como: Administrador del sistema

-Quiero: Supervisar que la plataforma se mantenga operativa con interrupciones mínimas y que cualquier incidente sea resuelto sin afectar la disponibilidad del servicio.

-Y debe suceder:  Que el sistema limite los tiempos de inactividad a un máximo de 52 minutos y 35 segundos al año, asegurando la continuidad operativa mediante monitoreo proactivo y recuperación automática.


# Historia _: Monitoreo del rendimiento en tiempo real

Prioridad: Alta

Atributo de calidad: Monitoreo

-Cuando: El consumo de CPU supera el 80% durante más de 5 minutos o la memoria principal excede el 75% por más de 10 minutos

-Dado que: El sistema está procesando múltiples solicitudes simultáneamente.

-Yo como: Ingeniero DevOps

-Quiero: Que el sistema envíe alertas automáticas sobre el estado del servidor.

-Y debe suceder: Que se genere una notificación en Grafana, permitiendo tomar acciones antes de que el servicio se degrade.
                 Se dispare una alerta en Prometheus que envíe un mensaje a Slack al Team.

