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


# Historia de Integridad

#### Prioridad: Alta

- **Cuando:** El sistema requiera una nueva funcionalidad.

- **Dado que:** El proyecto debe contar con una evolución constante.

- **Yo como:** Administrador del  Sistema.

- **Quiero:** Que el la integracion de nuevos componentes se realice de manera modular sin afectar a la estabilidad del sistema.

- **Y debe suceder:** Que se asegure la compatibilidad entre tecnologias,  reduciendo la necesidad de reorganizar el codigo y minimizando el impacto en el rendimiento.
 
 