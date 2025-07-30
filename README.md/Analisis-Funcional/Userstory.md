# User Stories – Proyecto: Pool Pay

## User Story 1

**ID:** US-001  
**Tipo de Usuario:** Comprador con nueva cuenta  
**Como** usuario nuevo sin cuenta,  
**Quiero** poder comprar un producto,  
**Para** agilizar la compra y proteger mi privacidad.

**Prioridad:** Alta  
**Criterios de Aceptación:**
- Puede acceder a productos sin login
- Puede pagar con wallet BTC ingresando solo dirección de entrega
- Recibe confirmación de pedido
- **Corrección:** Validación de dirección y límite de compra sin registro

---

## User Story 2

**ID:** US-002  
**Tipo de Usuario:** Usuario verificado  
**Como** usuario con cuenta,  
**Quiero** recibir una notificación cuando finaliza mi verificación de identidad,  
**Para** saber cuándo ya puedo operar sin restricciones.

**Prioridad:** Alta  
**Criterios de Aceptación:**
- Mensaje claro en pantalla al validar KYC
- Email + notificación push con aviso de aprobación
- **Corrección:** Incluir tiempo estimado de validación

---

## User Story 3

**ID:** US-003  
**Tipo de Usuario:** Comprador frecuente  
**Como** comprador frecuente,  
**Quiero** ver productos cercanos a mi ubicación,  
**Para** optimizar tiempos y costos de envío.

**Prioridad:** Media  
**Criterios de Aceptación:**
- El sistema detecta ubicación solo con consentimiento
- Se muestran productos según proximidad con indicador de distancia
- **Corrección:** Opción para ingresar ubicación manualmente

---

## User Story 4

**ID:** US-004  
**Tipo de Usuario:** Vendedor  
**Como** vendedor registrado,  
**Quiero** visualizar claramente la red de cripto utilizada (TRON, ERC20, etc.),  
**Para** evitar errores al transferir fondos.

**Prioridad:** Alta  
**Criterios de Aceptación:**
- Tooltip visible con red y comisiones antes de confirmar
- Validación automática de compatibilidad de red
- **Corrección:** Selección de red por defecto en perfil

---

## User Story 5

**ID:** US-005  
**Tipo de Usuario:** Usuario con wallet  
**Como** usuario activo,  
**Quiero** que las transferencias de fondos sean rápidas,  
**Para** evitar demoras que afecten mi experiencia.

**Prioridad:** Alta  
**Criterios de Aceptación:**
- Tiempo de transferencia menor a 1 minuto para redes rápidas
- Indicador de progreso en tiempo real
- **Corrección:** Alertas para transacciones lentas

---

## User Story 6

**ID:** US-006  
**Tipo de Usuario:** Usuario nuevo  
**Como** usuario en validación,  
**Quiero** que el segundo factor de autenticación solo se active cuando mi cuenta esté lista,  
**Para** no frustrarme con pasos innecesarios.

**Prioridad:** Alta  
**Criterios de Aceptación:**
- 2FA solo se habilita después de KYC aprobado
- Mensaje explicativo guiando al usuario
- **Corrección:** Tutorial opcional para configuración de 2FA

---

## User Story 7

**ID:** US-007  
**Tipo de Usuario:** Administrador de soporte  
**Como** agente Kriptonian,  
**Quiero** recibir alertas en tiempo real de fallas en pagos o validaciones,  
**Para** poder asistir rápidamente al usuario.

**Prioridad:** Media  
**Criterios de Aceptación:**
- Notificación con ID de usuario y tipo de error
- Acceso directo al historial del usuario afectado
- **Corrección:** Clasificación de alertas por urgencia

---

## User Story 8

**ID:** US-008  
**Tipo de Usuario:** Usuario frecuente  
**Como** usuario frecuente,  
**Quiero** invitar a otros mediante un sistema de referidos con recompensa,  
**Para** obtener un beneficio por cada persona que traigo a la plataforma.

**Prioridad:** Alta  
**Criterios de Aceptación:**
- Enlace único de invitación generado automáticamente
- Referido debe registrarse y completar primera transacción
- Recompensa en USDT para ambos usuarios
- Panel de control de referidos con estados
- **Corrección:** Límite mínimo de transacción para válidar referido.

