# ServidorFTPIIS

# Configuración de un Servidor FTP en IIS

## Prerrequisitos

1. **Sistema Operativo**: Windows Server (versión 2008 o superior).
2. **IIS Instalado**: Asegúrate de que IIS esté instalado en tu servidor.

## Paso 1: Instalar el Servidor FTP

1. Abre el **Administrador del servidor**.
2. Selecciona **Agregar roles y características**.
3. En la ventana de **Asistente para agregar roles y características**, selecciona **Instalación basada en características o roles** y haz clic en **Siguiente**.
4. Selecciona tu servidor en la lista y haz clic en **Siguiente**.
5. En la sección de **Roles de servidor**, expande **Servidor web (IIS)**.
6. Expande **Servicios de rol** y selecciona **FTP Server**.
7. Asegúrate de que las siguientes opciones estén seleccionadas:
    - **FTP Service**
    - **FTP Extensibility**
8. Haz clic en **Siguiente** y luego en **Instalar**.

## Paso 2: Configurar el Sitio FTP

1. Abre el **Administrador de IIS**.
2. En el panel de conexiones, haz clic derecho en **Sitios** y selecciona **Agregar sitio FTP**.
3. Rellena los siguientes campos:
    - **Nombre del sitio FTP**: Asigna un nombre a tu sitio FTP.
    - **Ruta de contenido físico**: Selecciona la carpeta raíz del sitio FTP.
4. Haz clic en **Siguiente**.

## Paso 3: Configurar la Información de Enlace y SSL

1. Configura los siguientes parámetros:
    - **Dirección IP**: Selecciona la IP del servidor o usa "Todas las no asignadas".
    - **Puerto**: El puerto por defecto es 21.
    - **SSL**: Puedes seleccionar **Sin SSL** o **Requiere SSL** según tus necesidades.
2. Haz clic en **Siguiente**.

## Paso 4: Configurar la Autenticación y Autorización

1. Configura los siguientes parámetros:
    - **Autenticación**: Habilita **Autenticación anónima** y/o **Autenticación básica**.
    - **Autorización**:
        - **Permitir acceso a**: Selecciona **Todos los usuarios** o **Usuarios especificados**.
        - **Permisos**: Selecciona los permisos necesarios (Leer y/o Escribir).
2. Haz clic en **Finalizar**.

## Paso 5: Configurar el Firewall para FTP

1. Abre **Panel de control** y selecciona **Sistema y seguridad** > **Firewall de Windows**.
2. Haz clic en **Configuración avanzada**.
3. En **Reglas de entrada**, selecciona **Nueva regla**.
4. Selecciona **Puerto** y haz clic en **Siguiente**.
5. Selecciona **TCP** y especifica el **Puerto local específico**: 21.
6. Permite la conexión y selecciona los perfiles deseados (Dominio, Privado, Público).
7. Asigna un nombre a la regla y haz clic en **Finalizar**.

## Paso 6: Probar la Conexión FTP

1. Abre un navegador web o un cliente FTP.
2. Conéctate a tu servidor FTP usando la dirección IP y el puerto configurados.
3. Ingresa las credenciales de acceso (si se configuró autenticación).

## Consideraciones Adicionales

- **Seguridad**: Es recomendable habilitar SSL para conexiones FTP seguras.
- **Permisos de Carpeta**: Asegúrate de que las carpetas utilizadas por el servidor FTP tienen los permisos adecuados.

¡Y eso es todo! Ahora deberías tener un servidor FTP funcionando en IIS.


# Rúbrica para Evaluación de Procedimientos en Salud

