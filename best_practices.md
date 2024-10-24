1. Minimizar la Versión SDK a 30
   Al establecer el minSdkVersion en 30, aseguramos que la aplicación no se pueda instalar en dispositivos que ejecutan versiones de Android que contienen 
   vulnerabilidades conocidas y que no reciben actualizaciones de seguridad. Esto protege a los usuarios de ataques que exploten estas vulnerabilidades.
   
2. Desactivar la Depuración
   Al desactivar la depuración, evitamos que los atacantes puedan conectar un depurador al proceso de la aplicación. Esto dificulta la ingeniería inversa y la      explotación de vulnerabilidades, ya que el acceso a las clases de ayuda de depuración y la posibilidad de inspeccionar el estado de la aplicación se limita.  

3. Uso de Permisos Específicos
  Al proteger tu BroadcastReceiver con un permiso específico, aseguras que solo las aplicaciones que requieren dicho permiso 
  puedan interactuar con tu receptor. Esto protege tu aplicación contra el acceso no autorizado, pero es vital que revises el nivel de protección de dicho 
  permiso.

4. Desactivar Copias de Seguridad
    Deshabilitar la opción de copia de seguridad impide que los datos sensibles de la aplicación sean respaldados o exportados a través de ADB. Esto reduce el 
    riesgo de que información crítica se extraiga y sea utilizada maliciosamente por usuarios no autorizados.
