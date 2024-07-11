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
