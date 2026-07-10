5. Requerimientos No Funcionales
    • Eficiencia (Rendimiento y tiempos de respuesta):
          - RNF-EF-01: Las consultas básicas (búsqueda de socios por CI o estado de cuenta) no deben tardar más de 1.5 segundos en retornar los datos en condiciones de red normales.
          - RNF-EF-02: El sistema debe soportar un mínimo de 50 usuarios administrativos concurrentes operando en la plataforma sin degradación del servicio.
          
    • Seguridad lógica y de datos (Autenticación y respaldos):
        ◦ RNF-SE-01: Todo acceso a los módulos privados (tanto para socios como para administradores) requerirá autenticación mediante correo y contraseña encriptada bajo el algoritmo SHA-256 o superior.
        ◦ RNF-SE-02: Se realizarán copias de seguridad (backups) incrementales automáticas de la base de datos relacional cada 24 horas a las 02:00 AM, almacenándose de forma segura en un servidor externo.
          
    • Usabilidad (Facilidad de uso y errores):
        ◦ RNF-US-01: El tiempo de aprendizaje estimado para que un nuevo usuario administrativo domine las operaciones esenciales (altas y cobros) no superará las 3 horas de inducción práctica.
        ◦ RNF-US-02: Los mensajes de error del sistema dirigidos al usuario final deben ser descriptivos y sin códigos técnicos (por ejemplo: "La cédula ingresada ya pertenece a un socio activo, intente de nuevo" en lugar de "SQL Error 1062: Duplicate entry").
