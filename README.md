# HistoriasCalidadTeam2_202501


# Historia _: Recuperacion automática ante fallos

Prioridad: Alta

Atributo de calidad: Disponibilidad

-Cuando: Un microservicio crítico del sistema (como autenticación o gestión de OVA) deja de responder debido a algún fallo
         inesperado

-Dado que: El sistema está en estado de falla.

-Yo como: Administrador del sistema

-Quiero: Que el sistema detecte automáticamente la falla y reinicie el microservicio afectado sin intervención manual

-Y debe suceder: Que Kubernetes reinicie el pod del microservicio en menos de 10 segundos, mientras el balanceador de carga 
                 redirige el tráfico a otras instancias saludables para evitar interrupciones en el servicio.


# Historia _: Monitoreo del rendimiento en tiempo real

Prioridad: Alta

Atributo de calidad: Monitoreo

-Cuando: El consumo de CPU supera el 80% durante más de 5 minutos o la memoria principal excede el 75% por más de 10 minutos

-Dado que: El sistema está procesando múltiples solicitudes simultáneamente.

-Yo como: Ingeniero DevOps

-Quiero: Que el sistema envíe alertas automáticas sobre el estado del servidor.

-Y debe suceder: Que se genere una notificación en Grafana, permitiendo tomar acciones antes de que el servicio se degrade.
                 Se dispare una alerta en Prometheus que envíe un mensaje a Slack al Team.