---

# Preguntas para entrevistas cualitativas.
- Se desarrollan preguntas claves para comprender al usuario de la plataforma a la que se quiere llegar. Estas preguntas, permiten acceder a un punto neuralgico de desarrollo del producto entendiendo al usuario desde sus cimientos y acercarse al el mismo desde la mayor humildad y lograr acceder a el sin complicaciones en el desarrollo.

# PREGUNTAS DE ENTREVISTA – USUARIOS QUE USAN OTRAS PLATAFORMAS

1. ¿Ya pagaste algún producto o servicio con cripto? ¿Cuándo y por qué razón lo hiciste?

2. ¿Cómo fue que te enteraste y empezaste a usar la plataforma de pagos que usás actualmente?

3. ¿Qué plataforma usaste y qué te pareció su funcionamiento?

4. ¿Qué fue lo que más te gustó de esa plataforma? ¿Y qué fue lo que menos te gustó?

5. ¿Por qué elegiste esa plataforma para comprar con cripto?

6. ¿Te sentiste cómodo durante el proceso de registro o validación de identidad en otros productos?

7. ¿Qué parte de la plataforma te resultó confusa?

8. ¿Se te dificultó en algún momento pagar con tu wallet?

9. ¿Qué te gustaría mejorar del proceso de búsqueda o filtrado de productos?

10. ¿Qué tan seguro te sentiste al usar la plataforma para hacer pagos?

11. ¿Qué fue lo que más te frustró al usar tu plataforma?

12. ¿Preferís registrarte o comprar sin cuenta? En caso de que no te quieras registrar, comentanos por qué.

13. Cuando usabas alguna plataforma, ¿qué información sentiste que te faltó antes de confirmar tu compra?

14. En el caso de que tuvieras algún problema cuando usás una plataforma habitual y necesitás resolverlo con ayuda de soporte técnico, ¿te contactarías con soporte?

15. ¿Qué tan rápido fue el proceso de transferencia y confirmación cuando hacías los pagos en las plataformas que consumís para pagos?

16. ¿Cómo te gustaría recibir las notificaciones del sistema luego de realizar un pago?

17. ¿Te resultó claro qué red de cripto estabas usando (TRON, ERC20, entre otras) en la plataforma que usás habitualmente?

18. ¿Qué haría que recomiendes esta plataforma a otra persona?

# ENTREVISTA USUARIO ACTUAL – PREGUNTAS CUALITATIVAS

## PERFIL Y COMPORTAMIENTO

1. ¿Recordás cuál fue la primera vez que pagaste un producto o servicio con criptomonedas?
   - ¿Qué compraste y por qué elegiste pagar en cripto?

2. ¿Qué plataforma de pagos en cripto usás actualmente con más frecuencia?
   - ¿Cómo llegaste a conocerla o empezar a usarla?

3. ¿Qué tipo de productos o servicios solés pagar usando cripto hoy en día?
   - ¿Con qué frecuencia lo hacés?

## EXPERIENCIA DE USO

4. ¿Qué es lo que más te gusta de la plataforma que usás hoy para pagar con cripto?

5. ¿Y qué es lo que menos te gusta o más te incomoda?

6. ¿Te sentiste cómodo o tuviste dudas durante el proceso de registro o validación de identidad?
   - ¿Hubo algo que no entendiste o que te pareció innecesario?

## SEGURIDAD Y FLUJO DE PAGO

7. ¿Alguna vez sentiste inseguridad o desconfianza al momento de pagar con tu wallet en esa plataforma?

8. ¿Tuviste dificultades técnicas o errores al realizar pagos desde tu wallet?

9. ¿Te resultó claro qué red de criptomoneda estabas utilizando (TRON, ERC20, etc.) en cada transacción?

## NAVEGACIÓN Y BÚSQUEDA

10. ¿Qué opinás del buscador y los filtros de productos en la plataforma?
    - ¿Fue fácil encontrar lo que buscabas?

11. ¿Sentiste que faltaba información antes de confirmar una compra?
    - (Ejemplo: precio final, red usada, tiempo estimado de entrega)

## SOPORTE Y PROBLEMAS

