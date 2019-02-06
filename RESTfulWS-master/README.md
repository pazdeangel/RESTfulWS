# RESTfulWS

# Evidencia de "Computaci�n avanzada en Java " 



# Instalaci�n

Importar a Eclipse
1.Clic en File -> Import -> Existing Projects into Workspace.
2.Seleccionar carpeta donde se clon� el proyecto.
3.Maven install.

Exportar .war
1.Clic derecho sobre proyecto.
2.Export -> WAR file.

Desplegar el archivo .war
1.Descargar o exportar el archivo WAR.
2.Ir a la p�gina principal de Tomcat http://localhost:8090 o http://localhost:8080 por default.
3.Manager App.
4.Escribir el usuario y contrase�a correctos.
5.Choose File y seleccionar el archivo WAR.
6.Desplegar.

# Uso


Recurso api/v1/
1.GET: Lista los recursos disponibles.
2.OPTIONS: Documentaci�n del recurso.

Recurso api/v1/file
1.GET: Descarga un archivo mediante el par�metro path.
api/v1/file/?path=

2.POST: Sube un archivo mediante los par�metros name, dir y file.
api/v1/file/ name="imagen.jpg" dir="/Files" file@/Users/User/Downloads/imagen.jpg --form

3.DELETE: Elimina un archivo mediante el par�metro path.
api/v1/file/?path=

4.OPTIONS: Documentaci�n del recurso.

Recurso api/v1/directory
1.GET: Lista los archivos de un directorio mediante el par�metro dir.
api/v1/directory/?dir=

2.OPTIONS: Documentaci�n del recurso.

Recurso api/v1/notify
1.GET: Lista las notificaciones enviadas.
2.POST: Env�a una notificaci�n mediante los par�metros subject, message, toAddress y ccAddress.
api/v1/notify subject="hello" message="Hello from Spring" toAddress="a@email.com" ccAddress="b@email.com"

3.OPTIONS: Documentaci�n del recurso.

Recurso api/v1/user
1.GET: Lista los usuarios.
2.POST: Crea un usuario mediante los par�metros username, password y fullName.
api/v1/user username="user" password="pass" fullName="John Doe"

3.OPTIONS: Documentaci�n del recurso.

Recurso api/v1/user/{username}
1.GET: Muestra la informaci�n del usuario.
2.PUT: Actualiza la informaci�n del usuario mediante los par�metros username, password y fullName.
api/v1/user/user username="user" password="pass" fullName="John Doe"

3.DELETE: Elimina al usuario.
4.OPTIONS: Documentaci�n del recurso.

# Cr�ditos
Desarrollado Pascual Tzompantzi






