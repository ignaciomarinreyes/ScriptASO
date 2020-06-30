# ScriptASO

Implementa una utilidad para visualizar los ficheros que se encuentran abiertos en el momento de hacer la llamada. Por cada fichero, se muestra el número de procesos que lo tienen abierto para leer y cuántos para escribrir, así como el nombre del propietario del fichero.
Se utiliza la información que hay en /proc.

El script admite la siguiente sintaxis:

ficheros_abiertos [-u lista_usuarios]

El argumento lista_usuarios se corresponde con una lista de nombres de cuentas de usuario separados por comas. El script sólo muestra ficheros cuyo propietario sea alguna de esas cuentas. Si se omite la opción -u, el script muestra todos los ficheros.