12. Cuando tuviste un problema o consulta, ¿contactaste al soporte técnico?
    - ¿Cómo fue tu experiencia?

13. ¿Qué tan rápido fue el proceso de transferencia y confirmación en las plataformas que usás?
    - ¿Esperaste segundos, minutos o más tiempo?

## NOTIFICACIONES Y COMODIDAD

14. ¿Cómo preferís recibir notificaciones después de una compra o transacción?
    - (Ejemplo: email, mensaje directo, notificación en la app)

15. En general, ¿preferís registrarte o comprar sin crear una cuenta?
    - ¿Por qué?

## VALOR Y RECOMENDACIÓN

16. ¿Qué tendría que tener una plataforma para que vos la recomiendes a otros usuarios?
    - ¿Qué te haría cambiarte de la que usás hoy?

## Respuestas Sintetizadas de una entrevista a usuario real consumidor de una platadorma de cripto.

# ENTREVISTA USUARIO REAL – ALEXIS MAURIZ

## Perfil del Entrevistado
- **Nombre:** Nadine Barros  
- **Edad:** 23 años  
- **Rol:** Usuario activo de criptomonedas  
- **Plataforma actual:** Lemon Cash  
- **Criptomonedas usadas:** USDC (Circle), USDT  
- **Frecuencia de uso:** Mensual  

---

## ENTREVISTA SINTETIZADA

### SECCIÓN 1 – EXPERIENCIA EN OTRAS PLATAFORMAS

1. **¿Pagaste con cripto?**  
   Sí. En noviembre 2024, con USDC tras recibir mi primer pago.

2. **¿Cómo conociste la plataforma actual?**  
   Mi empleador usaba Lemon y me pagó por ahí.

3. **¿Qué plataforma usaste y cómo fue?**  
   Lemon, intuitiva pero necesité ayuda inicial.

4. **Lo mejor / peor de Lemon:**  
   + Lo mejor: bajas comisiones, fácil cambio a pesos.  
   − Lo peor: dificultad inicial con la wallet.

5. **¿Por qué elegiste esa plataforma?**  
   Porque mi cliente la usaba y necesitaba convertir cripto a pesos.

6. **¿Cómo fue el registro?**  
   Cómodo, simple e intuitivo.

7. **¿Qué parte fue confusa?**  
   Al principio, convertir USDC a pesos.

8. **¿Dificultades al pagar?**  
   No, aunque algunos comercios no aceptan Lemon.

9. **¿Qué mejorarías del filtrado?**  
   Nada, es intuitivo.

10. **¿Te sentiste seguro?**  
    Al principio dudé, pero luego sí.

11. **¿Qué te frustró más?**  
    Que pocos comercios acepten Lemon directamente.

12. **¿Preferís registrarte?**  
    Sí, por seguridad y trazabilidad.

13. **¿Faltó info antes de confirmar compra?**  
    No, todo claro.

14. **¿Contactarías soporte?**  
    Nunca lo necesité, pero sí lo haría.

15. **¿Velocidad de transferencia?**  
    Inmediata.

16. **¿Tipo de notificación preferido?**  
    Email.

17. **¿Red de cripto entendida?**  
    No, tuve que preguntar qué red era más económica.

18. **¿Recomendarías la plataforma?**  
    Sí, por su facilidad de uso y protección ante inflación.

---

### SECCIÓN 2 – USUARIO ACTUAL

19. **Primera compra con cripto:**  
    En noviembre 2024, mercadería tras recibir el pago.

20. **¿Qué plataforma usás y cómo la conociste?**  
    Lemon, recomendada por mi cliente.

21. **¿Qué pagás con cripto?**  
    Mercadería personal, cuando cobro.

22. **¿Qué te gusta más?**  
    Facilidad de uso y buena cotización.

23. **¿Qué incomoda más?**  
    Poca adopción general de Lemon.

24. **¿Algo que mejorarías del onboarding?**  
    Un video tutorial breve sería útil.

25. **¿Sentiste inseguridad?**  
    No.

26. **¿Errores técnicos?**  
    No.

27. **¿Entendiste qué red usar?**  
    No al principio. Debería estar más claro.

