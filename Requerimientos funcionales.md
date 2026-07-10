3. Requerimientos Funcionales:
- RF1: Solicitud de Afiliación Web y Alta de Socio
      - Código unívoco: RF1 
      - Descripción detallada: El sistema debe permitir a un Postulante ingresar sus datos personales a través de un formulario web para solicitar unirse a la empresa. Posteriormente, un Administrador debe poder evaluar y aprobar dicha solicitud para transformarla en un registro de Socio activo con su respectiva Cédula de Identidad. 
      - Prioridad: Alta 
      - Acciones iniciadoras / Estímulos: El Postulante hace clic en "Enviar Solicitud" en el formulario web; el Administrador presiona el botón "Aprobar Solicitud" desde el panel de control.
      - Comportamiento esperado del sistema: El sistema valida que los campos obligatorios no estén vacíos y que la CI no esté duplicada. Guarda temporalmente la postulación. Al ser aprobada por el administrador, el sistema crea el registro correspondiente en la tabla Socio. 



RF2: Gestión de Miembros del Núcleo Familiar
      - Código unívoco: RF2 
      - Descripción detallada: El sistema debe permitir asociar un Socio Titular a un Grupo Familiar de manera unívoca, así como también vincular múltiples Personas (integrantes vivos o fallecidos) a dicho grupo. 
      - Prioridad: Alta 
      - Acciones iniciadoras / Estímulos: El Administrador ingresa al módulo de "Grupos Familiares", selecciona un Socio e introduce las cédulas y datos de los familiares a agregar. 
    • Comportamiento esperado del sistema: El sistema da de alta el identificador en GrupoFamiliar, crea las filas necesarias en Persona (con su estado "vivo o muerto") y actualiza las tablas intermedias de relación (Socio_GrupoFamiliar y GrupoFamiliar_Personas) manteniendo la integridad referencial. 







RF3: Registro y Control de Pagos Mensuales
      - Código unívoco: RF3 
      - Descripción detallada: El sistema debe permitir el registro de cada pago mensual efectuado por un socio, guardando de forma exacta el monto, la fecha de transacción, el mes correspondiente que se está abonando y el socio que realiza la acción. 
      - Prioridad: Alta 
      - Acciones iniciadoras / Estímulos: El Administrador ingresa al módulo de caja, busca la CI del socio y presiona "Registrar Pago". 
      - Comportamiento esperado del sistema: El sistema calcula y genera una nueva fila en la tabla Pago con un Idpago incremental automático, vinculándolo mediante la clave foránea a la CI del Socio respectivo, actualizando inmediatamente el saldo o estado de cuenta del mismo. 