| **Aspectos para evaluar**                                                                                     | **SI/NO** | **OBSERVACIONES** |
|---------------------------------------------------------------------------------------------------------------|-----------|--------------------|
| **Intubación**                                                                                               |           |                    |
| El personal de salud verifica los materiales antes de iniciar la intubación.                                 |           |                    |
| Se utiliza técnica aséptica durante la intubación.                                                           |           |                    |
| Se preoxigena al paciente antes de la intubación según las recomendaciones.                                  |           |                    |
| Se realiza monitoreo constante del paciente durante y después del procedimiento.                             |           |                    |
| Se utiliza un laringoscopio estéril y adecuado al tamaño del paciente.                                       |           |                    |
| El tubo endotraqueal se fija correctamente después de su colocación.                                         |           |                    |
| **Extubación**                                                                                               |           |                    |
| El personal informa al paciente y a los familiares antes de realizar la extubación.                         |           |                    |
| Se realiza preoxigenación antes de la extubación.                                                            |           |                    |
| Se evalúan signos de complicaciones post-extubación, como laringoespasmo o aspiración.                       |           |                    |
| Se coloca al paciente en posición adecuada para evitar complicaciones respiratorias.                         |           |                    |
| Se utiliza un carro de paro disponible en caso de emergencia.                                                |           |                    |
| **Infecciones Nosocomiales**                                                                                 |           |                    |
| Se realiza lavado de manos correctamente antes y después de cada procedimiento.                              |           |                    |
| Se utilizan guantes y mascarillas en cada interacción con pacientes de alto riesgo.                          |           |                    |
| Las áreas de trabajo se desinfectan regularmente según protocolo.                                            |           |                    |
| Se utiliza equipo desechable para cada procedimiento cuando es posible.                                      |           |                    |
| Se controla la temperatura y humedad del ambiente hospitalario para evitar el crecimiento microbiano.        |           |                    |
| **Colocación de Ropa para Aislamiento**                                                                      |           |                    |
| El personal utiliza correctamente el equipo de protección personal (EPP).                                   |           |                    |
| Se respetan las técnicas de aislamiento según la patología del paciente.                                     |           |                    |
| Se informa adecuadamente al paciente sobre el proceso de aislamiento.                                        |           |                    |
| Se verifica que todo el equipo de protección utilizado sea descartado adecuadamente al finalizar el turno.   |           |                    |
| Las batas son reemplazadas en cada turno para evitar contaminación cruzada.                                  |           |                    |
| **Canalización de Vena Periférica**                                                                          |           |                    |
| Se selecciona adecuadamente la vena para la canalización, priorizando las distales.                          |           |                    |
| Se utiliza material estéril y técnica correcta durante el procedimiento.                                     |           |                    |
| Se documenta correctamente la cantidad de solución administrada y otros detalles.                            |           |                    |
| El paciente es monitorizado constantemente durante la administración de soluciones intravenosas.             |           |                    |
| Se evita el uso continuo de la misma vena para prevenir colapso venoso.                                      |           |                    |
| **Curación (Plana, Irrigada y Avanzada)**                                                                    |           |                    |
| Se evalúa el estado de la herida antes de iniciar la curación.                                               |           |                    |
| Se utiliza solución fisiológica o Ringer lactato tibio según necesidad.                                      |           |                    |
| Se aplican apósitos adecuados al tipo de herida y condición del paciente.                                    |           |                    |
| Se utiliza técnica estéril durante todo el procedimiento.                                                    |           |                    |
| Se registran observaciones relevantes sobre la evolución de la herida en el expediente del paciente.         |           |                    |
| **Cuidado de Catéter de Hemodiálisis**                                                                       |           |                    |
| Se evalúa el sitio de inserción del catéter antes de cada sesión de hemodiálisis.                            |           |                    |
| Se sigue estrictamente el protocolo de asepsia para el manejo del catéter.                                   |           |                    |
| Se registran todas las observaciones relacionadas con el catéter en el expediente del paciente.              |           |                    |
| Se verifica la permeabilidad del catéter antes de cada sesión.                                               |           |                    |
| Se asegura que el catéter esté correctamente fijado para evitar desplazamientos o infecciones.               |           |                    |