28. **¿Cómo fue el filtrado de productos?**  
    Intuitivo y fácil.

29. **¿Faltó información para comprar?**  
    No.

30. **¿Contactaste soporte?**  
    No, pero lo haría si fuera necesario.

31. **¿Tiempo de transferencia?**  
    Inmediato.

32. **¿Tipo de notificación?**  
    Email + comprobante visual en app.

33. **¿Preferís registrarte?**  
    Sí, para mayor seguridad.

34. **¿Qué te haría recomendarla?**  
    Recompensas por referidos ($10–20 USD por invitación).

# Tabla de Patrones para Priorización (Actualizada)

| Problema Detectado                     | Frecuencia | Relevancia | Solución Propuesta                  |
|----------------------------------------|------------|------------|-------------------------------------|
| Falta guía inicial sobre wallets       | Alta       | Alta       | Video tutorial en onboarding        |
| Confusión en selección de red          | Alta       | Alta       | Comparador de redes/comisiones      |
| Baja adopción en comercios             | Media      | Media      | Programa de incentivos a vendedores |
| Necesidad de incentivos por referidos  | Alta       | Alta       | Implementar US-008 con recompensas  |
| Transferencias lentas                  | Alta       | Alta       | Optimizar integración con redes     |

---

# Matriz de Priorización MoSCoW (Revisada)

| ID    | Historia de Usuario              | M  | S  | C  | W  | Justificación                          |
|-------|----------------------------------|----|----|----|----|----------------------------------------|
| US-001| Compra sin registro              | X  |    |    |    | Esencial para conversión               |
| US-004| Claridad en redes cripto         | X  |    |    |    | Previene errores costosos              |
| US-008| Sistema de referidos             | X  |    |    |    | Crecimiento orgánico                   |
| US-002| Notificación KYC                 |    | X  |    |    | Mejora experiencia onboarding          |
| US-005| Transferencias rápidas           |    | X  |    |    | Impacto directo en UX                  |
| US-006| 2FA condicional                  |    |    | X  |    | Reduce fricción inicial                |
| US-003| Geolocalización                  |    |    | X  |    | Valor agregado no crítico              |
| US-007| Alertas para soporte             |    |    |    | X  | Prioridad interna baja                 |

**Leyenda:**  
M = Must have, S = Should have, C = Could have, W = Won't have  

---

# Matriz de Trazabilidad de Requisitos (Completa)

| Req-ID | Requisito                           | Fuente          | User Story | Caso Prueba | Estado     |
|--------|-------------------------------------|-----------------|------------|-------------|------------|
| REQ-001| Checkout express sin registro       | Entrevista      | US-001     | TC-101      | Pendiente  |
| REQ-002| Notificación KYC aprobado           | US-002          | US-002     | TC-205      | Aprobado   |
| REQ-003| Filtro geolocalización              | US-003          | US-003     | TC-307      | En análisis|
| REQ-004| Visualización de red + comisiones   | Entrevista      | US-004     | TC-410      | Aprobado   |
| REQ-005| Transacciones <1 minuto             | US-005          | US-005     | TC-503      | Pendiente  |
| REQ-006| Activación 2FA post-verificación    | US-006          | US-006     | TC-618      | En diseño  |
| REQ-007| Panel de referidos con recompensas  | Entrevista      | US-008     | TC-809      | Pendiente  |
| REQ-008| Tutorial inicial interactivo        | Entrevista      | -          | TC-917      | Pendiente  |
| REQ-009| Selección de red por defecto        | US-004          | US-004     | TC-422      | Aprobado   |

---
---
## CASOS DE USO – CRYPTONITA-BT

---

## CASOS DE USO – CRYPTONITA-BT (Actualizados con mejoras)

---

## Caso de Uso 1: Registro e Identidad Verificada

**Actor Principal:** Persona sin cuenta

**Descripción:**  
El usuario que no posee cuenta accede a la plataforma, se registra completando todos los datos requeridos y valida su identidad mediante documentos, correo electrónico y verificación biométrica.

**Precondiciones:**

- El usuario accede a la plataforma por primera vez.
- No tiene cuenta registrada.

**Postcondiciones:**

