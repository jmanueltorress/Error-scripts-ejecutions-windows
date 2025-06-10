Instrucciones para habilitar la ejecución de scripts en PowerShell

== Español ==

Para ejecutar scripts de PowerShell que no están firmados por una entidad de confianza, debes cambiar la política de ejecución.

Pasos:

1. Abre PowerShell como administrador:
   - Busca “PowerShell” en el menú de inicio.
   - Haz clic derecho sobre “Windows PowerShell”.
   - Selecciona "Ejecutar como administrador".

2. Si deseas habilitar temporalmente la ejecución de scripts (solo por esta sesión):

   Set-ExecutionPolicy -ExecutionPolicy Bypass -Scope Process

3. Si deseas habilitar permanentemente la ejecución de scripts para el usuario actual:

   Set-ExecutionPolicy RemoteSigned -Scope CurrentUser

⚠️ Precaución: Modificar la política de ejecución puede representar riesgos de seguridad. Asegúrate de entender las implicaciones antes de cambiarla.


== English ==

To run PowerShell scripts that are not signed by a trusted publisher, you need to change the execution policy.

Steps:

1. Open PowerShell as Administrator:
   - Search for “PowerShell” in the start menu.
   - Right-click on “Windows PowerShell”.
   - Select "Run as administrator".

2. To temporarily allow script execution (for the current session only):

   Set-ExecutionPolicy -ExecutionPolicy Bypass -Scope Process

3. To permanently allow script execution for the current user:

   Set-ExecutionPolicy RemoteSigned -Scope CurrentUser

⚠️ Warning: Modifying the execution policy can pose security risks. Be sure you understand the implications before making changes.
