RF1: Solicitud de Afiliación Web

Descripción: El sistema permitirá a un Postulante completar un formulario en línea para solicitar su ingreso y el de su grupo familiar a la empresa fúnebre.

Prioridad: Alta.

Acciones iniciadoras / Estímulos: El Postulante hace clic en "Solicitar Afiliación" en el portal web público.

Comportamiento esperado del sistema: El sistema despliega el formulario, valida que los campos obligatorios (DNI, Nombre, Correo, Teléfono) sean correctos, verifica que el DNI no esté ya registrado, guarda la solicitud en estado "Pendiente" y envía un correo de confirmación al postulante.

RF2: Gestión de Miembros del Núcleo Familiar

Descripción: Permite al Socio Titular o al Administrador añadir, modificar o dar de baja a los integrantes del núcleo familiar cubiertos por el servicio.

Prioridad: Media.

Acciones iniciadoras / Estímulos: El Socio Titular inicia sesión, va a "Mi Cuenta" y selecciona "Agregar Familiar".

Comportamiento esperado del sistema: El sistema solicita los datos del familiar, aplica las Reglas de Negocio (parentesco válido y límite de edad), actualiza el registro vinculado al Socio Titular y recalcula, si corresponde, el valor de la cuota mensual.

RF3: Registro de Pagos Mensuales

Descripción: El sistema registrará los pagos de las cuotas de los socios, ya sea de forma automática mediante la pasarela de pago o de forma manual por el Administrador.

Prioridad: Alta.

Acciones iniciadoras / Estímulos: La pasarela de pagos envía una confirmación de transacción aprobada (webhook) o el Administrador ingresa un pago en efectivo.

Comportamiento esperado del sistema: El sistema busca al Socio Titular, genera el recibo digital de pago, actualiza el estado de cuenta a "Al Día", extiende la cobertura del mes correspondiente y emite una alerta en caso de que el pago sea parcial o rechazado.