- El usuario se encuentra registrado y verificado correctamente.
- Puede iniciar sesión y operar dentro de la plataforma.

**Flujo Principal:**

1. El usuario accede al enlace de la plataforma.
2. Visualiza las opciones de "Iniciar sesión" y "Registrarse".
3. Selecciona "Registrarse".
4. Completa los datos: nombre, apellido, código postal, teléfono, email.
5. Ingresa una contraseña de seis dígitos.
6. Activa el segundo factor de autenticación (2FA).
7. Carga fotos del documento (frontal y dorsal).
8. Realiza verificación facial: mueve rostro hacia derecha, izquierda, arriba, abajo.
9. Recibe un correo de confirmación con enlace para validar email.
10. Se crea la cuenta y se habilita acceso a la plataforma.

**Flujos Alternativos:**

- A1: No se confirma el correo → El usuario no puede operar.
- A2: Verificación facial inválida → Se solicita repetir el proceso.

---

## Caso de Uso 2: Inicio de Sesión e Interacción Inicial

**Actor Principal:** Usuario registrado

**Descripción:**  
El usuario registrado e identificado inicia sesión para comenzar a operar y acceder a funcionalidades de compra y navegación.

**Precondiciones:**

- El usuario ya está registrado y verificado.

**Postcondiciones:**

- Puede navegar la plataforma y ver productos/servicios disponibles.

**Flujo Principal:**

1. El usuario accede a la plataforma.
2. Hace clic en "Iniciar sesión".
3. Ingresa correo electrónico y contraseña.
4. Ingresa código de 2FA (si corresponde).
5. Accede a la interfaz principal con buscador y productos.

**Flujos Alternativos:**

- A1: Datos incorrectos → Se muestra error.
- A2: No se valida 2FA → Se solicita reintentar.

---

## Caso de Uso 3: Proceso de Compra

**Actor Principal:** Usuario registrado

**Descripción:**  
El usuario autenticado selecciona un producto, lo añade al carrito, y completa el proceso de pago mediante cripto wallet.

**Precondiciones:**

- El usuario inició sesión correctamente.

**Postcondiciones:**

- La compra queda registrada.
- Se notifica al usuario vía email y pantalla.

**Flujo Principal:**

1. El usuario navega o busca productos.
2. Selecciona uno y lo agrega al carrito.
3. Ingresa la dirección de entrega.
4. Revisa red cripto y comisiones.
5. Escanea QR o paga manualmente.
6. El sistema detecta el pago y valida hash.
7. Se genera recibo y notificación.

**Flujos Alternativos:**

- A1: El pago no se confirma → Se solicita reintentar.
- A2: Dirección inválida → Se muestra mensaje de error y se notifica.

**Mejora:**  
✔ Se implementa validación en tiempo real de la dirección de entrega y formato de wallet antes del paso 4.

---

## Caso de Uso 4: Notificación post-verificación (KYC)

**Actor Principal:** Usuario verificado

**Descripción:**  
El sistema notifica al usuario cuando su verificación KYC ha sido aprobada.

**Precondiciones:**

- El usuario completó el proceso de verificación.

**Postcondiciones:**

- Puede operar sin restricciones.

**Flujo Principal:**

1. El sistema valida la verificación.
2. Muestra notificación en pantalla.
3. Envía correo o push.
4. Activa automáticamente el sistema 2FA si estaba pendiente (según US-006).

**Mejora:**  
✔ Se incluye visualización del tiempo promedio estimado de validación (ej: “Su verificación será revisada en aprox. 3-5 minutos”).

---

## Caso de Uso 5: Visualización por proximidad

**Actor Principal:** Comprador frecuente

**Descripción:**  
El sistema muestra productos ordenados por cercanía geográfica al usuario.

**Precondiciones:**

- El usuario acepta compartir su ubicación.

**Postcondiciones:**

- Visualiza productos priorizados por distancia.

**Flujo Principal:**

1. El usuario ingresa al catálogo.
2. Autoriza uso de ubicación.
3. El sistema filtra productos cercanos.
4. Ordena de menor a mayor distancia.

---

## Caso de Uso 6: Visualizar red cripto antes de pagar

**Actor Principal:** Vendedor

