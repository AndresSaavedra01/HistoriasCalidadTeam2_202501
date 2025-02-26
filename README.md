# HistoriasCalidadTeam2_202501

# Historia SEGURIDAD

Prioridad: Alta

Atributo de calidad: Seguridad

- Cuando: Un usuario accede al sistema para gestionar Objetos Virtuales de Aprendizaje (OVA) desde una conexión externa.

- Dado que: El sistema maneja información sensible de docentes y estudiantes.

- Yo como: Administrador del sistema.

- Quiero: Que el sistema proteja los datos contra ataques de inyección SQL, XSS y CSRF mediante autenticación segura con OAuth2/JWT.

- Y debe suceder: Que el sistema bloquee automáticamente cualquier intento de ataque y registre los eventos sospechosos para su posterior análisis.

Criterios de aceptacion

1. El sistema debe validar y sanitizar las entradas de los formularios para prevenir inyecciones SQL y XSS.


2. Las solicitudes HTTP deben incluir tokens JWT válidos para garantizar que solo usuarios autenticados accedan a los recursos.


3. El sistema debe rechazar cualquier solicitud que no incluya un token de autenticación válido.


4. Los eventos de seguridad sospechosos deben registrarse en un archivo de logs accesible solo por el administrador.


5. Las sesiones de usuario deben expirar automáticamente tras 30 minutos de inactividad.


# Historia _: Dispinibilidad al 99.99%

Prioridad: Crítica

Atributo de calidad: Disponibilidad

-Cuando: Un usuario accede a la plataforma en cualquier momento del dia, para subir contenido relacionado a un OVA

-Dado que: El sistema está en operación normal

-Yo como: Administrador del sistema

-Quiero: Que la plataforma se mantenga operativa con una dispinibilidad del 99.99%, con interrupciones mínimas y que cualquier incidente sea resuelto sin afectar la disponibilidad del servicio
         para garantizar el acceso continuo a los Objetos Virtuales de Aprendizaje (OVA)

-Y debe suceder: Que el sistema limite los tiempos de inactividad a un máximo de 52 minutos y 35 segundos al año, asegurando la continuidad operativa mediante monitoreo proactivo.


# Historia _: Respuestas a un error
Prioridad: Alta

Atributo de Calidad: Disponibilidad

-Cuando: Un servicio crítico del sistema deja de responder debido a un fallo inesperado.

-Dado que: El sistema está en un estado de falla y los usuarios dependen de su disponibilidad.

-Yo como: Administrador del sistema.

-Quiero: Que el sistema detecte automáticamente la falla y tome medidas correctivas sin intervención manual.

-Y debe suceder: Que el sistema restablezca el servicio en un tiempo menor a 10 segundos, minimizando la interrupción y asegurando que los usuarios puedan continuar con su flujo de trabajo sin afectaciones significativas.


# Historia _: Monitoreo del rendimiento en tiempo real

Prioridad: Alta

Atributo de Calidad: Monitoreo

-Cuando: El sistema presenta un alto consumo de recursos que podría afectar su desempeño.

-Dado que: La plataforma se encuentra en un estado crítico.

-Yo como: Administrador del sistema.

-Quiero: Recibir alertas automáticas cuando el sistema experimente un uso excesivo de recursos.

-Y debe suceder: Que el sistema detecte estos eventos y notifique oportunamente para que se tomen acciones correctivas y se eviten afectaciones en la experiencia del usuario.




# Historia de Integridad entre modulos

#### Prioridad: Alta

- **Atributo de calidad:** Integridad

- **Cuando:** El sistema requiera una nueva funcionalidad.

- **Dado que:** El proyecto debe contar con una evolución constante.

- **Yo como:** Administrador del  Sistema.

- **Quiero:** Que el la integracion de nuevos componentes se realice de manera modular sin afectar a la estabilidad del sistema.

- **Y debe suceder:** Que se asegure la compatibilidad entre tecnologias,  reduciendo la necesidad de reorganizar el codigo y minimizando el impacto en el rendimiento.
 
 # Historia de Rendimiento del sistema

#### Prioridad: Alta

- **Atributo de calidad:** Rendimiento

- **Cuando:** El sistema deba de procesar gran cantidad de solicitudes simultáneamente

- **Dado que:** el sistema debe de contar con tiempos de respuesta minimos

- **Yo como:** Administrador del  Sistema.

- **Quiero:** que el sistema optimice el uso de recursos, dando proriedad a las funciones requeridad

- **Y debe suceder:** Que se garantice una estabilidad bajo las altas cargas de trabajo, evitando cuellos de botella asegurando una experiencia fluida para los usuarios