**Descripción:**  
El sistema informa al comprador sobre la red blockchain del producto antes de pagar.

**Precondiciones:**

- El usuario va a realizar una transacción.

**Postcondiciones:**

- Evita errores por red equivocada.

**Flujo Principal:**

1. El vendedor configura la red en su producto.
2. El comprador la visualiza antes del pago.
3. Se muestran comisiones y red.
4. Se valida que coincidan red y wallet antes de permitir continuar.

---

## Caso de Uso 7: Alertas para soporte

**Actor Principal:** Administrador de soporte

**Descripción:**  
El sistema genera alertas internas cuando ocurren fallas en transacciones o validaciones.

**Precondiciones:**

- Se produce un error de pago o validación.

**Postcondiciones:**

- El equipo de soporte recibe notificación y puede actuar.

**Flujo Principal:**

1. El sistema detecta una anomalía.
2. Crea una alerta automática.
3. La alerta incluye el ID del usuario.
4. El administrador accede al historial del afectado.

---

## Caso de Uso 8: Sistema de referidos

**Actor Principal:** Usuario registrado

**Descripción:**  
El usuario puede invitar amigos y recibir recompensas si estos se registran y operan.

**Precondiciones:**

- El usuario está autenticado.

**Postcondiciones:**

- El sistema asigna recompensa.

**Flujo Principal:**

1. El usuario accede a su panel de referidos.
2. El sistema genera un link único.
3. El invitado se registra y realiza su primera transacción (mínimo $10).
4. El sistema valida operación y asigna USDT a ambos.
5. El usuario es notificado por email y panel.

**Mejora:**  
✔ Se establece un monto mínimo requerido para que el referido sea válido ($10).

---

## Caso de Uso 9: Onboarding con tutorial

**Actor Principal:** Usuario nuevo

**Descripción:**  
El sistema muestra un breve tutorial de bienvenida para entender cómo usar la wallet y hacer compras.

**Precondiciones:**

- El usuario crea una cuenta.

**Postcondiciones:**

- El usuario finaliza el tutorial o lo saltea.

**Flujo Principal:**

1. El sistema detecta que es el primer login.
2. Muestra un video tutorial (60 segundos) sobre uso de wallet y proceso de compra.
3. Se ofrece la opción “Saltar tutorial”.
4. El acceso al tutorial queda disponible en la sección de Ayuda.
5. El sistema marca como completado si el usuario lo termina.

**Relación:**  
✔ Este CU satisface la necesidad de onboarding expresada por el perfil usuario Nadine Barros.

---

## Caso de Uso 10: Confirmación visual del pago

**Actor Principal:** Usuario con wallet

**Descripción:**  
El sistema ofrece un comprobante visual y digital al confirmar una compra.

**Precondiciones:**

- La transferencia fue detectada correctamente.

**Postcondiciones:**

- El usuario visualiza su comprobante.

**Flujo Principal:**

1. El sistema valida el pago.
2. Genera un recibo en pantalla.
3. Lo envía por email.
4. Permite descarga o copia del hash.

---

## Caso de Uso 11: Selección de red por defecto

**Actor Principal:** Vendedor / Usuario avanzado

**Descripción:**  
Permite al usuario elegir una red cripto por defecto para evitar errores al recibir pagos.

**Precondiciones:**

- El usuario configuró su cuenta.

**Postcondiciones:**

- Toda transacción futura sugiere esa red.

**Flujo Principal:**

1. El usuario entra en configuración.
2. Selecciona red preferida (TRON, ERC20, BSC, etc.).
3. El sistema guarda la preferencia.
4. Todas las solicitudes futuras usan esa red como opción por defecto.

---

## Caso de Uso 12: Generación de hash y tracking de transacción

**Actor Principal:** Comprador

**Descripción:**  
El sistema permite al usuario copiar el hash de transacción para rastrear su operación en un explorador blockchain.

**Precondiciones:**

- El pago se ha confirmado.

**Postcondiciones:**

- El usuario puede hacer seguimiento externo.

**Flujo Principal:**

1. Al confirmar pago, se genera hash.
2. Se muestra al usuario junto con link al explorador.
3. El usuario puede copiarlo o abrirlo en nueva pestaña.

---
